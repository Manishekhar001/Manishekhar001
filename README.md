Manishekhar
AI Engineer · RAG Systems · Agentic Pipelines · AWS
Building production-grade AI systems, not just tutorials.

Interactive PortfolioLinkedInGitHub

👤 About Me
I'm a final-year B.E AI student at Neil Gogte Institute of Technology, Hyderabad (CGPA: 8.84 | Graduating 2027), focused on building production-ready AI engineering systems — not toy demos.

My work lives at the intersection of RAG architecture, LLM orchestration, and cloud deployment. I care about systems that actually run in production: with CI/CD, proper error handling, async design, and real evaluation pipelines.

📊 GitHub Stats
Manishekhar's GitHub Stats

Top Languages

🚀 Featured Projects
Three production-grade systems that define my engineering approach.

🏗️ IDOP — Intelligent Data Operations Platform
FastAPILangGraphQdrantRedisAWSSupabaseLive

Enterprise-grade data orchestration — NL-to-SQL · Document Mutations · Advanced CSRAG

A unified FastAPI + LangGraph platform routing any natural language query through a 5-path semantic router (SQL / MUTATION / RAG / CHAT / HYBRID), backed by an 18-node LangGraph state machine.

Capability	Implementation
NL-to-SQL	Vanna 2.0 → SQLValidator → LLM Judge → cryptographic approval gate → Supabase
Document Mutations	Excel/CSV → column mapping → business rule validation → LLM audit → atomic Postgres transaction
CSRAG	HyDE → hybrid BM25+dense (Qdrant) → Voyage AI reranking → CRAG eval → Tavily fallback → SRAG loops
Memory	AsyncPostgresStore (LTM) + AsyncPostgresSaver (STM) with auto-summarization
Cache	4 Redis namespaces + local LRU + S3 chunk cache with SHA-256 dedup
Full Stack: FastAPI LangGraph LangChain Qdrant Vanna 2.0 Voyage AI Supabase Redis AWS EC2 Docker GitHub Actions Opik

🪵 Log Classification System
FastAPIBERTscikit-learnPythonAccuracy

Multi-strategy tiered pipeline — Regex → BERT → LLM · ~99% accuracy · 10 categories · 2,410 logs

A production-grade fallback pipeline for system log classification. Each stage returns a (label, confidence) tuple and hands off to the next only when confidence is insufficient.

Stage	Strategy	Coverage
Stage 1	Regex exact-match (conf = 1.0)	User Actions, System Notifications
Stage 2	BERT (all-MiniLM-L6-v2) + Logistic Regression	7 categories, ~99% weighted F1
Stage 3	LLM via Groq (LRU-cached)	LegacyCRM domain-specific logs
/classify and /classify/batch FastAPI endpoints with full Pydantic validation
CLI tool for batch CSV classification with target_label + confidence output columns
Pre-trained models included — no re-training needed to run
Stack: Python FastAPI BERT Sentence Transformers scikit-learn Pydantic

→ View Repository

🔌 Expense Tracker MCP
FastMCPLangChainSQLiteMCP

Custom MCP server built with FastMCP · Claude Desktop compatible · ReAct agent integration

A Model Context Protocol (MCP) tool server that exposes financial tracking operations to any MCP-compatible client. Demonstrates how to build structured, schema-driven tool APIs for LLMs.

4 tools: add_expense, list_expenses, summarize, delete_expense — all with typed schemas auto-generated from Python type hints
1 resource: expense:///categories — lets the LLM query available categories before acting
Connected to Claude Desktop and custom ReAct loops via langchain-mcp-adapters
SQLite persistence with aiosqlite for async, non-blocking I/O
Stack: FastMCP LangChain Python SQLite aiosqlite

→ View Repository

📁 Other Projects
Project	Description
mini-p	Streamlit RAG chatbot with LLM judge — LangGraph routing between document context and general knowledge, FAISS + Nomic embeddings, SQLite persistence, streaming responses
Corrective-SelfRef-RAG-langchain-	Corrective + Self-Reflective RAG with dual memory — foundation for IDOP's RAG subsystem
BasicRAGProject	Industry-grade RAG with RAGAS evaluation, LangSmith tracing, AWS EC2 deployment
texttoSqlProject	NL-to-SQL + RAG hybrid router — foundation for IDOP's SQL subsystem
invoice-ocr-backend	Backend API for structured data extraction from invoice images
ANN_Classification	ANN classifier using TensorFlow/Keras
imdb_sentiment_analysis	Sentiment analysis on IMDB reviews using deep learning
🧰 Tech Stack
AI / MLLangChain LangGraph LangSmith RAGAS Qdrant FastMCP Voyage AI Vanna 2.0 Opik BERT Sentence Transformers

RAG TechniquesCRAG SRAG HyDE Hybrid Search (BM25 + Dense) RRF ColBERT Cross-Encoder Reranking

Backend & DataFastAPI Python SQL Supabase PostgreSQL Redis SQLite

Cloud & DevOpsAWS EC2 AWS S3 Docker GitHub Actions (CI/CD)

Open to AI/ML Engineering roles. If you're building something serious with LLMs, let's talk.
