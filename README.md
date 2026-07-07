<div align="center">

# Manishekhar
### AI Engineer · RAG Systems · Agentic Pipelines · AWS

*Building production-grade AI systems, not just tutorials.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chigullapally-manishekhar)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Manishekhar001)

</div>

---

## 👤 About Me

I'm a final-year **B.E AI student** at Neil Gogte Institute of Technology, Hyderabad (CGPA: 8.84 | Graduating 2027), focused on building **production-ready AI engineering systems** — not toy demos.

My work lives at the intersection of **RAG architecture**, **LLM orchestration**, and **cloud deployment**. I care about systems that actually run in production: with CI/CD, proper error handling, async design, and real evaluation pipelines.

---

## 📊 GitHub Stats

<div align="center">

![Manishekhar's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Manishekhar001&show_icons=true&theme=dark&hide_border=true&count_private=true&include_all_commits=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Manishekhar001&layout=compact&theme=dark&hide_border=true&langs_count=8)

</div>

---

## 🚀 Featured Projects

> Three production-grade systems that define my engineering approach.

---

### 🏗️ IDOP — Intelligent Data Operations Platform

<div align="left">

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![LangGraph](https://img.shields.io/badge/LangGraph-FF6F00?style=flat-square&logo=python&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![Qdrant](https://img.shields.io/badge/Qdrant-DC143C?style=flat-square&logo=databricks&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![AWS](https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)](https://github.com/Manishekhar001/IDOP)
[![Live](https://img.shields.io/badge/Live%20API-%E2%86%97-brightgreen?style=flat-square)](http://54.159.245.29/docs)

</div>

> Enterprise-grade data orchestration — NL-to-SQL · Document Mutations · Advanced CSRAG

A unified **FastAPI + LangGraph** platform routing any natural language query through a **5-path semantic router** (SQL / MUTATION / RAG / CHAT / HYBRID), backed by an **18-node LangGraph state machine**.

| Capability | Implementation |
|---|---|
| **NL-to-SQL** | Vanna 2.0 → SQLValidator → LLM Judge → cryptographic approval gate → Supabase |
| **Document Mutations** | Excel/CSV → column mapping → business rule validation → LLM audit → atomic Postgres transaction |
| **CSRAG** | HyDE → hybrid BM25+dense (Qdrant) → Voyage AI reranking → CRAG eval → Tavily fallback → SRAG loops |
| **Memory** | AsyncPostgresStore (LTM) + AsyncPostgresSaver (STM) with auto-summarization |
| **Cache** | 4 Redis namespaces + local LRU + S3 chunk cache with SHA-256 dedup |

**Full Stack:** `FastAPI` `LangGraph` `LangChain` `Qdrant` `Vanna 2.0` `Voyage AI` `Supabase` `Redis` `AWS EC2` `Docker` `GitHub Actions` `Opik`

---

### 🪵 Log Classification System

<div align="left">

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://github.com/Manishekhar001/log-classification-system)
[![BERT](https://img.shields.io/badge/BERT-FFD700?style=flat-square&logo=python&logoColor=black)](https://github.com/Manishekhar001/log-classification-system)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)](https://github.com/Manishekhar001/log-classification-system)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/Manishekhar001/log-classification-system)
[![Accuracy](https://img.shields.io/badge/Accuracy-~99%25-success?style=flat-square)](https://github.com/Manishekhar001/log-classification-system)

</div>

> Multi-strategy tiered pipeline — Regex → BERT → LLM · ~99% accuracy · 10 categories · 2,410 logs

A **production-grade fallback pipeline** for system log classification. Each stage returns a `(label, confidence)` tuple and hands off to the next only when confidence is insufficient.

| Stage | Strategy | Coverage |
|---|---|---|
| **Stage 1** | Regex exact-match (conf = 1.0) | User Actions, System Notifications |
| **Stage 2** | BERT (`all-MiniLM-L6-v2`) + Logistic Regression | 7 categories, ~99% weighted F1 |
| **Stage 3** | LLM via Groq (LRU-cached) | LegacyCRM domain-specific logs |

- `/classify` and `/classify/batch` FastAPI endpoints with full Pydantic validation
- CLI tool for batch CSV classification with `target_label` + `confidence` output columns
- Pre-trained models included — no re-training needed to run

**Stack:** `Python` `FastAPI` `BERT` `Sentence Transformers` `scikit-learn` `Pydantic`

**→ [View Repository](https://github.com/Manishekhar001/log-classification-system)**

---

### 🔌 Expense Tracker MCP

<div align="left">

[![FastMCP](https://img.shields.io/badge/FastMCP-6A0DAD?style=flat-square&logo=python&logoColor=white)](https://github.com/Manishekhar001/Expense_tracker_mcp)
[![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white)](https://github.com/Manishekhar001/Expense_tracker_mcp)
[![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)](https://github.com/Manishekhar001/Expense_tracker_mcp)
[![MCP](https://img.shields.io/badge/Claude%20Desktop-Compatible-blueviolet?style=flat-square)](https://github.com/Manishekhar001/Expense_tracker_mcp)

</div>

> Custom MCP server built with FastMCP · Claude Desktop compatible · ReAct agent integration

A **Model Context Protocol (MCP) tool server** that exposes financial tracking operations to any MCP-compatible client. Demonstrates how to build structured, schema-driven tool APIs for LLMs.

- **4 tools:** `add_expense`, `list_expenses`, `summarize`, `delete_expense` — all with typed schemas auto-generated from Python type hints
- **1 resource:** `expense:///categories` — lets the LLM query available categories before acting
- Connected to **Claude Desktop** and custom **ReAct loops** via `langchain-mcp-adapters`
- SQLite persistence with `aiosqlite` for async, non-blocking I/O

**Stack:** `FastMCP` `LangChain` `Python` `SQLite` `aiosqlite`

**→ [View Repository](https://github.com/Manishekhar001/Expense_tracker_mcp)**

---

## 📁 Other Projects

| Project | Description |
|---|---|
| [mini-p](https://github.com/Manishekhar001/mini-p) | Streamlit RAG chatbot with LLM judge — LangGraph routing between document context and general knowledge, FAISS + Nomic embeddings, SQLite persistence, streaming responses |
| [Corrective-SelfRef-RAG-langchain-](https://github.com/Manishekhar001/Corrective-SelfRef-RAG-langchain-) | Corrective + Self-Reflective RAG with dual memory — foundation for IDOP's RAG subsystem |
| [BasicRAGProject](https://github.com/Manishekhar001/BasicRAGProject) | Industry-grade RAG with RAGAS evaluation, LangSmith tracing, AWS EC2 deployment |
| [texttoSqlProject](https://github.com/Manishekhar001/texttoSqlProject) | NL-to-SQL + RAG hybrid router — foundation for IDOP's SQL subsystem |
| [invoice-ocr-backend](https://github.com/Manishekhar001/invoice-ocr-backend) | Backend API for structured data extraction from invoice images |
| [ANN_Classification](https://github.com/Manishekhar001/ANN_Classification) | ANN classifier using TensorFlow/Keras |
| [imdb_sentiment_analysis](https://github.com/Manishekhar001/imdb_sentiment_analysis) | Sentiment analysis on IMDB reviews using deep learning |

---

## 🧰 Tech Stack

**AI / ML**
`LangChain` `LangGraph` `LangSmith` `RAGAS` `Qdrant` `FastMCP` `Voyage AI` `Vanna 2.0` `Opik` `BERT` `Sentence Transformers`

**RAG Techniques**
`CRAG` `SRAG` `HyDE` `Hybrid Search (BM25 + Dense)` `RRF` `ColBERT` `Cross-Encoder Reranking`

**Backend & Data**
`FastAPI` `Python` `SQL` `Supabase` `PostgreSQL` `Redis` `SQLite`

**Cloud & DevOps**
`AWS EC2` `AWS S3` `Docker` `GitHub Actions (CI/CD)`

---

## 📚 What I'm Currently Building / Studying

- 🔌 **Model Context Protocol (MCP)** — building production tool servers with FastMCP, integrating MCP into custom ReAct/LangGraph pipelines
- 📖 **Advanced RAG theory** — ColBERT MaxSim, SPLADE inverted index, cross-encoder reranking pipelines

---

<div align="center">

*Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.*

</div> 
