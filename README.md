# Advanced AI Agent with LangGraph

The agent performs **deep research** by pulling **live data** from sources like **Google**, **Bing**, and **Reddit**, and processes it through a structured, modular architecture.

The tutorial focuses on:
- Advanced Python concepts  
- Agent architecture and orchestration  
- Working with live web data  
- Best practices for building scalable, multi-step AI systems  

---

## 🧠 Features

- LangGraph-powered agent framework  
- Multi-source data retrieval (Google, Bing, Reddit)  
- Integration with Bright Data APIs  
- Dynamic prompt chaining and reasoning  
- Customizable dataset and payload configuration

## 🔧 Setup Guide for the AI Agent Project
🔑 API Keys and Environment Setup

You’ll need your own Bright Data and OpenAI API keys.

In the .env file, replace the placeholders (****) with your own keys:

OPENAI_API_KEY=****

BRIGHTDATA_API_KEY=****

## 🗂️ Bright Data Setup
You’ll need to create two separate datasets in Bright Data:

One for reddit_search_api, and one for reddit_post_retrieval.

Each dataset has its own dataset_id.

In the code, you’ll see something like this inside web_operations.py:

dataset_id = "****"

Replace **** with the correct dataset ID for each API connection.

## 📦 Payload Configuration

The Bright Data payload used in this project is called "ai_agent".
If you want to rename it, you must change it in both places:

In your Bright Data dashboard

In the codebase (where "ai_agent" is referenced)

Consistency between Bright Data and your local code is required for it to work properly.
