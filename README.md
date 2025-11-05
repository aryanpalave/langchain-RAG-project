# LangChain RAG Project

## Overview
This project implements a Retrieval-Augmented Generation (RAG) pipeline using LangChain. It allows large language models (LLMs) to provide grounded, accurate responses by retrieving relevant context from external documents before generating answers.


## Architecture

1. **Document Loader** – Reads and extracts text from PDF, TXT, Markdown, or other files.  
2. **Text Splitter** – Breaks large documents into smaller overlapping chunks for better embedding and retrieval.  
3. **Embedding Model** – Converts text chunks into numerical vectors using OpenAI or HuggingFace embeddings.  
4. **Vector Store (ChromaDB)** – Stores embeddings and enables fast similarity search for relevant context.  
5. **Retriever** – Finds the top-k most relevant document chunks for a given query.  
6. **LLM (LangChain Chain)** – Takes the retrieved context and generates a grounded, coherent answer.  
7. **Query Interface** – A Python script or API endpoint where users input natural language questions and receive responses.
