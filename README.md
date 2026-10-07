<div align="center">

# Manishekhar
### AI Engineer · RAG Systems · Agentic Pipelines · AWS

*Building production-grade AI systems, not just tutorials.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chigullapally-manishekhar)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Manishekhar001)
[![Interactive Portfolio](https://img.shields.io/badge/Interactive_Portfolio-3b82f6?style=for-the-badge&logo=About.me&logoColor=white)](https://manishekhar001.github.io/)

</div>

---

## 👤 About Me

I'm a final-year **B.E AI student** at Neil Gogte Institute of Technology, Hyderabad (CGPA: 8.84 | Graduating 2027), focused on building **production-ready AI engineering systems** — not toy demos.

My work lives at the intersection of **RAG architecture**, **LLM orchestration**, and **cloud deployment**. I care about systems that actually run in production: with CI/CD, proper error handling, async design, and real evaluation pipelines.

---

## 🚀 Featured Projects

> Three systems that define my engineering approach.

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

### 📦 PO Generation Engine

<div align="left">

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/Manishekhar001/PurchaseOrderCreation)
[![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)](https://github.com/Manishekhar001/PurchaseOrderCreation)
[![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)](https://github.com/Manishekhar001/PurchaseOrderCreation)

</div>

> Rule-based purchase order generation for a retail grocery store · Posible POS exports in, per-vendor PO files out

A **Python CLI engine** that reads sales, purchase, returns and stock exports from the store's POS and works out which products need reordering and how much. The logic is deliberately explainable: no ML, and every flag carries an action a buyer can check.

| Component | What it does |
|---|---|
| **Reorder rule** | Reorder when stock < velocity × vendor reorder cycle × 1.2 safety factor; quantity capped at 1.5× the SKU's historical average |
| **Vendor and cycle discovery** | Primary vendor per SKU from 180-day purchase history; reorder cycle = median gap between a vendor's PO dates |
| **3-tier flags** | Critical / Warning / Info with prescriptive actions; expired stock is never ordered, dormant items capped at 50% |
| **Pending-order tracking** | Open orders suppress duplicate suggestions; closed when receipt is detected, expired, or manually cleared |
| **Outputs** | Per-vendor CSV for POS upload and Excel for human review |

- Reorder logic is pure computation with no I/O, which keeps it unit-testable in isolation
- `pytest` suite covering reorder logic, pending-order lifecycle and data loading
- Documented limitations: no backtest yet, no seasonality, vendor-level cycles

**Stack:** `Python` `pandas` `openpyxl` `pytest`

**→ [View Repository](https://github.com/Manishekhar001/PurchaseOrderCreation)**

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
`FastAPI` `Python` `SQL` `pandas` `Supabase` `PostgreSQL` `Redis` `SQLite`

**Cloud & DevOps**
`AWS EC2` `AWS S3` `Docker` `GitHub Actions (CI/CD)`

---

<div align="center">

*Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.*

</div>
