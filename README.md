# Svetlana Sidorenko

**AI Engineer · Python Backend Engineer · LLM Applications**

I design and build AI-powered applications and production backend systems with Python.

My current work focuses on LLM integrations, RAG, embeddings and vector retrieval, structured AI outputs, backend APIs, asynchronous processing, external service integrations, and reliable production architecture.

I work across the full product delivery cycle: requirements analysis, architecture, backend implementation, AI integration, testing, production debugging, deployment, and ongoing improvement.

---

## Core Stack

### Python / Backend

- Python 3.12
- FastAPI
- AsyncIO
- REST APIs
- Pydantic 2
- SQLAlchemy 2
- Alembic
- Background processing

### AI / LLM

- OpenAI API and OpenAI-compatible APIs
- LLM integrations
- RAG pipelines
- Embeddings
- Semantic search
- Vector search
- Structured outputs
- Context assembly and management
- Prompt and response validation
- Retry, repair, and fallback flows
- AI workflow orchestration

### Data & Retrieval

- PostgreSQL
- pgvector
- Redis
- SQLite
- Vector retrieval
- Similarity search

### Integrations

- External REST APIs
- Telegram Bot API / aiogram
- Google APIs
- OAuth
- Webhooks
- CRM and business-service integrations

### Infrastructure

- Docker
- Docker Compose
- Linux
- Git / GitHub
- GitHub Actions
- Railway
- Environment-based configuration
- Application logging and health checks

---

## Featured Projects

### Stock Keyworder

AI-assisted metadata generation service for stock photography.

The application processes uploaded images through a vision-capable LLM and generates structured metadata including titles, descriptions, and keywords.

The backend controls the complete processing flow from upload and image normalization to AI generation, validation, persistence, editing, history, and CSV export.

**Engineering highlights**

- Fully asynchronous FastAPI backend
- Async SQLAlchemy 2 persistence layer
- PostgreSQL production database
- Pydantic validation of structured AI responses
- OpenAI Vision integration
- Shared asynchronous HTTP client
- Bounded retries with exponential backoff and jitter
- Alembic database migrations
- Google OAuth authentication
- Batch processing
- User-scoped data access
- AI output validation before persistence

**Stack:** Python 3.12, FastAPI, AsyncIO, SQLAlchemy 2, PostgreSQL, Pydantic 2, httpx, OpenAI API, Alembic, OAuth

**Repository:** [github.com/Sviatana/stock-keyworder](https://github.com/Sviatana/stock-keyworder)

---

### ContextFlow

RAG backend service built with FastAPI and an OpenAI-compatible API.

The service receives a question, retrieves semantically relevant context from a knowledge base using embeddings and similarity search, constructs controlled LLM context, generates an answer, validates the response, and returns structured output.

**Pipeline**

`Request → Retrieval → Context Selection → Prompt Construction → LLM → Validation → Structured Response`

**Engineering highlights**

- Retrieval-augmented generation pipeline
- Embeddings-based semantic retrieval
- Cosine similarity search
- Explicit separation of retrieval and generation
- Controlled context selection
- Structured response validation
- Maintainable FastAPI service architecture

**Stack:** Python, FastAPI, Pydantic, OpenAI-compatible API, embeddings, semantic search, cosine similarity

**Repository:** [github.com/Sviatana/ContextFlow](https://github.com/Sviatana/ContextFlow)

---

### Anima

Production-oriented FastAPI backend architecture for API-driven applications, AI services, and automation systems.

The project demonstrates a modular backend structure with asynchronous request handling, persistent storage, configuration management, CI, and deployment infrastructure.

**Engineering highlights**

- Modular FastAPI architecture
- Async request processing
- PostgreSQL persistence
- SQLAlchemy data layer
- Environment-based configuration
- Database migration structure
- Docker deployment
- GitHub Actions CI
- Railway deployment configuration

**Stack:** Python, FastAPI, AsyncIO, PostgreSQL, SQLAlchemy, Docker, Railway, GitHub Actions

**Repository:** [github.com/Sviatana/anima](https://github.com/Sviatana/anima)

---

## Current Engineering Focus

My current engineering work includes:

- production Python backend development
- LLM-powered applications
- RAG and retrieval pipelines
- embeddings and vector search
- PostgreSQL and pgvector
- Redis-backed application components
- structured and validated LLM outputs
- asynchronous API integrations
- background processing
- context-aware AI workflows
- production debugging and root-cause analysis
- Docker-based deployments

I am particularly interested in building AI systems where LLM generation is only one component of a controlled application pipeline rather than an isolated prompt call.

---

## Engineering Approach

### Controlled AI outputs

LLM responses are treated as untrusted application input.

Where AI output participates in business logic, I prefer explicit schemas, validation, bounded retries, repair/fallback paths, and predictable failure handling.

### Clear architecture

I separate API transport, business logic, AI integrations, retrieval, persistence, and infrastructure concerns instead of placing the complete workflow inside endpoint handlers.

### Async by design

For network-bound applications I use asynchronous request processing and avoid blocking operations in async execution paths.

### Production responsibility

My work does not stop when an endpoint works locally.

I also work with:

- configuration and secrets
- database migrations
- Docker environments
- application logs
- health checks
- production debugging
- deployment verification
- regression testing

### Root-cause debugging

I prefer identifying the source of incorrect behavior in data flow, context, routing, validation, or integration boundaries instead of introducing case-specific hardcoded fixes.

---

## Additional Experience

I have also developed and integrated:

- AI assistants
- Telegram products and Mini Apps
- business automation systems
- external API integrations
- Google API integrations
- OAuth flows
- browser automation
- file processing and parsing
- data validation pipelines
- asynchronous background workflows
- SaaS backend components

---

## What I Build

Typical architecture:

`Client / Bot / Web App`

↓

`FastAPI`

↓

`Application / Domain Logic`

↓

`AI / Retrieval / Integration Services`

↓

`PostgreSQL / pgvector / Redis`

↓

`External APIs / LLM Providers`

The goal is not simply to connect an application to an LLM API, but to build a backend around the model that controls context, data, validation, persistence, errors, and system behavior.

---

## Contacts

**Email:** ssidaren@gmail.com

**Website:** [ai24solutions.ru](https://ai24solutions.ru)

**LinkedIn:** [linkedin.com/in/sviatanasidarenka](https://www.linkedin.com/in/sviatanasidarenka/)

**Telegram:** [t.me/sidarenkas](https://t.me/sidarenkas)
