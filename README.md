# 🧠 RAG From Scratch

A minimal **Retrieval-Augmented Generation (RAG)** implementation built from the ground up to demonstrate how modern LLM pipelines work internally — from document ingestion and embeddings to semantic search and grounded response generation.

This project focuses on clarity and learning rather than heavy frameworks, making it ideal for understanding how production-style RAG systems are structured.

---

## ✨ Overview

Retrieval-Augmented Generation combines:

* **Vector search** → find relevant context from data
* **Large Language Models** → generate grounded answers
* **Embeddings** → convert text into semantic vectors

This repository walks through building that pipeline step-by-step.

---

## 🚀 Features

* Build a RAG pipeline without hidden abstractions
* Environment-based API key handling
* Notebook-driven experimentation
* Clean modular structure
* Easy to extend with new models or vector stores

---

## 🏗️ Architecture

```
User Query
     ↓
Embedding Model
     ↓
Vector Search / Retrieval
     ↓
Context Injection
     ↓
LLM Generation
     ↓
Grounded Response
```

---

## 🧰 Tech Stack

* Python
* Jupyter Notebook
* Vector embeddings
* LLM inference (Groq API or compatible provider)
* dotenv for environment configuration

---

## 📂 Project Structure

```
RAG-From-Scratch/
│
├── notebook/
│   ├── rag_pipeline.ipynb
│   └── .env            # local secrets (ignored by git)
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Szransh/RAG-From-Scratch.git
cd RAG-From-Scratch
```

### 2️⃣ Create virtual environment (recommended)

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Variables

Create a local `.env` file inside `notebook/`:

```
GROQ_API_KEY=your_api_key_here
```

⚠️ Never commit `.env` files.
Use `.env.example` for sharing structure instead.

---

## ▶️ Usage

Start Jupyter:

```bash
jupyter notebook
```

Open the notebook inside the `notebook/` folder and run cells sequentially to:

1. Load documents
2. Generate embeddings
3. Build retrieval pipeline
4. Query the RAG system

---

## 🧪 Learning Goals

This project is useful if you want to understand:

* How embeddings enable semantic search
* Why prompt grounding improves LLM accuracy
* What happens internally in frameworks like LangChain or LlamaIndex

---

## 🛠️ Roadmap

* [ ] Add chunking strategies
* [ ] Streaming responses
* [ ] Hybrid search (keyword + vector)
* [ ] Evaluation metrics for retrieval quality
* [ ] Web UI demo

---

## 🤝 Contributing

Contributions, issues, and suggestions are welcome.
Feel free to fork the repo and open a pull request.

---

## 📄 License

MIT License — use freely for learning and experimentation.
