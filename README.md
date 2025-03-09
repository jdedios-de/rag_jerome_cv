# CV Information Query API

This is a FastAPI application that enables users to ask natural language questions about Jerome de Dios's CV. It processes the CV (in PDF format), generates embeddings using a multilingual model, stores them in Pinecone, and uses LangChain with OpenAI's GPT-4o-mini to provide accurate answers through a retrieval-augmented generation (RAG) approach.

## Features

- **PDF Processing**: Loads and processes "Jerome de Dios.pdf".
- **Text Chunking**: Splits the CV into smaller, manageable chunks.
- **Embeddings Generation**: Uses the 'multilingual-e5-large' model to create embeddings.
- **Vector Storage**: Stores embeddings in a Pinecone index for efficient retrieval.
- **Question Answering**: Answers queries using a retrieval chain powered by LangChain and OpenAI.

## Prerequisites

- **Python**: Version 3.8 or higher.
- **API Keys**:
  - Pinecone API key
  - OpenAI API key
  - LangSmith API key (optional, for tracing)
- **PDF File**: "Jerome de Dios.pdf" must be present in the project directory.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/cv-query-api.git
   cd cv-query-api
