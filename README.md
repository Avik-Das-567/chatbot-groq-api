# Chatbot Groq API - Data Analysis Assistant
---
### Open in Colab : https://colab.research.google.com/drive/1ldJH-h_yGU1itJUbYYSrERq7JQ-E1lL4?usp=sharing
---
## Overview
This project is an interactive AI-powered chatbot that helps explore and analyze a Netflix dataset. It uses the Groq large language model API and vector search with FAISS to perform retrieval-augmented generation (RAG), enabling smart and context-aware answers about the data.

---
## Features
- **Data upload & chunking:** Loads and splits large CSV datasets into manageable chunks for analysis.
- **Semantic search:** Uses embeddings from a sentence transformer model to retrieve relevant chunks of data based on user queries.
- **Conversational analysis:** Integrates with Groq’s LLM to generate detailed answers and insights in response to questions.
- **Automated insights:** Generates statistical summaries and trends from the dataset without manual prompting.
---
## How It Works
- **Dataset loading:** Reads a CSV file containing Netflix titles, including metadata like type, title, director, cast, release year, rating, and description.
- **Chunk creation:** Splits the dataset into smaller JSON chunks for efficient retrieval.
- **Embedding generation:** Converts text chunks into numerical embeddings using a pretrained transformer.
- **Vector indexing:** Stores embeddings in a FAISS index to enable quick similarity search.
- **Question answering:** Retrieves the most relevant data chunks and sends them to the Groq LLM to generate natural language answers.
- **Insight generation:** Automatically summarizes dataset characteristics and extracts trends.
---
## Tech Stack
- **Groq API:** For generating human-like responses.
- **FAISS:** For fast similarity search across large datasets.
- **SentenceTransformers:** To convert text into embeddings.
- **Pandas & NumPy:** For data manipulation and processing.
---
## Project Structure
- Jupyter Notebook / Colab file containing:
  - Data preprocessing logic
  - Embedding and vector index creation
  - Functions to retrieve relevant chunks and generate answers
  - A conversational loop for interactive Q&A

- CSV dataset (Netflix titles) for analysis.
---
## What You Can Do
- Ask questions about shows, movies, and dataset statistics.
- Discover trends, outliers, and summary statistics.
- Explore the dataset interactively, using natural language instead of manual filtering.
---
## Requirements
- Python environment (e.g., Google Colab)
- Access to the Groq API (requires API key)
---
## Usage Highlights
- Load a dataset and create embeddings.
- Ask questions about data (e.g., longest duration, earliest added show).
- Generate automated insights about distribution, release years, and other trends.
---
