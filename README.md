# 📊 Simple RAG System on Video Game Sales

This project implements a *simple Retrieval-Augmented Generation (RAG) pipeline*
from scratch using a structured CSV dataset of video game sales.

The goal is to demonstrate how a language model can **answer questions strictly
based on retrieved data**, without hallucinating information.

---

## 🧠 What is implemented

The pipeline follows these steps:

1. Load a CSV dataset (vgsales.csv)
2. Convert each row into a text document
3. Generate vector embeddings for documents
4. Store embeddings in a vector database
5. Retrieve the most relevant documents for a user query
6. Generate an answer *only using retrieved context*

If the answer is not present in the data, the model explicitly responds:
> "I don't know based on the provided data."

---

## 🛠️ Tech Stack

- Python
- Pandas
- Sentence Transformers
- FAISS (vector search)
- Hugging Face Transformers
- Google Colab / Jupyter Notebook

---

## ▶️ How to run the project

1. Open 01_rag_simple.ipynb in *Google Colab*
2. Upload the dataset vgsales.csv
3. Install dependencies:
```bash
pip install -r requirements.txt
