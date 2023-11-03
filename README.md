# 🔀 CMU Tepper's Navigator: A 24/7 Chatbot Companion App using PALM2 + OpenRouter + Streamlit

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)]

Carnegie Mellon Tepper's MSBA program introduces students to a wide range of information related to job preparation, academics,immigration and life in Pittsburgh. While this information is meant to assist students in their transition to academic life it inadvertently overwhelms them. The information is scattered across various platforms, including Canvas, OIE, SIO, Slack, Handshake, Careernomics, Twelve20, and Tepper emails. This leads to confusion, stress, and inefficiency as students spend excessive time searching for relevant data, rather than focusing on their academic and personal growth. To assess the scope of these issues, a survey was conducted among 29 MSBA students from the class of 2023. The survey aimed to comprehend the challenges resulting from information overload and the difficulties students face in accessing the right information promptly. The primary goal of the survey was to empirically recognize and comprehend the challenges related to information retrieval faced by MSBA students.

Here are the results of the survey:
![image](https://github.com/sherinegeorge21/Hackathon/assets/40655116/bac714a8-a6f2-4d9d-9210-d6d000e331be)


Here are examples for building LLM apps with Streamlit and [OpenRouter](https://openrouter.ai), using [OpenRouter OAuth PCKE](https://openrouter.ai/docs#oauth).

## Overview of the App

This app showcases a growing collection of OpenRouter minimum working examples, using a single API to access multiple language models, including [OpenAI GPT3/4, Anthropic Claude and Claude 100k, Google PaLM 2, and more](https://openrouter.ai/docs#models).

Current examples include:

- Helpbot
- Tepper File Q&A
- Langchain Quickstart
- Langchain PromptTemplate

## Running the code

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run Chatbot.py
```

## Getting API keys

Not needed! Your users will click the **Connect OpenRouter** button and auto-supply your app with a custom API key, using an [OAuth PKCE flow](https://openrouter.ai/docs#oauth).
