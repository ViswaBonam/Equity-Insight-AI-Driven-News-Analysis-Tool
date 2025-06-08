# Equity-Insight-AI-Driven-News-Analysis-Tool

This project is an **end-to-end Retrieval-Augmented Generation (RAG) AI system** designed for equity research analysts. It allows users to input multiple financial news article URLs and then **ask natural language questions** about those articles — receiving accurate answers backed by specific sources.

> **Built with:** LangChain, OpenAI, FAISS, and Streamlit  
> **Inspired by:** Real-world financial workflows and equity research teams in mutual funds and investment banks.

---

## 🔍 Use Case

Equity research analysts read dozens of articles daily from sources like Economic Times, Bloomberg, or Moneycontrol. This tool automates that process:

- ✅ Ingests financial news via URLs  
- ✅ Splits, embeds, and stores them in a vector store (FAISS)  
- ✅ Allows natural language Q&A  
- ✅ Retrieves and references specific articles as sources

This is a **realistic, scalable prototype** ideal for financial institutions such as Jefferies or HDFC Mutual Fund.

---

## 📸 Demo

![screenshot](equityinsights.png)

---

## 🧠 Architecture

- **LangChain**: Document loaders, splitters, retrievers, chains
- **OpenAI**: Embedding & answer generation via `gpt-3.5-turbo`
- **FAISS**: Lightweight in-memory vector store for fast retrieval
- **Streamlit**: Intuitive UI to load articles and ask questions

### Long-Term Architecture (for production)

- Web scraper (e.g. BrightData, Playwright, or Python native)
- Scheduled ingestion and embedding
- Scalable vector DB (e.g. Pinecone, Weaviate, Chroma)
- Frontend chatbot (React + Flask backend)

---

## 🛠 Features

| Feature                            | Description                                                  |
|------------------------------------|--------------------------------------------------------------|
| 🔗 Article URL ingestion           | Load text from live news URLs                                |
| 🧱 Text chunking with overlap      | Ensures context-aware LLM input                              |
| 🧬 Semantic search via embeddings  | Efficient retrieval using vector similarity (FAISS)          |
| 🗣️ Ask natural language questions  | Get answers grounded in real news articles                   |
| 🔍 Source attribution              | View exact article links used in each answer                 |
| 🧪 Notebook walk-throughs          | Modular Jupyter notebooks for each core component            |
