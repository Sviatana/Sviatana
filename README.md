# Svetlana Sidorenko

**AI Engineer · Python Backend Engineer · LLM Applications**

I build production-oriented AI applications and Python backend systems. My current focus is on LLM integrations, retrieval-augmented generation, structured AI outputs, API orchestration, validation, and reliable backend architecture.

I work across the full delivery cycle: requirements, architecture, implementation, testing, production debugging, Docker-based release preparation, and ongoing improvement.

---

## Core Stack

### Backend

- Python 3.12
- FastAPI
- AsyncIO
- REST APIs
- Pydantic 2
- SQLAlchemy 2
- Alembic

### AI / LLM

- OpenAI-compatible APIs
- RAG pipelines
- Embeddings
- Semantic and vector search
- Structured outputs
- Context assembly
- Validation, retry, repair, and fallback flows

### Data

- PostgreSQL
- pgvector
- SQLite
- Redis

### Infrastructure

- Docker
- Docker Compose
- Git and GitHub
- Linux
- Railway
- GitHub Actions

---

## Featured Projects

### Stock Keyworder

AI-assisted metadata generation for stock photography.

The service accepts uploaded images, normalizes them, sends them to a vision-capable OpenAI model, validates structured metadata, stores results, supports batch processing, editing, history, and CSV export.

**Highlights**

- Fully async FastAPI and SQLAlchemy 2 backend
- PostgreSQL in production and SQLite locally
- Pydantic validation for AI responses
- Bounded retries with exponential backoff and jitter
- Google OAuth
- Alembic migrations
- Batch workflow and secure user-scoped access

**Stack:** Python 3.12, FastAPI, SQLAlchemy 2, PostgreSQL, Pydantic 2, httpx, OpenAI API, Alembic, Docker

**Repository:** [github.com/Sviatana/stock-keyworder](https://github.com/Sviatana/stock-keyworder)

---

### ContextFlow

Backend service demonstrating a controlled retrieval-augmented generation pipeline.

The service accepts a user question, retrieves relevant context from an in-memory knowledge base using embeddings and cosine similarity, sends the selected context to an OpenAI-compatible model, validates the answer, and returns structured JSON.

**Highlights**

- Clear separation of retrieval, generation, and validation
- Embeddings-based semantic search
- Controlled prompt construction
- Response validation before returning output
- Simple, maintainable FastAPI architecture

**Stack:** Python, FastAPI, Pydantic, OpenAI-compatible API, embeddings, cosine similarity

**Repository:** [github.com/Sviatana/ContextFlow](https://github.com/Sviatana/ContextFlow)

---

### Anima

Production-style FastAPI backend template for API-driven services, AI assistants, and voice-enabled systems.

The repository demonstrates modular backend architecture, asynchronous request handling, PostgreSQL integration, environment-based configuration, CI, and deployment-ready setup.

**Highlights**

- Separation of API, core logic, and database layers
- Async request handling
- PostgreSQL schema and migration structure
- Docker and Railway deployment setup
- GitHub Actions CI

**Stack:** Python, FastAPI, AsyncIO, PostgreSQL, SQLAlchemy, Docker, Railway, GitHub Actions

**Repository:** [github.com/Sviatana/anima](https://github.com/Sviatana/anima)

---

## Additional Experience

- AI assistants and business automation
- Telegram products and Mini Apps
- External API integrations
- Background processing
- File parsing and data validation
- Production logs and root-cause debugging
- Browser automation with Selenium and undetected-chromedriver

---

## How I Work

- Design systems with clear component boundaries
- Keep AI outputs controlled and validated
- Prefer root-cause analysis over one-off fixes
- Treat deployment and maintainability as part of development
- Use AI-assisted development tools while retaining responsibility for architecture, review, testing, and final code quality

---

## Contacts

- **Email:** ssidaren@gmail.com
- **Website:** [ai24solutions.ru](https://ai24solutions.ru)
- **LinkedIn:** [linkedin.com/in/sviatanasidarenka](https://www.linkedin.com/in/sviatanasidarenka/)
- **Telegram:** [t.me/sidarenkas](https://t.me/sidarenkas)
