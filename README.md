# 📚 Interactive Textbook Q&A using Hybrid RAG

An AI-powered **Interactive Textbook Question Answering System** built using **LangChain**, **Hybrid Retrieval (BM25 + ChromaDB)**, and **OpenRouter LLMs**. The system allows students to upload textbooks and ask natural language questions while receiving context-grounded answers with source citations.

---

## 🚀 Features

✅ Hybrid Retrieval (Semantic Search + BM25 Keyword Search)

✅ Persistent ChromaDB Vector Database

✅ Incremental PDF Indexing (Add new textbooks without rebuilding)

✅ Multi-Document Question Answering

✅ File & Page Number Citations

✅ Source-Grounded Responses

✅ RAG Evaluation using Ragas

---

## 🛠️ Tech Stack

- 🐍 Python
- 🦜 LangChain
- 🗂️ ChromaDB
- 🔍 BM25 Retriever
- 🤖 OpenRouter API
- 💎 Google Gemini 2.5 Flash
- 📄 PyPDF
- 📊 Ragas Evaluation Framework

---

## ⚙️ Pipeline

```text
PDF Textbooks
      │
      ▼
Document Loading
      │
      ▼
Recursive Character Text Splitter
      │
      ▼
OpenAI Embeddings (OpenRouter)
      │
      ▼
Persistent ChromaDB
      │
      ▼
Hybrid Retrieval
(BM25 + Semantic Search)
      │
      ▼
LangChain Retrieval Chain
      │
      ▼
Gemini 2.5 Flash (OpenRouter)
      │
      ▼
Answer + File/Page Citation
```

---

## 📈 RAG Evaluation

The retrieval pipeline was evaluated using the **Ragas** framework.

| Metric | Score |
|---------|-------|
| ✅ Faithfulness | **92.3%** |
| 📌 Response Relevancy | 74.2% |
| 🎯 Context Recall | 83.3% |
| 🔍 Context Precision | 38.0% |

**Evaluation Framework:** Ragas

---

## 💡 Example

### Question

> What is photosynthesis and how does it occur in plants?

### Answer

> Photosynthesis is the process by which green plants prepare their own food using sunlight, carbon dioxide and water in the presence of chlorophyll. Oxygen is released as a by-product.

**📄 Source**

- Class7ScienceTextbook.pdf — Page 18

---

## 📂 Project Structure

```text
Interactive_TextBook/
│
├── InteractiveTextBook.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── textbooks/
```

---

## ▶️ Installation

```bash
pip install -r requirements.txt
```

---

## ⭐ Key Highlights

- Hybrid RAG Architecture
- Persistent Vector Database
- Incremental Document Indexing
- Citation-Based Answer Generation
- Automated RAG Evaluation using Ragas
- Multi-Document Support

---

## 📌 Future Improvements

- Conversational Memory
- Query Expansion
- Reranking Models
- OCR Support for Scanned PDFs
- Streamlit/Web Interface
- Support for DOCX & PPT Files

---

## 👨‍💻 Author

**Vighnesh Takke**

GitHub: https://github.com/vighi2004
