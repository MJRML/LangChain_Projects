# Retrieval-Augmented Generation (RAG) Pipeline with LangChain, OpenAI, and FAISS

## Project Overview

Extract knowledge from a PDF, store it as embeddings, and enable users to ask natural language questions and get precise, context-aware answers  
The PDF document I will be using is "COMMUNITY ARCHETYPES IN THE PERMIAN BASIN AND THEIR RELATIONSHIP TO ENERGY RESOURCES"

It uses:

- LangChain for orchestration
- OpenAI GPT models for generating answers
- FAISS for fast semantic search
- Unstructured documents (PDFs)

## Project Features: Document-Based QA System with LangChain
## Core Features
- PDF Ingestion  
-Load and extract content from PDF documents using PyPDFLoader.  

- Smart Text Chunking  
  -Use RecursiveCharacterTextSplitter to split large documents into overlapping, meaningful chunks.

- OpenAI Embeddings  
  -Generate dense vector embeddings that capture semantic meaning of each document chunk.

- Semantic Search via FAISS  
  -Store and retrieve document chunks with FAISS, enabling fast, similarity-based search.

- Natural Language Querying  
  -Accept user questions in plain English and match them with relevant document sections.

- GPT-4 Powered Answers    
  -Use ChatOpenAI and load_qa_chain to generate context-aware answers based on the matched chunks.

- Contextual Document Retrieval (RAG)  
  -Retrieval-Augmented Generation ensures answers are based on specific, grounded source content.

##  Use Cases

- Internal knowledge base search
- PDF document summarization
- Legal or energy industry documentation Q&A
- Reports and whitepaper intelligence

### Notes
- This pipeline uses OpenAI's text-embedding-3 models by default.
- FAISS stores the vector index in-memory by default, but it can be persisted to disk.
