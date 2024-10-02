
# 📚 Botgauge AI Internship Assignment - Multi-Stage Text Retrieval Pipeline

## Project Overview

This repository contains the assignment for the **Botgauge AI Internship**, focused on building a **multi-stage text retrieval pipeline** for question-answering tasks. The goal is to implement and benchmark **embedding** and **ranking models** to evaluate their impact on retrieval accuracy and understand the trade-offs between model size, accuracy, and performance.

### 🎯 Task Objectives:

- **Literature Review**: Study the provided paper on multi-stage text retrieval and summarize the key points.
- **Dataset Preparation**: Use public Q&A datasets from the **BEIR benchmark** (e.g., Natural Questions, HotpotQA, and FiQA) and preprocess them for the task.
- **Candidate Retrieval (Stage 1)**: Implement retrieval using two embedding models (one small, one large).
- **Reranking (Stage 2)**: Use two ranking models to reorder the retrieved passages based on relevance scores.
- **Benchmarking**: Evaluate retrieval accuracy using **NDCG@10** and compare the impact of different model combinations.

## 🛠️ Approach

1. **Paper Understanding**: The foundation of the task is based on the concepts explained in the paper [https://www.arxiv.org/abs/2409.07691]. The focus is on how **ranking models** enhance retrieval accuracy in Q&A systems.
2. **Model Selection**:
   - **Embedding Models**: `sentence-transformers/all-MiniLM-L6-v2` and `nvidia/nv-embedqa-e5-v5`.
   - **Ranking Models**: `cross-encoder/ms-marco-MiniLM-L-12-v2` and `nvidia/nv-rerankqa-mistral-4b-v3`.
3. **Pipeline Stages**:
   - **Stage 1 (Candidate Retrieval)**: Retrieve top-k passages using embedding models.
   - **Stage 2 (Reranking)**: Reorder retrieved passages using ranking models.
4. **Evaluation**: Measure performance using **NDCG@10** and compare accuracy with and without reranking.

## 📊 Benchmark and Evaluation

The performance of the retrieval pipeline will be evaluated using the **NDCG@10** metric. We will compare the effectiveness of different embedding and ranking model combinations to analyze trade-offs in accuracy and performance.

---

### 🚀 Author

This assignment is being solved by **Shubham Murtadak**, aspiring AI intern, as part of the **Botgauge AI Internship** selection process.

---

