# MedBuddy

---

# 🧠 MedBuddy – Mental Health Chatbot

MedBuddy is an AI-powered **mental health support chatbot** built using **LangChain, Groq LLMs, and ChromaDB**. It provides compassionate, context-aware responses to user queries and can also retrieve insights from PDF documents (like medical journals or mental health resources).

# video : https://www.awesomescreenshot.com/video/43672880?key=c8a92e1389e416861f60d54bb3c8d8f6

---

## 🚀 Features

* 💬 **Conversational AI**: Powered by **Groq’s Llama-3.3-70B model** for empathetic and intelligent responses.
* 📚 **PDF Knowledge Base**: Upload medical/mental health PDFs to enhance chatbot responses using **ChromaDB vector search**.
* 🔎 **Retrieval-Augmented Generation (RAG)**: Combines LLM with stored embeddings for accurate, source-backed answers.
* 🌐 **Gradio UI**: User-friendly web interface with real-time chat support.
* 🔒 **Local Persistence**: Vector database stored locally (`./chroma_db`) for reuse across sessions.

---

## 🛠️ Tech Stack

* **Python**
* **LangChain** – Framework for LLM workflows
* **Groq LLM API** – High-performance inference
* **ChromaDB** – Vector store for embeddings
* **HuggingFace Embeddings** – Text embedding model
* **PyPDFLoader** – Extract text from PDF files
* **Gradio** – Interactive web-based chatbot UI

---

## 📂 Project Structure

```
medbuddy.py          # Main chatbot script
/content/data/       # Folder containing PDF knowledge base
/chroma_db/          # Persistent Chroma vector database
```

---

## ⚡ Setup & Usage

1. **Clone Repository & Install Dependencies**

   ```bash
   pip install langchain_groq langchain_core langchain_community
   pip install pypdf chromadb langchain_chroma gradio
   ```

2. **Run the Chatbot (CLI mode)**

   ```bash
   python medbuddy.py
   ```

   Type your query and the chatbot will respond. Type `exit` to quit.

3. **Run with Gradio UI**

   ```bash
   python medbuddy.py
   ```

   * A browser window will open with the chatbot UI.
   * Use `share=True` in `app.launch()` for public sharing.

---

## 🔮 Future Improvements

* Add **speech-to-text** support for voice conversations.
* Extend knowledge base with **medical datasets**.
* Fine-tune on **specialized therapy dialogues**.

---


