# 🔀 CMU Tepper's Navigator: A 24/7 Chatbot Companion App for Tepper using PALM2 + LangChain + OpenRouter + Streamlit 

**Note - Dont skip out on watching our result video below.**  
## Problem Introduction
Carnegie Mellon Tepper's MSBA program introduces students to a wide range of information related to job preparation, academics,immigration and life in Pittsburgh. While this information is meant to assist students in their transition to academic life it inadvertently overwhelms them. The information is scattered across various platforms, including Canvas, OIE, SIO, Slack, Handshake, Careernomics, Twelve20, and Tepper emails. This leads to confusion, stress, and inefficiency as students spend excessive time searching for relevant data, rather than focusing on their academic and personal growth. To assess the scope of these issues, a survey was conducted among 29 MSBA students from the class of 2023. The survey aimed to comprehend the challenges resulting from information overload and the difficulties students face in accessing the right information promptly. The primary goal of the survey was to empirically recognize and comprehend the challenges related to information retrieval faced by MSBA students.

![image](https://github.com/sherinegeorge21/Hackathon/assets/40655116/bac714a8-a6f2-4d9d-9210-d6d000e331be)

After analyzing the survey results, we discovered a crucial need for a centralized system to address inquiries and challenges within the Tepper School of Business. Motivated by this insight, we envisioned a groundbreaking solution. Our proposal is to develop a state-of-the-art helpbot, a user-friendly digital assistant designed to empower students on their Tepper journey, all powered by the cutting-edge Google Palm 2 API. This innovative helpbot aims to streamline information retrieval, reduce stress, and enhance the overall student experience. Our goal is not only to participate in the hackathon but to emerge as leaders in creating a valuable solution for our academic community all while harnessing the capabilities of the **Google Palm 2 API**.

## Tepper HelpBot
Our helpbot solution not only **answers student queries** but also empowers students to effortlessly **summarize text files** and efficiently **structure their assignments**. By combining intelligent information retrieval, text summarization, and assignment structuring, we're redefining how students approach their academic tasks. We've also harnessed the power of OpenRouter to connect with a range of LLM models, enabling us to conduct a comprehensive comparative analysis. This strategic feature is an asset that was build for the purpose of this hackathon to compare different models and is not intended to be taken for our project proposal. 
![image](https://github.com/sherinegeorge21/Hackathon/assets/40655116/ccde9abe-6b82-4d18-b01a-3e87761727a8)

Here are examples for building LLM apps with Streamlit and [OpenRouter](https://openrouter.ai), using [OpenRouter OAuth PCKE](https://openrouter.ai/docs#oauth).

## Overview of the App

https://github.com/sherinegeorge21/Hackathon/assets/40655116/418f49d2-b0c8-47af-a1cc-9138aba142b0

Our current solution includes:

**Helpbot** : To answer student queries based on our custom tuned model.

**Tepper File Q&A** - To summarize text documents or ask questions based on any text document.

**Tepper Langchain Quickstart** - Similar to the helpbot, but uses langchain for faster retrieval from the web, we plan to integrate LangChain into our tuned model.

**Tepper Langchain PromptTemplate** - This is to generate a basic outline for any assignment/blog/posts that students may need to write.

This app showcases a growing collection of OpenRouter minimum working examples, using a single API to access multiple language models, including [OpenAI GPT3/4, Anthropic Claude and Claude 100k, Google PaLM 2, and more](https://openrouter.ai/docs#models).

## Design and Implementation
![image](https://github.com/sherinegeorge21/Hackathon/assets/40655116/8fe02dcf-9787-44de-b3bf-14f879165a10)

## Data Ingestion
Although data preparation was comparatively difficult task we managed to divide it into four segments and synthesise it.We seamlessly segmented the process into four key categories: **Academic, Faculty, Admissions, and Lifestyle**. At present, we've harnessed our capabilities to train the model effectively on Academic and Faculty data. Our vision is to extend this by incorporating the remaining segments in the near future. 

**Examples:- Train Data**

Q. Who is the executive director for the Master Student Services?	

A. Wendy Hermann is the executive director for the Master Student Services.

Q. Who is teaching Experiential Learning?	

A. Ganesh Mani will be teaching Experiential Learning in mini 3.

Q. What is covered in the Optimization for Prescriptive Analytics course?	

A. In this course, the framework and techniques of mathematical optimization are introduced. The
course emphasizes modeling. That is, creating a mathematical description that reflects a given
real-world problem. Equipped with these models, we then discuss the necessary mathematical
techniques for finding optimal solutions. Finally, we consider the solution of these problems
using optimization software, i.e. we represent the models in either Excel or Python, and use a
solver to compute an optimal solution.

## Test Scenarios


## Drawbacks




## Running the code

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run Chatbot.py
```

## Getting API keys

Not needed! Your users will click the **Connect OpenRouter** button and auto-supply your app with a custom API key, using an [OAuth PKCE flow](https://openrouter.ai/docs#oauth).
