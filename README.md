# tenXengage RAG Chatbot Prototype

**AI Engineer Intern | tenXengage | June–August 2025**

## Source Code

The source code is not publicly available, as this project was developed during a company internship and permission for public sharing has not been confirmed. This repository documents my technical implementation and contributions.

## Project Overview

During my AI engineering internship at tenXengage, I developed a prototype of an AI-powered product support chatbot using Retrieval-Augmented Generation (RAG).

The chatbot was designed to answer product-specific questions by retrieving relevant information from a knowledge base and using a large language model (LLM) to generate responses. The prototype was developed and evaluated to support over 100 product-related questions.

My prototype subsequently served as a basis for a similar chatbot developed further by company employees and made available on the tenXengage website.

**Company Website:** [tenXengage](https://tenxengage.com/)

## Technical Implementation

**Technologies:** Python, Flask, LangChain, FAISS, OpenAI API (GPT-4o-mini), React, JavaScript, HTML, CSS

The chatbot consists of two main components:

### 1. Backend

- Developed a Python Flask backend to handle chatbot requests.
- Used LangChain document loaders to process product information stored in TXT, PDF, and DOCX files.
- Split product knowledge base documents into smaller, overlapping text chunks using LangChain's `RecursiveCharacterTextSplitter`.
- Generated vector embeddings using OpenAI's embedding model through LangChain's `OpenAIEmbeddings`.
- Built a FAISS vector index using LangChain's FAISS integration to support similarity-based retrieval of relevant product information.
- Retrieved the three most relevant document chunks for each user question using LangChain's `similarity_search()` method.
- Used the OpenAI API to send retrieved product information and the user's question to GPT-4o-mini, which generated a response using the provided context.
- Implemented a Flask API endpoint to connect the backend with the frontend.

### 2. Frontend

- Developed a web-based chatbot interface using React, JavaScript, HTML, and CSS.
- Integrated the `react-chat-widget` library to allow users to submit questions and receive responses.
- Connected the React frontend to the Flask backend through HTTP POST requests.

## Prototype Screenshots

The screenshots in this repository show the original chatbot prototype I developed during my internship, including its user interface and examples of product-related responses.
