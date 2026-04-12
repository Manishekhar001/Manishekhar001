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

Currently building **IDOP** — an Intelligent Data Operations Platform with multi-modal query routing (RAG + Text2SQL + document mutation), targeting production deployment in mid-2025.

---

## 🔨 Flagship Projects

### 🧠 CSRAG — Corrective + Self-Reflective RAG with Memory
> Production FastAPI + LangGraph pipeline deployed on AWS EC2

The most complete RAG system I've built. Goes well beyond naive retrieval:

- **Corrective RAG (CRAG):** Evaluates retrieved documents for relevance before generation. Falls back to web search if retrieval quality is low.
- **Self-Reflective RAG (SRAG):** Uses reflection tokens to decide *when* to retrieve, *what* to retrieve, and *whether* the generated answer is grounded.
- **Dual Memory:** Long-term (vector store via Qdrant) + short-term (conversation buffer) memory with a self-healing vector store mechanism.
- **Full CI/CD:** GitHub Actions pipeline with mocked lifespan for integration tests. Deployed to AWS EC2 via Docker.
- **Architectural highlights:** `decide_retrieval_node` with concrete few-shot examples; `generate_direct` path routed through `verify_usefulness` for automatic fallback; async-safe throughout.

**Stack:** FastAPI · LangGraph · LangChain · Qdrant Cloud · Groq API · AWS EC2 · Docker · GitHub Actions

---

### 📊 BasicRAGProject — Industry-Grade RAG Baseline
> End-to-end RAG system with cloud deployment and full observability

Built to production standards from day one — not a notebook, a real deployable service.

- LCEL pipeline (LangChain Expression Language) for clean, composable retrieval chains
- **RAGAS evaluation** — automated faithfulness, answer relevancy, and context precision scoring
- **LangSmith tracing** — full observability into every chain step
- Deployed to AWS EC2 with GitHub Actions CI/CD and Docker Hub integration

**Stack:** FastAPI · LangChain LCEL · Qdrant Cloud · RAGAS · LangSmith · AWS EC2 · Docker

---

### 🏗️ IDOP — Intelligent Data Operations Platform *(In Development)*
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

### 🔌 Custom MCP Servers *(FastMCP)*
> Model Context Protocol servers for tool-augmented LLM workflows

Built multiple MCP servers using **FastMCP** and integrated them with LangChain-based clients:
- **Expense Tracker MCP** — SQLite-backed tool server for financial tracking
- **Calculator MCP** — arithmetic tool server with schema-validated inputs
- Connected to Claude Desktop and custom ReAct agent loops via `langchain-mcp-adapters`

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
---

<div align="center">

*Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.*

</div>
