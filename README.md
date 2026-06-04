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
> Enterprise-grade data orchestration — NL-to-SQL · Document Mutations · CSRAG

My most ambitious and complete system. A unified FastAPI + LangGraph platform that routes any natural language query to the right AI-driven operation via a **5-path semantic router** (SQL / MUTATION / RAG / CHAT / HYBRID), backed by an **18-node LangGraph state machine**.

| Feature | What it does |
|---|---|
| **NL-to-SQL** | Vanna 2.0 → SQLValidator → LLM Judge → cryptographic approval gate → Supabase execution |
| **Document Mutations** | Excel/CSV upload → column mapping → business rule validation → LLM audit → all-or-nothing Postgres transaction |
| **CSRAG** | HyDE → hybrid BM25+dense search (Qdrant) → Voyage AI reranking → CRAG relevance eval → Tavily web fallback → SRAG grounding loops |
| **Memory** | AsyncPostgresStore (LTM) + AsyncPostgresSaver (STM) with auto-summarization |
| **Multi-Level Cache** | Four Redis namespaces + local LRU fallback + S3 document chunk cache with SHA-256 dedup |
| **Enterprise Security** | Cryptographic single-use approval tokens, CORS hardening, all-or-nothing transaction rollbacks, Opik observability |

**Stack:** FastAPI · LangGraph · LangChain · Qdrant · Vanna 2.0 · Voyage AI · OpenAI · Supabase · Redis · AWS EC2 · Docker · GitHub Actions · Opik

---

### 🧠 [CSRAG](https://github.com/Manishekhar001/CSRAG) — Corrective + Self-Reflective RAG with Memory
> Production FastAPI + LangGraph pipeline deployed on AWS EC2

The foundation for IDOP's RAG subsystem, built and deployed independently:

- **Corrective RAG (CRAG):** Evaluates retrieved documents for relevance before generation. Falls back to web search if retrieval quality is low.
- **Self-Reflective RAG (SRAG):** Uses reflection tokens to decide *when* to retrieve, *what* to retrieve, and *whether* the generated answer is grounded.
- **Dual Memory:** Long-term (Qdrant vector store) + short-term (conversation buffer) with a self-healing vector store mechanism.
- **Full CI/CD:** GitHub Actions pipeline with mocked lifespan for integration tests. Deployed to AWS EC2 via Docker.

**Stack:** FastAPI · LangGraph · LangChain · Qdrant Cloud · Groq API · AWS EC2 · Docker · GitHub Actions

---

### 📊 [BasicRAGProject](https://github.com/Manishekhar001/BasicRAGProject) — Industry-Grade RAG Baseline
> End-to-end RAG system with cloud deployment and full observability

- LCEL pipeline (LangChain Expression Language) for clean, composable retrieval chains
- **RAGAS evaluation** — automated faithfulness, answer relevancy, and context precision scoring
- **LangSmith tracing** — full observability into every chain step
- Deployed to AWS EC2 with GitHub Actions CI/CD and Docker Hub integration

**Stack:** FastAPI · LangChain LCEL · Qdrant Cloud · RAGAS · LangSmith · AWS EC2 · Docker

---

### 🗃️ [texttoSqlProject](https://github.com/Manishekhar001/texttoSqlProject) — Text-to-SQL + RAG Hybrid System
> Natural language query router with dual answering strategies

- **RAG path** — retrieves from document store for unstructured knowledge queries
- **Text2SQL path** — generates and validates SQL for structured data queries
- LLM-as-Judge validation loop to ensure query correctness before execution

**Stack:** FastAPI · LangChain · Python · SQL

---

### 🔌 [Expense Tracker MCP](https://github.com/Manishekhar001/Expense_tracker_mcp) — Custom MCP Servers *(FastMCP)*
> Model Context Protocol servers for tool-augmented LLM workflows

- **Expense Tracker MCP** — SQLite-backed tool server for financial tracking
- Connected to Claude Desktop and custom ReAct agent loops via `langchain-mcp-adapters`

**Stack:** FastMCP · LangChain · Python · SQLite

---

### Other Projects

| Project | Description |
|---|---|
| [invoice-ocr-backend](https://github.com/Manishekhar001/invoice-ocr-backend) | Backend API for extracting structured data from invoice images using OCR |
| [n8n_personal_project](https://github.com/Manishekhar001/n8n_personal_project) | Personal note-taking and task manager built with n8n workflow automation |
| [Expense_tracker_using_claude_code](https://github.com/Manishekhar001/Expense_tracker_using_claude_code) | Full-stack expense tracking web app built with Claude Code |
| [Corrective-SelfRef-RAG-langchain-](https://github.com/Manishekhar001/Corrective-SelfRef-RAG-langchain-) | Earlier Corrective + Self-Reflective RAG implementation (predecessor to CSRAG) |
| [ANN_Classification](https://github.com/Manishekhar001/ANN_Classification) | ANN classifier using TensorFlow/Keras |
| [ANN_Regression](https://github.com/Manishekhar001/ANN_Regression) | ANN regression model using TensorFlow/Keras |
| [imdb_sentiment_analysis](https://github.com/Manishekhar001/imdb_sentiment_analysis) | Sentiment analysis on IMDB reviews using deep learning |

---

## 🧰 Tech Stack

**AI / ML**
`LangChain` `LangGraph` `LangSmith` `RAGAS` `Qdrant` `FastMCP` `Groq API` `OpenAI` `Voyage AI` `Vanna 2.0` `Opik`

**RAG Techniques**
`CRAG` `SRAG` `HyDE` `Hybrid Search (BM25 + Dense)` `RRF` `ColBERT` `Cross-Encoder Reranking` `FAISS IVF`

**Backend & Data**
`FastAPI` `Python` `SQL` `Supabase` `PostgreSQL` `Redis` `SQLite`

**Cloud & DevOps**
`AWS EC2` `AWS S3` `Docker` `Docker Hub` `GitHub Actions (CI/CD)`

**Automation**
`n8n`

---

## 📚 What I'm Currently Building / Studying

- 📖 **Agentic systems from scratch** — ReAct loops, LiteLLM, tool schema design
- 📖 **Advanced RAG theory** — ColBERT MaxSim, SPLADE inverted index, FAISS IVF nprobe tradeoffs

---

<div align="center">

*Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.*

</div>
