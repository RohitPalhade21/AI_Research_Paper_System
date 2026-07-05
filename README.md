# 🧠 AI Research Paper Intelligence System

An intelligent research paper retrieval system that enables semantic search over machine learning research papers using Natural Language Processing (NLP). Instead of relying on exact keyword matching, the system understands the meaning of a user's query and returns the most relevant papers based on semantic similarity.

---

## 🌟 Overview

Searching through thousands of research papers using keywords often misses relevant results. This project addresses that limitation by converting research papers into vector embeddings and performing semantic similarity search using FAISS.

The system allows users to search research papers using natural language queries such as:

> "Deep learning for medical image analysis"

and retrieves the most semantically relevant papers along with their titles, abstracts, and similarity scores.

---

## 🔑 Key Features

- Semantic search instead of keyword search
- Fast vector similarity search using FAISS
- Transformer-based sentence embeddings
- Research paper retrieval with similarity scores
- Efficient embedding and index caching
- Easy to extend for larger datasets

---

## 🏗️ Project Pipeline

```
Research Papers
       │
       ▼
Dataset Loading
       │
       ▼
Text Preprocessing
       │
       ▼
Sentence Embedding
(MiniLM)
       │
       ▼
FAISS Vector Index
       │
       ▼
User Query
       │
       ▼
Query Embedding
       │
       ▼
Similarity Search
       │
       ▼
Top Relevant Papers
```

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Dataset | Hugging Face Datasets |
| NLP | Sentence Transformers |
| Embeddings | all-MiniLM-L6-v2 |
| Vector Database | FAISS |
| Data Processing | Pandas, NumPy |
| Similarity | Cosine Similarity |
| Environment | Google Colab |

---

## 📂 Dataset

The project uses the **ML-ArXiv Papers Dataset** available on Hugging Face.

Dataset contains over **117,000 Machine Learning research papers** with:

- Title
- Abstract

To reduce computation time, this implementation indexes the first **15,000 papers**.

---

## ⚙️ How It Works

1. Load the research paper dataset.
2. Merge paper titles with abstracts.
3. Generate dense vector embeddings using Sentence Transformers.
4. Store embeddings inside a FAISS index.
5. Convert the user's query into an embedding.
6. Retrieve the Top-K most similar research papers.

---

## 📊 Sample Search

**Query**

```
Deep learning for medical image analysis
```

**Output**

- A Perspective on Deep Imaging
- Convolutional Neural Networks for Medical Image Analysis
- Classification of MRI Data using Deep Learning
- High Resolution Breast Cancer Screening
- Deep Learning for Classification of Lung Nodules

---

## 📁 Project Structure

```
AI_Research_Paper_System/
│
├── data/
├── notebooks/
├── src/
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🚀 Future Enhancements

- Streamlit Web Application
- PDF Upload & Search
- Paper Summarization using LLMs
- Research Paper Recommendation System
- Citation Export
- Hybrid Search (Keyword + Semantic)

---

## 👨‍💻 Author

**Rohit Palhade**

Second-Year Information Technology Student

Interested in:
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Data Science

GitHub: https://github.com/RohitPalhade21

---

### ⭐ If you found this project useful, consider giving it a star!
