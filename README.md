# Sviatlana Sidarenka

**AI Engineer · GenAI / LLM Applications · Python Backend**

I design and build applied AI systems, AI assistants, RAG applications, backend services, and business automation products.

My work covers the full delivery cycle: requirements analysis, architecture and technology selection, implementation, AI integration, testing, debugging, deployment, and production improvement.

My main engineering focus is not isolated LLM calls, but controlled AI systems where models work together with retrieval, structured data, business logic, permissions, validation, background processing, and reliable failure handling.

## Main Areas

### GenAI / LLM

- LLM-powered applications
- RAG pipelines
- Embeddings and semantic retrieval
- Vector search
- AI assistants
- Agentic workflows
- LangChain / LangGraph
- Structured outputs
- Tool-calling patterns
- Context and state management
- Prompt and response validation
- Grounded generation
- Fallback and repair flows
- Human-in-the-loop workflows

### Python / Backend

- Python 3.12
- FastAPI
- AsyncIO
- REST APIs
- Pydantic 2
- SQLAlchemy 2
- Alembic
- Background workers
- External API integrations

### Data

- PostgreSQL
- pgvector
- Redis
- SQLite
- Relational data modelling
- Vector retrieval
- Similarity search

### Infrastructure

- Docker
- Docker Compose
- Linux
- Git / GitHub
- GitHub Actions
- Cloud deployment
- Environment-based configuration
- Application logging
- Health and readiness checks
- Production debugging

## Product Work

### AI24 Persona Studio

Corporate AI platform for managing AI personas, knowledge, content, roles, and controlled publishing.

**Status:** active development

The platform is being developed for companies that need managed AI representatives for brands and future automation of social-media activity.

Implemented and ongoing areas include:

- organization / brand / persona hierarchy
- Python / FastAPI backend
- PostgreSQL and pgvector
- Redis and ARQ background processing
- private object storage
- document and knowledge processing
- role-based access control
- ownership and scope checks
- audit and versioning
- controlled content lifecycle
- human review and approval before publication
- isolation of knowledge between organizations, brands, and personas
- Docker-based infrastructure
- automated backend checks

Current development is focused on using AI personas for controlled social-media content workflows.

A further product direction is **visual AI agents**: AI representatives with their own visual identity, knowledge, behaviour and controlled actions.

**Product:** [persona.ai24solutions.online](https://persona.ai24solutions.online/)

---

### Anvera

SaaS application for building AI assistants from company knowledge.

The product implements a complete RAG workflow:

- user authentication
- AI assistant creation and configuration
- PDF, TXT, Markdown and manual-text knowledge upload
- private document storage
- chunking
- embeddings
- vector retrieval
- RAG-based grounded answers
- fallback when the knowledge base does not contain a confirmed answer
- dialogue context
- protection boundaries for retrieved content
- Playground
- Free / Pro limits
- publication
- embeddable website widget
- separate public assistant identifiers
- automated tests and browser E2E checks

**Stack:** Next.js, React, TypeScript, PostgreSQL, pgvector, Supabase, OpenRouter, Cloudflare Workers, Vitest, Playwright

**Live:** [paralect-chatbot-builder.ssidaren.workers.dev](https://paralect-chatbot-builder.ssidaren.workers.dev)

**Demo:** [Northstar Coffee](https://paralect-chatbot-builder.ssidaren.workers.dev/demo/northstar-coffee)

---

### Song Gift

Production AI service for creating personalized songs from a user's story.

The system includes:

- Telegram product flow
- Python backend
- external AI API integrations
- user state management
- asynchronous and background processing
- separate music-generation worker
- error handling
- service health checks
- Docker deployment
- end-to-end automated tests
- GPU inference integration through a separate RunPod deployment layer

Long-running music generation is isolated from the user-facing API so that model inference can be monitored and scaled separately.

**Telegram:** [t.me/PesnyaVPodarokAIBot](https://t.me/PesnyaVPodarokAIBot)

**Product:** [pesnya-v-podarok.online](https://pesnya-v-podarok.online)

---

### SportMethod

Digital methodology and training-management platform for sports organizations.

The system turns distributed documents and spreadsheets into structured operational data.

Implemented functionality includes:

- exercise bank
- methodology management
- annual planning
- weekly planning
- training-session planning
- plan / fact tracking
- attendance
- athlete results
- Excel import and export
- structured data model
- analytics
- data mart for reporting and analysis

This project is an example of a data-first architecture where AI capabilities are built around reliable structured business data.

**Demo:** [sportmethod.ai24solutions.online/demo](https://sportmethod.ai24solutions.online/demo)

---

### AI24garden

Product and marketplace platform for plant nurseries and sellers.

**Status:** active development

The backend is based on Python / FastAPI and PostgreSQL.

Current implementation includes:

- plant and variety domain model
- product catalogue
- product variants
- seller / nursery entities
- images and media
- inventory-related data
- public catalogue APIs
- import workflows
- validation and preview of imported data
- PostgreSQL
- SQLAlchemy
- Alembic migrations
- Docker
- automated backend tests

The architecture keeps botanical/domain data separate from commercial product data.

AI-based matching and recommendation functionality is being developed on top of this structured model rather than replacing it with an LLM-only approach.

**Product:** [ai24garden.online](https://ai24garden.online/)

---

### AI Assistant for Medical Centers

AI assistant for automating the first stage of communication with patients.

The assistant is designed to:

- answer service-related questions
- collect initial information
- help determine the relevant service direction
- structure an incoming request
- transfer the conversation to a human administrator when required

The system deliberately uses limited AI autonomy: medical or critical decisions remain with a human specialist.

---

## Public Engineering Repositories

### Stock Keyworder

AI-assisted metadata generation service for stock photography.

The application processes uploaded images through a vision-capable LLM and generates structured titles, descriptions and keywords.

Engineering areas demonstrated in the repository:

- asynchronous FastAPI backend
- async SQLAlchemy 2
- PostgreSQL
- Pydantic validation of AI output
- vision-capable LLM integration
- shared asynchronous HTTP client
- bounded retries
- exponential backoff and jitter
- Alembic migrations
- Google OAuth
- batch processing
- user-scoped data access
- CSV export
- persistence of user edits

**Stack:** Python 3.12, FastAPI, AsyncIO, PostgreSQL, SQLAlchemy 2, Pydantic 2, httpx, OpenAI API, Alembic, OAuth

**Repository:** [github.com/Sviatana/stock-keyworder](https://github.com/Sviatana/stock-keyworder)

---

### ContextFlow

Controlled RAG and LLM orchestration backend built with FastAPI, LangChain and LangGraph.

The workflow includes:

- semantic retrieval
- embeddings
- context selection
- structured generation
- validation
- conditional repair
- bounded retry logic
- typed workflow state

LangGraph `StateGraph` is used to explicitly control transitions between retrieval, generation, validation and repair.

**Stack:** Python 3.12, FastAPI, Pydantic 2, LangGraph, LangChain, OpenAI-compatible API, embeddings, semantic retrieval

**Repository:** [github.com/Sviatana/ContextFlow](https://github.com/Sviatana/ContextFlow)

---

### Anima

Reusable production-style FastAPI backend foundation for API-driven applications, AI services and automation systems.

The repository demonstrates:

- modular FastAPI architecture
- asynchronous request processing
- PostgreSQL integration
- SQLAlchemy data layer
- environment-based configuration
- database migration structure
- Docker deployment
- GitHub Actions CI
- Railway deployment configuration

**Repository:** [github.com/Sviatana/anima](https://github.com/Sviatana/anima)

## How I Choose Technology

I prefer to select tools from the requirements of the system rather than starting with a preferred framework.

Typical factors include:

- type and structure of data
- expected workload
- latency requirements
- reliability
- security
- cost
- maintainability
- deployment environment
- operational complexity
- scalability
- vendor dependency

For example:

- I use PostgreSQL when the core domain is relational and consistency matters.
- I use pgvector when vector retrieval can stay close to relational data without introducing another database too early.
- Long-running operations are moved out of HTTP requests into workers or asynchronous workflows.
- AI output that affects application logic is validated before it is trusted.
- Critical actions remain behind backend permission checks and, where appropriate, human approval.
- I avoid adding orchestration frameworks or additional infrastructure when a simpler architecture solves the same problem.

## Debugging and Reliability

My debugging process is based on locating the failing system layer rather than immediately changing code.

I usually separate the problem into:

- client / UI
- API transport
- application and domain logic
- database
- background worker
- AI / retrieval layer
- external provider
- infrastructure

Typical workflow:

1. reproduce the failure
2. inspect logs and system state
3. identify the failing layer
4. form a concrete hypothesis
5. make the smallest reasonable change
6. add or update a regression test
7. run the relevant quality checks
8. verify the real user flow

For AI systems I additionally inspect:

- retrieved context
- source relevance
- model response
- structured-output validation
- fallback behaviour
- tool arguments
- provider errors
- latency
- retries
- permission boundaries

## Engineering Principles

### LLM output is untrusted input

If an AI response participates in business logic, I prefer explicit schemas, validation, bounded retries and predictable fallback behaviour.

### Business logic stays outside the model

Permissions, critical validation and irreversible actions remain controlled by the application backend.

### AI is one system component

I build applications where models operate together with APIs, databases, retrieval, workers, security controls and business rules.

### Root-cause debugging

I prefer fixing the source of incorrect behaviour in data flow, state, context, routing or integration boundaries instead of introducing isolated hardcoded fixes.

### Production responsibility

Implementation is not complete when an endpoint works locally.

I also work with:

- tests
- configuration
- secrets
- migrations
- Docker
- CI
- health checks
- logs
- deployment verification
- regression testing
- production debugging

## Current Focus

My current engineering focus is:

- applied GenAI systems
- AI assistants
- RAG
- AI agents and agentic workflows
- knowledge systems
- Python / FastAPI backend
- LangChain / LangGraph orchestration
- embeddings and vector retrieval
- structured LLM outputs
- Redis-backed background processing
- AI security and controlled autonomy
- production debugging and observability
- reliable AI product architecture

## Contacts

**GitHub:** [github.com/Sviatana](https://github.com/Sviatana)

**Portfolio:** [ai24solutions.online](https://ai24solutions.online/)

**LinkedIn:** [linkedin.com/in/sviatanasidarenka](https://www.linkedin.com/in/sviatanasidarenka/)

**Telegram:** [t.me/sidarenkas](https://t.me/sidarenkas)

**Email:** ssidaren@gmail.com
