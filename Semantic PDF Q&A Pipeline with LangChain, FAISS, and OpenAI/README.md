# Semantic PDF Q&A Pipeline with LangChain, FAISS, and OpenAI

## Project Overview

This project demonstrates how to convert an unstructured PDF document into a searchable, structured knowledge base using vector embeddings, semantic search, and LLM-based question answering.
The PDF document I will be using is "COMMUNITY ARCHETYPES IN THE PERMIAN BASIN AND THEIR RELATIONSHIP TO ENERGY RESOURCES"

It uses:

- LangChain for orchestration
- OpenAI Embeddings for semantic representation
- FAISS for fast vector-based retrieval
- Unstructured PDF Parsing via LangChain's PyPDFLoader
- GPT-4 to answer natural language questions based on document conte

##  Features

- Load and parse PDF documents
- Split large documents into manageable chunks
- Generate embeddings and store them in a FAISS vector store
- Perform semantic search over document content
- Use GPT-4 for accurate and contextual Q&A

##  Use Cases

- Internal knowledge base search
- PDF document summarization
- Legal or energy industry documentation Q&A
- Reports and whitepaper intelligence

### Notes
- This pipeline uses OpenAI's text-embedding-3 models by default.
- You can switch to HuggingFace embeddings for an open-source version.
- FAISS stores the vector index in-memory by default, but it can be persisted to disk.
