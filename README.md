# Agentic RAG with Hallucination Filtering & Self-Reflection

This project implements an intelligent, modular Retrieval-Augmented Generation (RAG) system using LangGraph, designed to produce factually grounded responses by actively detecting and reducing hallucinations.

The system routes each user query through an adaptive flow that includes retrieval, answer generation, hallucination grading (via both LLM and NLI models), and self-reflective correction. It supports both indexed document retrieval and live web search, making it flexible for multi-domain applications.



![Screenshot 2025-06-14 150943](https://github.com/user-attachments/assets/505fa0be-8e61-49d3-9231-6b67824d74b2)

## Core Capabilities
- Query classification and routing to vector DB or web search
- Context-aware retrieval using FAISS or Tavily API (Web search) for unrelated queries
- Answer generation via OpenAI's GPT-4o
- Binary Hallucination filtering with LLM-based grading
- Adaptive question rewriting and self-reflection for unreliable outputs

## Tech Stack
- **LangGraph** for agentic flow control
- **LangChain** for retrievers and prompt chaining
- **OpenAI GPT-4o** for generation and structured grading
- **FAISS** for document vector search
- **Tavily API** for live web results

This prototype serves as a step toward building self-aware, hallucination-resistant LLM agents that prioritize answer quality and reliability.
