# LangGraph AI Agent 🤖

An AI chatbot app built with **LangGraph**, **FastAPI**, and **Streamlit**. Supports multiple LLMs (Groq & OpenAI), web search via Tavily, and customizable system prompts.

## 🔥 Features

- ✅ Groq & OpenAI model support (LLaMA 3.3, Mixtral, GPT-4)
- 🔎 Optional web search using Tavily API
- ✍️ Custom system prompts
- 🧠 ReAct-style agent with tools
- 🖥️ FastAPI backend + Streamlit frontend

## 🛠️ Setup

### 1. Clone the Repository
bash
```
git clone https://github.com/yourusername/langgraph-ai-agent.git
cd langgraph-ai-agent
```
2. Install Dependencies
bash
```
pip install -r requirements.txt
```
3. Configure API Keys
Create a .env file in the root directory with the following:
bash
```
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```
🚀 Run the App
Start the Backend (FastAPI)
bash
```
python backend.py
📍 API available at: http://127.0.0.1:9999/docs
```

Start the Frontend (Streamlit)
bash
```
python frontend.py
📍 App runs at: http://localhost:8501

📡 API Endpoint
POST /chat
```

Request Example
json
```
{
  "model_name": "llama-3.3-70b-versatile",
  "model_provider": "Groq",
  "system_prompt": "Act as a helpful AI assistant",
  "messages": ["What is machine learning?"],
  "allow_search": true
}
```
