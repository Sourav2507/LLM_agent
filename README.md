# 🌐 LLM Agent [Gleam AI](https://gleam-ai-agent.onrender.com/) — Browser-Based Multi-Tool Reasoning

This project is a **proof-of-concept (POC)** for building a **browser-based LLM agent** that can combine **natural language reasoning** with **external tools** like search engines, pipelined APIs, and even **live JavaScript execution**.

Modern LLM agents aren’t limited to text — they dynamically integrate multiple tools and loop until tasks are solved. This app demonstrates that idea with a **minimal, hackable UI + JavaScript agent core**.

---

## 🚀 Features

✅ **Multi-Provider Model Picker**  
- Choose between **AI Pipe Proxy API** (default), OpenAI GPT, Gemini, Claude, and others.  
- Dynamic dropdown for switching providers & models.

✅ **Reasoning Loop Agent**  
- Takes user input, queries the LLM, and loops with tool calls until the task is done.  
- Uses **OpenAI-style tool/function calls** for tool invocation.

✅ **Supported Tools**  
- 🔎 **Google Search Snippets** – Fetch relevant web info.  
- 🔗 **AI Pipe Proxy API** – Flexible AI workflows & pipelines.  
- ⚡ **JavaScript Sandbox** – Execute JS code securely inside the browser.

✅ **Robust UI/UX**  
- Bootstrap-based clean design.  
- Streaming-style chat window with file upload.  
- Graceful error handling via **bootstrap alerts**.  
- Performance monitor & tool action logging for debugging.

---

## 📋 Project Overview

### Goal

Build a minimal JavaScript-based agent that can:  
- Accept user input in the browser.  
- Query an LLM for reasoning.  
- Dynamically trigger **tool calls** (search, AI workflows, code execution).  
- Loop until the LLM decides no more tools are needed.


### JavaScript Implementation

This POC reimplements the above loop in **browser JavaScript**, connected to provider APIs.

---

## 🛠️ Getting Started

### Prerequisites

- A modern browser (Chrome/Edge/Firefox).  
- API keys for:  
  - [AI Pipe](https://aipipe.org/) proxy API (recommended)  
  - Optional: OpenAI, Gemini, or other providers.

### Setup

git clone https://github.com/Sourav2507/LLM_agent.git



### Running Locally


Open [http://localhost:8000](http://localhost:8000) in your browser.

### Deploy on Render.com

- Connect your GitHub repo on Render.  
- Select Web Service for backend (FastAPI), and Static Site for frontend if served separately.  
- Use branch `main` or your deployment branch.  
- Set build and start commands as needed for backend.  
- For static frontend, use publish directory `.` if files in root.  
- Deploy and visit your live URL.

---

## 📖 Usage

1. Enter your input text or markdown.  
2. (Optional) Add one-line guidance (e.g., "make it a research summary").  
3. Paste your LLM API key (OpenAI, Anthropic, Gemini).  
4. Upload `.pptx` or `.potx` template for styles.  
5. Click **Generate** to get your styled presentation.

---

## 🧪 Deliverable

- Fully functional browser-based AI agent with multi-tool integration  
- Support for web search, AI pipelines, and JS execution  
- Minimalistic UI with performance monitoring and error handling

---

## 📂 Project Structure

├── index.html # Frontend UI (chat + settings)
├── agent.js # Core agent loop, models, and tools
├── styles.css # Styling file
├── app.py # FastAPI backend if applicable
├── requirements.txt # Python dependencies
└── README.md # This documentation file



---

## 🙌 Acknowledgements

- [AI Pipe](https://aipipe.org/) for proxy API workflows  
- OpenAI / Anthropic / Google for LLM Providers  
- Bootstrap for UI components  

---

Feel free to reach out for further customization or deployment help!
