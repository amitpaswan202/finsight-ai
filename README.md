# FinSight AI – Financial Knowledge Assistant

## Overview
FinSight AI is a document-grounded AI assistant designed to answer
financial questions strictly from verified documents such as policies,
guidelines, and FAQs.

The project focuses on building a **real AI system using
Retrieval-Augmented Generation (RAG)** with an emphasis on accuracy,
trust, and explainability — key requirements for fintech products.

---

## Problem Statement
Generic AI chatbots often produce confident but incorrect answers.
In fintech, this can lead to misinformation and compliance risk.

FinSight AI addresses this by ensuring:
- Responses are grounded in uploaded documents
- The system avoids hallucinations
- Answers are explainable and traceable

---

## Key Features
- Upload financial documents (PDF/Text)
- Document chunking and embedding
- Semantic search using vector similarity
- Question answering using retrieved context
- Source references for answers
- Safe fallback when no relevant information is found

---

## Architecture Overview
1. Documents are uploaded and parsed
2. Text is split into overlapping chunks
3. Each chunk is converted into embeddings
4. Embeddings are stored in a vector database (FAISS)
5. User queries retrieve the most relevant chunks
6. The LLM generates an answer strictly from the retrieved context

---

## Tech Stack
- Backend: Python, FastAPI
- Embeddings: Sentence Transformers
- Vector Store: FAISS
- LLM: Local LLM (Llama 3 via Ollama), pluggable
- Frontend: React

---

## Scope
### Included
- Single-user prototype
- Local document ingestion
- Embedding-based semantic retrieval
- Context-grounded answer generation
- Basic web interface

### Out of Scope
- Authentication & authorization
- Model fine-tuning
- Production deployment
- Real-time data ingestion
- Multi-language support

---

## Example Use Cases
- Internal financial knowledge assistant
- Policy and FAQ automation
- Compliance-safe AI responses
- Support team enablement

---

## Future Enhancements
- Cloud vector database
- Document versioning
- Access controls
- Advanced reranking models

---

## Status
Initial design and development in progress.
