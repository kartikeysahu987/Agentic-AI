# Chatbot in LangGraph

A conversational chatbot built with **LangGraph** and **Streamlit**, using MCP (Model Context Protocol) tools for search, math, and other capabilities.

## Features

- **LangGraph** stateful chat with checkpointing (SQLite)
- **Streamlit** web UI with multiple conversation threads
- **MCP tools** (e.g. DuckDuckGo search, stock price, arithmetic, expense)
- **Hugging Face** or configurable LLM backend

## Setup

1. **Clone the repo** (or use your local folder):

   ```bash
   git clone https://github.com/YOUR_USERNAME/chatbot-in-langgraph.git
   cd chatbot-in-langgraph
   ```

2. **Create a virtual environment** (recommended):

   ```bash
   python -m venv .venv
   .venv\Scripts\activate   # Windows
   # source .venv/bin/activate   # macOS/Linux
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Environment variables** (optional):

   Create a `.env` file in the project root if you use API keys or override config (e.g. for OpenAI). The app can run with Hugging Face endpoints as configured in the code.

## Run

Start the Streamlit app:

```bash
streamlit run streamlit_frontend_mcp.py
```

Open the URL shown in the terminal (usually `http://localhost:8501`).

## Project structure

- `streamlit_frontend_mcp.py` – Streamlit UI and chat loop
- `langgraph_mcp_backend.py` – LangGraph graph, tools, MCP client, and checkpointing
- `requirements.txt` – Python dependencies

## License

Use as you like. Add your own license file if needed.
