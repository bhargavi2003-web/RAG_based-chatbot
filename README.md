
# RAG-Based PDF Question Answering Chatbot

## Project Overview

This project is a Retrieval-Augmented Generation (RAG) application that allows users to ask questions about PDF documents and receive relevant answers using an LLM.

## Technologies Used

- Python
- LangChain
- Groq API
- Openai-oss 20b
- Hugging Face Embeddings
- ChromaDB
- Gradio
- LangSmith

## Project Workflow

1. Load PDF documents.
2. Split documents into smaller text chunks.
3. Convert text chunks into vector embeddings.
4. Store embeddings in ChromaDB.
5. Retrieve relevant document chunks based on user queries.
6. Pass retrieved context to the LLM.
7. Generate answers with source information.

## Features

- PDF document question answering
- Semantic search
- Context-based answers
- Source document retrieval
- Interactive Gradio interface

## Installation

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file and add:

```text
GROQ_API_KEY=your_groq_api_key
LANGCHAIN_API_KEY=your_langsmith_api_key
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=RAG_PDF_CHATBOT
```

Run the application:

```bash
python app.py
```
