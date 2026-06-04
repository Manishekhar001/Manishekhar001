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

Currently building **IDOP** — an Intelligent Data Operations Platform with multi-modal query routing (RAG + Text2SQL + document mutation), targeting production deployment in mid-2026.

---

## 📊 GitHub Stats

<div align="center">

![Manishekhar's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Manishekhar001&show_icons=true&theme=dark&hide_border=true&count_private=true&include_all_commits=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Manishekhar001&layout=compact&theme=dark&hide_border=true&langs_count=8)

</div>

---

## 🔨 Flagship Projects

### 🧠 [CSRAG](https://github.com/Manishekhar001/CSRAG) — Corrective + Self-Reflective RAG with Memory
> Production FastAPI + LangGraph pipeline deployed on AWS EC2

The most complete RAG system I've built. Goes well beyond naive retrieval:

- **Corrective RAG (CRAG):** Evaluates retrieved documents for relevance before generation. Falls back to web search if retrieval quality is low.
- **Self-Reflective RAG (SRAG):** Uses reflection tokens to decide *when* to retrieve, *what* to retrieve, and *whether* the generated answer is grounded.
- **Dual Memory:** Long-term (vector store via Qdrant) + short-term (conversation buffer) memory with a self-healing vector store mechanism.
- **Full CI/CD:** GitHub Actions pipeline with mocked lifespan for integration tests. Deployed to AWS EC2 via Docker.
- **Architectural highlights:** `decide_retrieval_node` with concrete few-shot examples; `generate_direct` path routed through `verify_usefulness` for automatic fallback; async-safe throughout.

**Stack:** FastAPI · LangGraph · LangChain · Qdrant Cloud · Groq API · AWS EC2 · Docker · GitHub Actions

---

### 📊 [BasicRAGProject](https://github.com/Manishekhar001/BasicRAGProject) — Industry-Grade RAG Baseline
> End-to-end RAG system with cloud deployment and full observability

Built to production standards from day one — not a notebook, a real deployable service.

- LCEL pipeline (LangChain Expression Language) for clean, composable retrieval chains
- **RAGAS evaluation** — automated faithfulness, answer relevancy, and context precision scoring
- **LangSmith tracing** — full observability into every chain step
- Deployed to AWS EC2 with GitHub Actions CI/CD and Docker Hub integration

**Stack:** FastAPI · LangChain LCEL · Qdrant Cloud · RAGAS · LangSmith · AWS EC2 · Docker

---

### 🗃️ [texttoSqlProject](https://github.com/Manishekhar001/texttoSqlProject) — Text-to-SQL + RAG Hybrid System
> Natural language query router with dual answering strategies

Routes natural language questions to the right engine automatically:
- **RAG path** — retrieves from document store for unstructured knowledge queries
- **Text2SQL path** — generates and validates SQL for structured data queries
- LLM-as-Judge validation loop to ensure query correctness before execution

**Stack:** FastAPI · LangChain · Python · SQL

---

### 🏗️ [IDOP](https://github.com/Manishekhar001/IDOP) — Intelligent Data Operations Platform *(In Development)*
> 32-node LangGraph multi-agent system for enterprise data operations

My most ambitious project. A unified platform that routes natural language queries to the right operation:

| Feature | What it does |
|---|---|
| **Feature 1 — Text2SQL** | Converts natural language to SQL with LLM-as-Judge validation loop |
| **Feature 2 — Doc Mutation** | Handles document insert/update/delete with audit logging |
| **Feature 3 — RAG** | Hybrid BM25 + dense retrieval, reranking, RAGAS evaluation (~70% carried over from CSRAG) |
| **HYBRID Merge** | Top-level router that dispatches queries to the right subgraph |

Planned: ColBERT late-interaction reranking · RRF score fusion · SPLADE sparse retrieval

**Stack:** FastAPI · LangGraph · LangChain · Qdrant · AWS EC2 · Docker · GitHub Actions

---

### 🔌 [Expense Tracker MCP](https://github.com/Manishekhar001/Expense_tracker_mcp) — Custom MCP Servers *(FastMCP)*
> Model Context Protocol servers for tool-augmented LLM workflows

Built multiple MCP servers using **FastMCP** and integrated them with LangChain-based clients:
- **Expense Tracker MCP** — SQLite-backed tool server for financial tracking
- **Calculator MCP** — arithmetic tool server with schema-validated inputs
- Connected to Claude Desktop and custom ReAct agent loops via `langchain-mcp-adapters`

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
`LangChain` `LangGraph` `LangSmith` `RAGAS` `Qdrant` `FastMCP` `Groq API`

**RAG Techniques I've Implemented or Studied in Depth**
`CRAG` `SRAG` `Hybrid Search (BM25 + Dense)` `RRF` `ColBERT` `SPLADE` `Cross-Encoder Reranking` `FAISS IVF`

**Backend & APIs**
`FastAPI` `Python` `SQL (Intermediate–Professional)`

**Cloud & DevOps**
`AWS EC2` `Docker` `Docker Hub` `GitHub Actions (CI/CD)`

**Automation**
`n8n`

---

## 📚 What I'm Currently Building / Studying

- 🔨 **IDOP production build** — Text2SQL subgraph, RAGAS auto-eval, full deployment
- 📖 **Agentic systems from scratch** — ReAct loops, LiteLLM, tool schema design
- 📖 **Advanced RAG theory** — ColBERT MaxSim, SPLADE inverted index, FAISS IVF nprobe tradeoffs

---

<div align="center">

*Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.*

</div>
