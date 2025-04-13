
# 📄 PDF Question Answering Bot using AWS Bedrock, LangChain, FAISS, and Streamlit

This project is a Streamlit-based web application that allows users to interactively ask questions from PDF files using powerful Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG). The solution uses **Amazon Bedrock** for LLMs and embeddings, **LangChain** for orchestration, **FAISS** for vector storage, and **Streamlit** for the UI.

---

## 🚀 Features

- 🧠 Query PDFs using AWS Bedrock-hosted LLMs (Claude or LLaMA2)
- 📄 Upload and split PDFs using LangChain's document loaders
- 🧩 Generate and store embeddings with Titan Embeddings via Bedrock
- ⚡ Fast retrieval powered by FAISS
- 🖥️ Simple and responsive Streamlit user interface
- 🛠️ RAG-based response generation with custom prompt templates

---

## 🏗️ Architecture Overview

1. **Data Ingestion**: Load and split PDF documents.
2. **Vectorization**: Generate embeddings using Amazon Titan Embeddings and store them using FAISS.
3. **LLM Retrieval**: Use Bedrock-hosted Claude or LLaMA2 for answering questions.
4. **RAG Chain**: Retrieve relevant chunks and use them in prompt-driven QA generation.
5. **Web UI**: Streamlit interface for uploading files, updating vector store, and querying.

---

## 🧰 Tech Stack

- **AWS Bedrock** – For LLMs and Embedding Models
- **LangChain** – Orchestration & RAG chain setup
- **FAISS** – Vector store for document similarity search
- **Streamlit** – Interactive web application UI
- **boto3** – AWS SDK for Python to interface with Bedrock

---

## 📂 Project Structure

```
project/
│
├── data/                     # Folder to store PDF documents
├── faiss_index/             # Saved vector index files
├── app.py                   # Main Streamlit application
└── README.md                # Project documentation (this file)
```

---

## ▶️ How to Run

1. **Clone the repository**:

```bash
git clone https://github.com/Regu7/AWS-Bedrock-LLM-RAG.git
cd AWS-Bedrock-LLM-RAG
```

2. **Install required packages**:

```bash
pip install -r requirements.txt
```

3. **Place your PDFs** in the `data/` directory.

4. **Run the Streamlit app**:

```bash
streamlit run app.py
```

---

## 📌 Notes

- Make sure your AWS credentials are configured and have access to Bedrock.
- You can use the sidebar to create or update the FAISS vector store.
- Two models (Claude and LLaMA2) are available via button interaction for response generation.

---

## 📜 License

MIT License. See [LICENSE](LICENSE) for more details.

---

## 🙌 Acknowledgements

- [Amazon Bedrock](https://aws.amazon.com/bedrock/)
- [LangChain](https://www.langchain.com/)
- [FAISS](https://github.com/facebookresearch/faiss)
- [Streamlit](https://streamlit.io/)
