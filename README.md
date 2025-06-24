# LangGraph-RAG-Pipeline

Agent-based Retrieval-Augmented Generation (RAG) using LangGraph and Large Language Models (LLMs).

## Project Overview

This project explores an agent-based architecture for Retrieval-Augmented Generation. It uses LangGraph to dynamically route queries through modular components such as:

- **Retriever**
- **Rewriter**
- **Reranker**
- **Grader**
- **LLM Generator**

The pipeline is designed to reduce hallucinations, improve traceability, and enhance the quality of LLM-generated responses.

## Files Included

- `final_code.ipynb`: Full implementation of the LangGraph-based agent pipeline using Sentence-BERT and FAISS.
- `Agentic_RAG.pdf`: Project report summarizing the architecture, implementation, and evaluation results.
- `.gitattributes`, `.DS_Store`: System/configuration files.

## Evaluation Metrics

The performance of the pipeline was evaluated using:

- Cosine Similarity
- Context Precision @10 (CP@10)
- ROUGE-L
- METEOR

Ablation studies were conducted to assess the impact of each agent node.

## Setup Instructions

> This project runs in a Jupyter environment.

**Dependencies:**

- `sentence-transformers`
- `faiss-cpu`
- `transformers`
- `langchain`
- `langgraph`
- `openai` (optional for testing other LLMs)
