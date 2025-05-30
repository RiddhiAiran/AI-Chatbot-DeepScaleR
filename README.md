# 🤖 AI Chatbot with DeepScaleR

This project implements a local, privacy-focused AI chatbot using **DeepScaleR**. It consists of a FastAPI backend and a **Gradio** web UI, running entirely offline via **Ollama**. Ideal for general-purpose conversations with lightning-fast responses and no API costs.

---

## 🚀 Features

- 🧠 Local AI chatbot powered by DeepScaleR
- 🔒 No cloud or API usage — fully offline via Ollama
- 🧑‍💻 FastAPI backend for scalable API handling
- 🎨 Gradio-based UI for seamless interaction
- ⚡ Fast, low-latency responses

---

## 🛠️ Tech Stack

- Python
- FastAPI
- Gradio
- Ollama (for local inference)
- DeepScaleR model

---

## 📁 Project Structure

```
├── chatbot_api.py      # Backend API using FastAPI
├── chatbot_ui.py       # Frontend interface using Gradio
├── Modelfile           # Ollama model definition for DeepScaleR
├── requirements.txt    # Python dependencies
├── README.md           # Documentation
```

---

## 💻 Setup Instructions

### 1. Install Ollama

Download and install Ollama from [https://ollama.com](https://ollama.com), then pull the model:

```bash
ollama pull deepscaler
```

### 2. Clone the Repository

```bash
git clone https://github.com/riddhiairan/ai-chatbot-deepscaler.git
cd ai-chatbot-deepscaler
```

### 3. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the FastAPI Server

```bash
uvicorn chatbot_api:app --reload
```

### 5. Launch the Gradio UI

```bash
python chatbot_ui.py
```

---

## 📄 Modelfile Example

```
FROM deepscaler
SYSTEM "You are a helpful and friendly AI chatbot. Respond in a conversational and engaging manner."
```

---

## 🙌 Credits

- Model: [DeepScaleR via Ollama](https://ollama.com/library/deepscaler)
- UI: [Gradio](https://gradio.app)
- Backend: [FastAPI](https://fastapi.tiangolo.com/)
- Course: *Mastering DeepScaleR* by Vivian Aranha

---
