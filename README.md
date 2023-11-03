# 🔀 OpenRouter + Streamlit Example App

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)]

Here are examples for building LLM apps with Streamlit and [OpenRouter](https://openrouter.ai), using [OpenRouter OAuth PCKE](https://openrouter.ai/docs#oauth).

## Overview of the App

This app showcases a growing collection of OpenRouter minimum working examples, using a single API to access multiple language models, including [OpenAI GPT3/4, Anthropic Claude and Claude 100k, Google PaLM 2, and more](https://openrouter.ai/docs#models).

Current examples include:

- Chatbot
- File Q&A
- Langchain Quickstart
- Langchain PromptTemplate
- LangChain Search

## Demo App

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openrouter.streamlit.app/)

## Running the code

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run Chatbot.py
```

## Getting API keys

Not needed! Your users will click the **Connect OpenRouter** button and auto-supply your app with a custom API key, using an [OAuth PKCE flow](https://openrouter.ai/docs#oauth).
