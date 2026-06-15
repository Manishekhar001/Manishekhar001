<div align="center">

# Manishekhar
### AI Engineer · RAG Systems · Agentic Pipelines · AWS

*Building production-grade AI systems, not just tutorials.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chigullapally-manishekhar)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Manishekhar001)

</div>

---

## 👤 About Me

I'm a final-year **B.Tech AI student** at Neil Gogte Institute of Technology, Hyderabad (CGPA: 8.84 | Graduating 2027), focused on building **production-ready AI engineering systems** — not toy demos.

My work lives at the intersection of **RAG architecture**, **LLM orchestration**, and **cloud deployment**. I care about systems that actually run in production: with CI/CD, proper error handling, async design, and real evaluation pipelines.

---

## 📊 GitHub Stats

<div align="center">

![Manishekhar's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Manishekhar001&show_icons=true&theme=dark&hide_border=true&count_private=true&include_all_commits=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Manishekhar001&layout=compact&theme=dark&hide_border=true&langs_count=8)

</div>

---

## 🔨 Flagship Projects

### 🏗️ [IDOP](https://github.com/Manishekhar001/IDOP) — Intelligent Data Operations Platform
> Enterprise-grade data orchestration — NL-to-SQL · Document Mutations · CSRAG · **[Live API ↗](http://54.159.245.29/docs)**

My most complete system. A unified FastAPI + LangGraph platform routing any natural language query via a **5-path semantic router** (SQL / MUTATION / RAG / CHAT / HYBRID), backed by an **18-node LangGraph state machine**.

| Feature | What it does |
|---|---|
| **NL-to-SQL** | Vanna 2.0 → SQLValidator → LLM Judge → cryptographic approval gate → Supabase execution |
| **Document Mutations** | Excel/CSV upload → column mapping → business rule validation → LLM audit → all-or-nothing Postgres transaction |
| **CSRAG** | HyDE → hybrid BM25+dense (Qdrant) → Voyage AI reranking → CRAG relevance eval → Tavily web fallback → SRAG grounding loops |
| **Memory** | AsyncPostgresStore (LTM) + AsyncPostgresSaver (STM) with auto-summarization |
| **Multi-Level Cache** | Four Redis namespaces + local LRU fallback + S3 document chunk cache with SHA-256 dedup |

**Stack:** FastAPI · LangGraph · LangChain · Qdrant · Vanna 2.0 �� Voyage AI · Supabase · Redis · AWS EC2 · Docker · GitHub Actions · Opik

---

### 🪵 [log-classification-system](https://github.com/Manishekhar001/log-classification-system) — Multi-Strategy Log Classifier
> Regex → BERT + Logistic Regression → LLM (Groq) — ~99% accuracy · FastAPI · 10 categories

A production-grade tiered fallback pipeline for classifying system logs. Each strategy returns a `(label, confidence)` tuple; if one fails it gracefully falls through to the next.

- **Stage 1 — Regex:** Exact pattern match (conf=1.0) for deterministic categories (User Action, System Notification)
- **Stage 2 — BERT + LR:** Sentence Transformers (`all-MiniLM-L6-v2`) embeddings → Logistic Regression; trained on 1,903 logs across 7 categories; ~99% weighted accuracy
- **Stage 3 — LLM (Groq):** Reserved for LegacyCRM domain-specific logs; LRU-cached to minimize API calls
- **FastAPI server** — `/classify` and `/classify/batch` endpoints with Pydantic validation
- **CLI tool** — batch-classify CSV files with `target_label` + `confidence` columns output

**Stack:** Python · FastAPI · BERT · Sentence Transformers · scikit-learn · Pydantic

---

### 🔌 [Expense Tracker MCP](https://github.com/Manishekhar001/Expense_tracker_mcp) — Custom MCP Server *(FastMCP)*
> Model Context Protocol server · ReAct agent integration · Claude Desktop compatible

- SQLite-backed MCP tool server exposing financial tracking operations over the MCP protocol
- Connected to Claude Desktop and custom ReAct loops via `langchain-mcp-adapters`
- Demonstrates MCP server design pattern for production LLM tooling

**Stack:** FastMCP · LangChain · Python · SQLite

---

### Other Projects

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
