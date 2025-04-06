# 🔍 Semantic Search & Recommendation Engine

This repository contains a comprehensive **Semantic Search and Recommendation Engine** built entirely within a single **Jupyter Notebook**. It integrates advanced techniques including embeddings, vector stores, and Retrieval-Augmented Generation (RAG) to dynamically retrieve relevant products and services.

---

## 🚀 Key Features

- **Semantic Search**: Powered by fine-tuned Sentence-BERT embeddings for precise context-aware matching.
- **Vector Database (Pinecone)**: Efficient storage and fast retrieval of embeddings for similarity search.
- **Retrieval-Augmented Generation (RAG)**: Utilizes LangChain and ChatGroq (LLaMA3) to provide coherent and contextually accurate recommendations.
- **Dynamic Query Handling**: Includes metadata-based filtering (e.g., product or service, gender, category).
- **Natural Language Processing (spaCy)**: Contextual extraction and filtering based on query content.

---

## 📂 Project Structure

- **Single Jupyter Notebook**: End-to-end implementation covering data ingestion, preprocessing, embedding creation, semantic search, and RAG-powered recommendations.

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **LangChain**
- **ChatGroq (LLaMA3)**
- **HuggingFace Embeddings (Sentence-BERT)**
- **Pinecone Vector Store**
- **spaCy**

---

## 🚦 How to Run

1. **Setup Environment**:
   ```bash
   pip install -r requirements.txt
   ```

2. **Configure API Keys**:
   - Create a `.env` file with your `GROQ_API_KEY` and `PINECONE_KEY`.

3. **Run Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

---

## 📖 Example Queries

- "Show me men's blue jeans"
- "I need painting services"
- "Find women's jeans"
- "Recommend a product"
- "I need automotive services"

---

## 🎯 Use Case

Ideal for e-commerce platforms, knowledge bases, and recommendation systems where accurate semantic retrieval and personalized recommendations are critical.

---

## 🤝 Contributing

Feel free to fork, modify, and enhance this project. Contributions are always welcome!

---

## 📜 License

Distributed under the MIT License.

