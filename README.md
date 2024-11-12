# LangChain
I've created a comprehensive implementation of a RAG-based chatbot using LangChain. Here's a breakdown of the key components:

## Document Loading:
Supports PDF, CSV, and DOCX files
Uses appropriate loaders from LangChain community

## Text Splitting:
Uses RecursiveCharacterTextSplitter
Configurable chunk size and overlap
Default chunk size of 1000 with 200 overlap

## Embeddings:
Uses OpenAI's text-embedding-3-small model
Generates embeddings for document chunks

## Vectorstore:
Uses Pinecone as the vector database
Automatically creates index if it doesn't exist
Stores embeddings with metadata

## LCEL Chain:
Implements a Retrieval-Augmented Generation (RAG) chain
Uses ChatGPT (gpt-3.5-turbo) as the base model
Custom prompt template for answer generation
Includes context retrieval and answer generation

To use this chatbot, you'll need to:

## Install required packages:

pip install langchain langchain-openai pinecone-client python-docx pypdf

Set up your API keys:


OpenAI API key
Pinecone API key and environment
