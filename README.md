# Semantic Search Engine with LangChain, Pinecone, and Hugging Face

This project implements a **Semantic Search Engine** using **LangChain**, **Pinecone**, and **Hugging Face Embeddings**. It allows users to perform semantic searches on product and service data, providing context-aware results using advanced machine learning models.

## Table of Contents
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Environment Variables](#environment-variables)
- [Project Structure](#project-structure)
- [Data Used](#data-used)
- [How It Works](#how-it-works)
- [Logging](#logging)

---

## Features
- **Semantic Search**: Finds relevant products and services based on natural language queries.
- **Conversational QA**: Uses a pre-trained language model to answer queries contextually.
- **Vector Indexing**: Efficient search and retrieval using Pinecone.
- **Dynamic Document Creation**: Converts product and service data into document objects for indexing.

---

## Technology Stack
- **Python**
- **LangChain**
- **Pinecone**
- **Hugging Face Embeddings**
- **ChatGroq**
- **dotenv** (for environment variable management)
- **pandas** (for data handling)

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/semantic-search-engine.git
   cd semantic-search-engine
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Linux/Mac
   venv\Scripts\activate    # On Windows
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
1. **Set up your `.env` file** with the required API keys (see [Environment Variables](#environment-variables)).

2. **Run the Jupyter Notebook** to initialize the embeddings and Pinecone index:
   ```bash
   jupyter notebook SearchEngine_Pinecone.ipynb
   ```

3. **Use the semantic search functions** to perform searches on the product and service data.

---

## Environment Variables
Create a `.env` file in the project root directory and add the following variables:
```env
GROQ_API_KEY=your_chatgroq_api_key
PINECONE_KEY=your_pinecone_api_key
PINECONE_ENV=your_pinecone_environment
```
Replace the values with your actual API keys.

---

## Project Structure
```
semantic-search-engine/
├── SearchEngine_Pinecone.ipynb
├── requirements.txt
├── .env
└── README.md
```

---

## Data Used
The project includes example data for products and services:
- **Products**: Contains product IDs, names, descriptions, gender, and base color.
- **Services**: Contains service IDs, names, descriptions, and categories.

---

## How It Works
### 1. **Loading Environment Variables**
The `.env` file is used to securely manage API keys for Pinecone and ChatGroq.

### 2. **Initializing Hugging Face Embeddings**
A fine-tuned SentenceTransformer model is used to generate embeddings for queries and documents.

### 3. **Creating Documents**
Products and services are converted into document objects that can be indexed in Pinecone.

### 4. **Indexing in Pinecone**
The documents are indexed in Pinecone for fast and efficient retrieval.

### 5. **Querying with LangChain**
Queries are processed using LangChain to provide context-aware responses from the indexed data.

---

## Logging
The project logs important events and errors to `semantic_search.log`.
```
2025-01-07 10:00:00 - INFO - HuggingFaceEmbeddings initialized with model: models/fine-tuned-sbert-triplet
2025-01-07 10:05:00 - INFO - ChatGroq LLM initialized successfully.
```

