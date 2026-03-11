# Overview

In Week 3, the AI Study Assistant was upgraded with **AI memory using a vector database**.

This technique is called **Retrieval-Augmented Generation (RAG)**.

Instead of sending the entire PDF to the LLM, the system retrieves **only the most relevant context** before generating quiz questions.

This makes the system more **efficient, scalable, and accurate** for large study materials.

---

# System Workflow

PDF

↓

Text Extraction

↓

Text Chunking

↓

Vector Database

↓

Relevant Context Retrieval

↓

LLM Generates Quiz

---

# Technologies Used

- Python
  
- Groq API (LLaMA 3.1)
  
- PyPDF2
  
- LangChain
  
- Sentence Transformers
  
- ChromaDB

---

# Project Structure

week3-ai-agent/

│

├── quiz_generator.py

├── pdf_reader.py

├── rag_pipeline.py

├── requirements.txt

└── README.md


---

# Implementation Steps

## 1 Install Libraries

pip install groq
pip install PyPDF2
pip install chromadb
pip install sentence-transformers
pip install langchain-community
pip install langchain-text-splitters


---

## 2 Connect to LLM (Groq)

The system uses **Groq LLaMA 3.1 Instant** model to generate quizzes.

📷 Screenshot: *Groq API connection*

---

## 3 Extract Text from PDF

The uploaded PDF is processed using **PyPDF2** and the text is extracted from each page.

📷 Screenshot: *PDF upload and extracted text*

---

## 4 Text Chunking

Large text is split into smaller segments using:

Configuration:

- chunk_size = 1000
- chunk_overlap = 200

📷 Screenshot: *Chunk creation output*

---

## 5 Create Vector Database

Chunks are converted into **vector embeddings** using:


They are stored inside **ChromaDB**.

📷 Screenshot: *Vector database creation*

---

## 6 Context Retrieval

The system searches the vector database for the most relevant chunk based on a query.

Example query:

📷 Screenshot: *Retrieved context*

---

## 7 Quiz Generation using RAG

The retrieved context is passed to the LLM which generates **multiple-choice questions**.

📷 Screenshot: *Generated quiz output*

---

# Example Output

Question 1:
What is Machine Learning?

A) A programming language
B) A branch of AI that learns from data
C) A database system
D) A hardware device

Correct Answer: B


---

# Key Concepts Learned

- Retrieval-Augmented Generation (RAG)
- Vector Databases
- Embeddings
- Context Retrieval
- LLM Integration

---


