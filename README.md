#LLMAPP: PDF Question Answering with LangChain, OpenAI, and Pinecone#

This project demonstrates how to build a question-answering system over a collection of PDF documents using modern LLM and vector database tools. It uses LangChain for document processing and orchestration, OpenAI for embeddings and language models, and Pinecone as a vector database for efficient semantic search.

Features

PDF Loading: Automatically loads and parses all PDFs from a specified directory.

Text Chunking: Splits documents into manageable chunks for better embedding and retrieval.

Embeddings: Supports both OpenAI and HuggingFace embedding models.

Vector Search: Stores and searches document embeddings in Pinecone.

Question Answering: Uses OpenAI LLMs to answer questions based on retrieved document chunks.


How it works

Load PDFs: All PDFs in the documents folder are loaded and parsed.

Chunk Text: Documents are split into overlapping chunks for context preservation.

Embed Chunks: Each chunk is embedded using OpenAI or HuggingFace models.

Store in Pinecone: Embeddings are stored in a Pinecone vector index.

Ask Questions: User queries are embedded and used to retrieve relevant chunks from Pinecone.

Generate Answers: Retrieved chunks are passed to an OpenAI LLM to generate a final answer.


Requirements
Python 3.8+
OpenAI API key
Pinecone API key and environment
See requirements.txt for all dependencies.
