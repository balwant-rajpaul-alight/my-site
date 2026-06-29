# Career Roadmap: RPA Engineer → GenAI / Agentic AI Engineer

> **Prepared**: June 2026  
> **Profile**: Mid-level Python automation engineer at Alight Solutions  
> **Current Domain**: RPA, Contact Center (Genesys), HR/Benefits, QA Automation  
> **Target**: GenAI Engineer / Agent Engineer / Applied AI Engineer  

---

## Table of Contents

1. [Your Current Skill Snapshot](#1-your-current-skill-snapshot)
2. [Market Reality Check — June 2026](#2-market-reality-check--june-2026)
3. [Target Roles & Salary Bands](#3-target-roles--salary-bands)
4. [Skill Gap Analysis](#4-skill-gap-analysis)
5. [The Roadmap — 6 Phases over ~9 Months](#5-the-roadmap--6-phases-over-9-months)
6. [Phase 1 — Foundation Fixes (Weeks 1–3)](#phase-1--foundation-fixes-weeks-13)
7. [Phase 2 — LLM Application Engineering (Weeks 4–8)](#phase-2--llm-application-engineering-weeks-48)
8. [Phase 3 — RAG Systems & Evaluation (Weeks 9–14)](#phase-3--rag-systems--evaluation-weeks-914)
9. [Phase 4 — Agentic AI Engineering (Weeks 15–22)](#phase-4--agentic-ai-engineering-weeks-1522)
10. [Phase 5 — Production, Security & LLMOps (Weeks 23–30)](#phase-5--production-security--llmops-weeks-2330)
11. [Phase 6 — Portfolio Capstone & Job Prep (Weeks 31–36)](#phase-6--portfolio-capstone--job-prep-weeks-3136)
12. [Portfolio Projects That Get Interviews](#7-portfolio-projects-that-get-interviews)
13. [Learning Resources — Curated & Prioritised](#8-learning-resources--curated--prioritised)
14. [Certifications Worth Getting](#9-certifications-worth-getting)
15. [Weekly Time Budget](#10-weekly-time-budget)
16. [How to Leverage Your RPA Background](#11-how-to-leverage-your-rpa-background)
17. [Red Flags to Avoid](#12-red-flags-to-avoid)
18. [Decision: Self-Study vs Bootcamp vs Hybrid](#13-decision-self-study-vs-bootcamp-vs-hybrid)
19. [90-Day Quick Wins](#14-90-day-quick-wins)

---

## 1. Your Current Skill Snapshot

### What You Already Have (Transferable Strengths)

| Skill | Evidence from Your Work | GenAI Relevance |
|-------|------------------------|-----------------|
| **Python (intermediate+)** | 50+ scripts, classes, functions, error handling | Core language for all GenAI engineering |
| **REST API integration** | JIRA, SharePoint, Genesys, ServiceNow, New Relic, AWS | LLM APIs, tool-calling, webhook systems |
| **OAuth2 / Auth patterns** | Client credentials, Basic auth, API keys, Base64 encoding | API security, JWT/OIDC for agents |
| **Data wrangling** | pandas, openpyxl, regex, JSON traversal | Dataset curation, eval datasets, ETL for RAG |
| **PII detection & log masking** | HMAC tokenisation, regex-based PII scanning, risk ratings | Directly maps to Presidio/NER-based PII in AI systems |
| **Automation pipelines** | End-to-end: data acquisition → processing → reporting | Same pattern as RAG/agent pipelines |
| **Excel/report engineering** | Dynamic header discovery, multi-sheet comparison, colour-coded validation | Eval report generation, dashboard data |
| **AWS basics** | S3, Bedrock (Claude 3.5), Lambda handlers | Cloud deployment for AI services |
| **Domain depth** | Contact center IVR, HR benefits config, auth models | Vertical AI agent opportunities |
| **Error handling patterns** | try/except with categorised exceptions, retry logic | LLM reliability patterns (retry, fallback) |

### What You've Started But Need to Deepen

| Area | Current State | Target State |
|------|--------------|--------------|
| OpenAI API | Single hello-world call | Streaming, structured output, tool calling, multi-model |
| Embeddings | Encoded text with `all-MiniLM-L6-v2` | Full RAG pipeline with vector DB, chunking, retrieval |
| AWS Bedrock | Lambda log summariser template | Production inference with cost controls |
| Computer Vision | OpenCV frame analysis for screen recordings | Multimodal embeddings (CLIP), image RAG |

---

## 2. Market Reality Check — June 2026

### What's Happened in the Last 12 Months

1. **Agentic AI is the dominant hiring theme**. Companies want engineers who can build multi-step AI systems, not just prompt wrappers. "Agent Engineer" is now a distinct job title on LinkedIn and Naukri.

2. **MCP (Model Context Protocol) and A2A (Agent-to-Agent)** have become production standards. Both are now under the Linux Foundation's AAIF, co-governed by OpenAI, Anthropic, Google, Microsoft, and AWS. Knowing these protocols is becoming as fundamental as knowing REST.

3. **Evaluation engineering is the new differentiator**. Companies have realised that building LLM apps is easy — making them reliable is hard. Engineers who can design eval suites, measure hallucination rates, and run regression tests on prompts are in very high demand.

4. **Open-source models are production-viable**. Llama 3, Mistral, Phi-3 run locally via Ollama. Companies want engineers who can choose between frontier APIs and open-source based on cost/latency/privacy tradeoffs — not just default to OpenAI.

5. **RPA is being absorbed into AI automation**. UiPath, Automation Anywhere, and Microsoft Power Automate are all adding GenAI features. Pure RPA roles are flattening; hybrid RPA+AI roles are growing. This is your transition window.

6. **India GenAI salary data (Glassdoor, June 2026)**:
   - Entry (1-3 yrs): ₹5L–₹24L (wide range based on skill proof)
   - Mid (4-6 yrs): ₹9L–₹20L+ 
   - Senior (7-9 yrs): ₹15L–₹77L
   - US remote: $124K–$193K (relevant for freelance/contract work)

7. **Supply-demand gap is still real**. Most candidates can call an API. Very few can design an eval pipeline, debug hallucinations systematically, or architect a multi-agent system with proper state management.

### What Hiring Managers Actually Look For

Based on current job postings for GenAI/Agent Engineer roles:

```
MUST-HAVE (Table Stakes)
├── Python 3.10+ (async, type hints, Pydantic)
├── LLM API integration (OpenAI, Anthropic, Google)
├── Prompt engineering (system prompts, few-shot, chain-of-thought)
├── RAG pipeline (embeddings → vector DB → retrieval → generation)
├── Basic evaluation (accuracy, groundedness, latency measurement)
└── Docker + Git (CI/CD basics)

STRONG DIFFERENTIATORS (Gets You Shortlisted)  
├── Agentic systems (tool loops, state management, multi-agent)
├── MCP server development
├── Evaluation science (LLM-as-judge, regression testing, adversarial)
├── Open-source model experience (fine-tuning, local inference)
├── PII detection / security guardrails
├── Production deployment with observability
└── System design thinking for AI architectures

RARE & VALUABLE (Gets You the Offer)
├── A2A protocol implementation
├── AI reliability engineering (hallucination debugging, prompt versioning)
├── FinOps for LLMs (cost routing, prompt caching, SLM routing)
├── End-to-end deployed system with metrics
└── Domain-specific AI agents (HR, contact center, compliance)
```

---

## 3. Target Roles & Salary Bands

| Role | India (₹ LPA) | US Remote ($K) | Your Fit |
|------|---------------|----------------|----------|
| **GenAI Engineer** | 12–30L | 120–180K | Primary target — your Python + API skills map directly |
| **Agent Engineer** | 15–35L | 130–200K | High-growth role — build multi-agent systems |
| **Applied AI Engineer** | 12–28L | 115–170K | Broader — AI features in products |
| **AI Platform Engineer** | 18–40L | 140–210K | Infra-heavy — needs stronger DevOps |
| **AI Solutions Engineer** | 10–25L | 100–150K | Client-facing — your domain knowledge is gold here |
| **LLM App Developer** | 10–22L | 100–160K | Build-focused — quickest path from your current skills |

### Recommended Primary Target: **GenAI Engineer** or **Agent Engineer**
### Recommended Bridge Role: **AI Solutions Engineer** (leverages your domain + automation background immediately)

---

## 4. Skill Gap Analysis

### Critical Gaps (Must Fix — Blocks Every Application)

| Gap | Why It Matters | Time to Fix |
|-----|---------------|-------------|
| No RAG pipeline experience | Required in 90%+ of GenAI job descriptions | 3-4 weeks |
| No prompt engineering depth | System prompts, few-shot, chain-of-thought, structured output | 2 weeks |
| No LLM orchestration framework | LangChain/LangGraph/LlamaIndex expected | 3 weeks |
| No Docker in practice | Every deployment requires containerisation | 1 week |
| No Git/CI/CD hygiene | `.gitignore`, branches, PRs, GitHub Actions | 1 week |
| No `pytest` or testing framework | Production code needs automated tests | 1 week |
| No async Python | `asyncio`/`aiohttp` needed for concurrent LLM calls | 1 week |

### Important Gaps (Fix During Learning — Strengthens Applications)

| Gap | Why It Matters | Time to Fix |
|-----|---------------|-------------|
| No secrets management | Hardcoded API keys are a red flag in interviews | 1 day |
| No evaluation/measurement | LLM output quality metrics, golden datasets | 2-3 weeks |
| No agent state management | Tool loops, checkpoints, persistent state | 2-3 weeks |
| No fine-tuning experience | LoRA/PEFT on open-source models | 2 weeks |
| No MCP/A2A protocol knowledge | Emerging standard, strong differentiator | 2 weeks |
| No frontend for AI apps | Basic Streamlit/React for demo UIs | 1 week |

### Already Strong (Just Need to Reframe for GenAI Context)

| Strength | How to Reframe |
|----------|---------------|
| PII detection & log masking | → "Built PII detection pipeline for LLM-safe data processing" |
| API integration patterns | → "Designed tool-calling interfaces for AI agent systems" |
| Data validation & comparison | → "Developed evaluation frameworks for automated quality assurance" |
| Retry logic & error handling | → "Implemented reliability patterns for LLM response handling" |
| Excel report generation | → "Built automated reporting pipelines for AI system metrics" |

---

## 5. The Roadmap — 6 Phases over ~9 Months

```
PHASE 1 ─── Foundation Fixes ──────────────── Weeks 1–3
    │   Secrets, Docker, Git, async, pytest, Pydantic
    │
PHASE 2 ─── LLM Application Engineering ──── Weeks 4–8
    │   APIs, prompting, structured output, streaming, tool calling
    │
PHASE 3 ─── RAG & Evaluation ─────────────── Weeks 9–14
    │   Embeddings, vector DBs, RAG pipeline, eval science
    │
PHASE 4 ─── Agentic AI Engineering ───────── Weeks 15–22
    │   Agents, multi-agent, MCP, A2A, memory, state
    │
PHASE 5 ─── Production & Security ────────── Weeks 23–30
    │   Deploy, observe, PII/guardrails, reliability, FinOps
    │
PHASE 6 ─── Portfolio & Job Prep ─────────── Weeks 31–36
        Capstone polish, resume, interview prep, applications
```

---

## Phase 1 — Foundation Fixes (Weeks 1–3)

> **Goal**: Fix engineering hygiene gaps that would be red flags in any code review or interview.

### Week 1: Secrets, Environment & Git Hygiene

**Do these on your existing codebase (learn by fixing your own code):**

- [ ] Install and configure `python-dotenv` — move all hardcoded API keys to `.env` files
- [ ] Create a proper `.gitignore` (Python template + `.env`, `*.pyc`, `__pycache__/`)
- [ ] Set up a clean Git repo with meaningful commits (not "update" or "fix")
- [ ] Learn branching: `main` → `feature/xyz` → PR → merge
- [ ] Create a GitHub account (if not active) and push 2-3 cleaned-up projects

**Deliverable**: Your `OpenAI_Api.py`, `SharepointTesting.py`, and `SharePoint_File_Lister.py` refactored with `.env` secrets management and pushed to GitHub with clean commits.

### Week 2: Docker & Testing

- [ ] Install Docker Desktop
- [ ] Dockerise one of your existing scripts (e.g., `check_abb_services.py`)
- [ ] Write a `Dockerfile` + `docker-compose.yml`
- [ ] Learn `pytest` basics — write 5 tests for one of your validation scripts
- [ ] Add `conftest.py`, fixtures, parametrised tests

**Deliverable**: One Dockerised Python project with 5+ passing `pytest` tests.

### Week 3: Async Python & Pydantic v2

- [ ] Learn `asyncio` basics: `async def`, `await`, `asyncio.gather()`
- [ ] Convert one API-calling script to async (e.g., JIRA or Genesys API calls)
- [ ] Learn Pydantic v2: `BaseModel`, validators, serialisation
- [ ] Use Pydantic to define typed models for one of your API responses (e.g., Genesys conversation model)
- [ ] Learn type hints: annotate functions in 2-3 scripts

**Deliverable**: One async API client + Pydantic response models for Genesys or JIRA data.

---

## Phase 2 — LLM Application Engineering (Weeks 4–8)

> **Goal**: Go from "I've called the OpenAI API once" to "I can build production LLM features."

### Week 4: LLM API Mastery

- [ ] OpenAI Chat Completions: system prompts, temperature, max_tokens, stop sequences
- [ ] Anthropic Claude API: messages format, system prompt differences
- [ ] Google Gemini API: basic text generation
- [ ] **Compare outputs** from all three on the same prompt — document differences
- [ ] API error handling: rate limits, retries with exponential backoff, timeouts

**Build**: `ModelCompare` — A script that sends the same prompt to 3 providers and compares response quality, latency, and cost. Use your existing retry logic patterns.

### Week 5: Prompt Engineering Depth

- [ ] System prompt design: role, context, constraints, output format
- [ ] Few-shot prompting with examples
- [ ] Chain-of-thought (CoT) prompting
- [ ] Self-consistency (multiple reasoning paths)
- [ ] Prompt templates with variable injection (not f-strings — use proper templating)

**Build**: `TicketClassifier` — Takes your JIRA ticket descriptions, classifies by priority/category/team using structured prompts. Compare zero-shot vs few-shot vs CoT accuracy.

### Week 6: Structured Outputs & Pydantic Enforcement

- [ ] OpenAI JSON mode
- [ ] OpenAI Structured Outputs (function calling with Pydantic schemas)
- [ ] Anthropic tool use for structured extraction
- [ ] Pydantic validation of LLM responses
- [ ] Handling malformed LLM output: parsing fallbacks, retry on validation failure

**Build**: `ConfigExtractor` — Feed your auth config validation data through an LLM to extract structured config objects with Pydantic validation. Compare against your existing regex-based extraction.

### Week 7: Tool Calling & Function Execution

- [ ] OpenAI function calling (tools parameter)
- [ ] Anthropic tool use
- [ ] Design tool schemas (name, description, parameters)
- [ ] Tool execution loop: LLM decides → execute function → feed result back
- [ ] Safety: tool allowlists, parameter validation before execution

**Build**: `OpsHelper` — An LLM that can call your existing functions (JIRA search, SharePoint file listing, Genesys conversation lookup) as tools. This directly leverages your existing codebase.

### Week 8: Streaming & SSE

- [ ] OpenAI streaming responses
- [ ] Server-Sent Events (SSE) with FastAPI
- [ ] Build a streaming FastAPI endpoint
- [ ] Basic Streamlit UI for chat interface
- [ ] Token counting and cost tracking per request

**Build**: `StreamChat` — FastAPI + Streamlit chat app with streaming responses, token counting, and cost display. Connect to the tools from Week 7.

---

## Phase 3 — RAG Systems & Evaluation (Weeks 9–14)

> **Goal**: Build a real retrieval system and learn to measure whether it actually works.

### Week 9: Embeddings & Vector Databases

- [ ] Embedding models: `text-embedding-3-small`, `all-MiniLM-L6-v2`, Nomic Embed
- [ ] Understand embedding dimensions, similarity metrics (cosine, dot product)
- [ ] Set up a vector database: start with **ChromaDB** (local), then try **Pinecone** or **Qdrant**
- [ ] Index 50+ documents, query with semantic search
- [ ] Chunking strategies: fixed-size, sentence-based, recursive character splitting

**Build**: `DocSearch` — Index your existing `.md` files (EXTRACTION_QUICK_START.md, SERVICES_EXTRACTION_GUIDE.md) and Python docstrings. Semantic search over your own documentation.

### Week 10: RAG Pipeline Architecture

- [ ] Full RAG flow: query → embed → retrieve → augment prompt → generate
- [ ] Context window management (what fits, what gets truncated)
- [ ] Citation generation (source attribution in responses)
- [ ] "I don't know" handling (when retrieval confidence is low)
- [ ] Conversation memory in RAG (multi-turn with context)

**Build**: `KnowledgeBot` — RAG system over Alight's service documentation (or any domain docs you can use). Answers with citations. Handles out-of-scope questions gracefully.

### Week 11: Advanced RAG Techniques

- [ ] Query transformation: HyDE (Hypothetical Document Embeddings)
- [ ] Multi-query retrieval (generate multiple search queries from one question)
- [ ] Reranking (cross-encoder reranker after initial retrieval)
- [ ] Context compression (summarise retrieved chunks before sending to LLM)
- [ ] Hybrid search (keyword BM25 + semantic vector)
- [ ] Metadata filtering (date range, category, source type)

**Build**: Upgrade `KnowledgeBot` with reranking + hybrid search. Measure before/after on retrieval quality.

### Week 12: Evaluation Foundations

- [ ] **Golden datasets**: Create a set of question-answer pairs with expected answers
- [ ] Metrics: accuracy, groundedness, relevance, faithfulness
- [ ] LLM-as-Judge: use one LLM to evaluate another's output
- [ ] RAGAS framework for RAG evaluation
- [ ] A/B testing: compare two RAG configs on the same eval set
- [ ] Track metrics over time (regression detection)

**Build**: `EvalHarness` — Evaluation pipeline for your RAG system. 20+ golden QA pairs, automated scoring, before/after comparison reports.

### Week 13: Adversarial Testing & Red-Teaming

- [ ] Prompt injection attacks (direct and indirect)
- [ ] Jailbreak attempts on your system
- [ ] Data exfiltration through clever prompting
- [ ] Hallucination-inducing queries
- [ ] Edge cases: empty input, extremely long input, multilingual, code injection

**Build**: Extend `EvalHarness` with an adversarial test suite. Document which attacks succeed and how you defended against them.

### Week 14: Multimodal RAG

- [ ] PDF ingestion (text + tables + images)
- [ ] Image embeddings with CLIP or OpenCLIP
- [ ] GPT-4o Vision / Claude Vision for image understanding
- [ ] Combined text + image retrieval
- [ ] Table extraction and structured indexing

**Build**: `MultimodalSearch` — Index PDFs with figures and tables (use your Genesys documentation or any technical PDFs). Search returns relevant text AND images.

---

## Phase 4 — Agentic AI Engineering (Weeks 15–22)

> **Goal**: Build AI systems that can reason, use tools, and coordinate with other agents.

### Week 15: Agent Fundamentals

- [ ] Understand the agent loop: Observe → Think → Act → Observe
- [ ] ReAct pattern (Reasoning + Acting)
- [ ] Tool schemas and execution
- [ ] Stop conditions (when to stop the loop)
- [ ] State management: short-term (conversation), workflow (steps), persistent (memory)
- [ ] **Critical**: When NOT to use agents (explicit rejection exercise)

**Build**: `ServiceAgent` — Single agent that can check service status, query JIRA for related tickets, and suggest fixes. Uses your existing API integrations as tools. Include a state diagram.

### Week 16: LangGraph for Agent Orchestration

- [ ] LangGraph basics: nodes, edges, state
- [ ] Conditional routing (different paths based on LLM output)
- [ ] Tool nodes and human-in-the-loop nodes
- [ ] Checkpointing and state persistence
- [ ] Streaming agent execution

**Build**: Refactor `ServiceAgent` using LangGraph. Add conditional routing (simple query → RAG path, action needed → tool path, unclear → human approval path).

### Week 17–18: Multi-Agent Systems

- [ ] Agent roles: router, specialist, reviewer
- [ ] Handoff protocols between agents
- [ ] Manager-worker patterns
- [ ] Shared vs isolated state
- [ ] OpenTelemetry tracing for multi-agent flows
- [ ] **When NOT to over-engineer**: explicit "reject multi-agent" exercise

**Build**: `TriageSystem` — Three agents: (1) Triage agent classifies incoming requests, (2) Knowledge agent answers from docs, (3) Action agent creates JIRA tickets or triggers workflows. Full trace replay.

### Week 19: Long-Term Memory

- [ ] In-context memory (conversation history management)
- [ ] External memory with vector store (persistent knowledge)
- [ ] Episodic memory (conversation summaries)
- [ ] Procedural memory (learned user preferences)
- [ ] Memory lifecycle: when to store, when to forget, when to update

**Build**: Add 4-layer memory to `TriageSystem`: Redis session state, pgvector long-term, episodic summaries, user preference learning.

### Week 20: MCP (Model Context Protocol)

- [ ] MCP architecture: what it is, why it matters
- [ ] Build an MCP server (expose your existing tools as MCP capabilities)
- [ ] MCP client integration
- [ ] Tool discovery and invocation
- [ ] Testing MCP servers locally

**Build**: `MCPToolServer` — Expose your JIRA search, SharePoint file listing, and Genesys lookup functions as an MCP server. Test with Claude Desktop or an MCP client.

### Week 21: A2A (Agent-to-Agent Protocol)

- [ ] A2A architecture: Agent Cards, task lifecycle
- [ ] SSE streaming for A2A communication
- [ ] JWT/OIDC security for agent authentication
- [ ] Publishing a discoverable agent service
- [ ] Client-remote architecture

**Build**: `A2AService` — Expose your TriageSystem as an A2A-compatible service with a signed Agent Card, SSE streaming, and JWT auth.

### Week 22: AGENTS.md & Agent Documentation

- [ ] Write AGENTS.md files for your repos (repo context for AI tools)
- [ ] Agent capability documentation
- [ ] Tool schema documentation
- [ ] Integration testing for agent systems

**Build**: Complete AGENTS.md for your capstone project. Document every agent, tool, and interaction pattern.

---

## Phase 5 — Production, Security & LLMOps (Weeks 23–30)

> **Goal**: Ship AI systems that are secure, observable, reliable, and cost-efficient.

### Week 23: PII Detection & Guardrails

- [ ] Microsoft Presidio for PII detection and scrubbing
- [ ] spaCy NER for entity detection
- [ ] Input sanitisation before LLM calls
- [ ] Output filtering before returning to users
- [ ] PII handling in RAG pipelines (tiered access)
- [ ] GDPR/CCPA compliance basics

**Build**: `GuardLayer` — Middleware that detects and scrubs PII from inputs and outputs of your agent system. **You already have PII detection skills from `log_masker.py` and `pi_data_analyzer.py` — extend them with Presidio.**

### Week 24: Prompt Injection Defense & Security

- [ ] Direct prompt injection (user input overrides system prompt)
- [ ] Indirect prompt injection (malicious content in retrieved documents)
- [ ] Tool misuse prevention (agent calls dangerous tools)
- [ ] RBAC for agent capabilities
- [ ] Approval checkpoints + audit logging
- [ ] Red-team your own system

**Build**: `SecurityAudit` — Document and defend against 10 attack vectors on your agent system. Implement RBAC, approval gates, and audit logging.

### Week 25–26: Deployment & CI/CD

- [ ] Docker multi-stage builds for Python AI apps
- [ ] Docker Compose for multi-service AI systems (app + vector DB + Redis)
- [ ] GitHub Actions CI/CD pipeline
- [ ] Cloud deployment: start with Railway/Render (simple), then AWS ECS or Azure Container Apps
- [ ] Environment management: dev/staging/prod configs
- [ ] Health checks and readiness probes

**Build**: Deploy your capstone system to the cloud with full CI/CD. Every push runs tests + eval suite.

### Week 27: Observability & Monitoring

- [ ] OpenTelemetry for LLM applications
- [ ] Trace every LLM call: model, prompt, response, tokens, latency, cost
- [ ] LangSmith or Langfuse for LLM-specific observability
- [ ] Alerting on quality degradation
- [ ] Dashboard for system health

**Build**: Add OpenTelemetry instrumentation to your capstone. Build a monitoring dashboard showing latency, cost, and quality metrics.

### Week 28: Reliability Engineering

- [ ] Hallucination debugging decision tree:
  - Retrieval gap? → Fix indexing/chunking
  - Prompt ambiguity? → Fix system prompt
  - Model mismatch? → Try different model
  - Parsing failure? → Fix output enforcement
- [ ] Prompt versioning in Git (track every change, regression test)
- [ ] Model upgrade control (A/B test, frozen test sets)
- [ ] Pydantic enforcement patterns for robust parsing
- [ ] Fallback strategies when structured output breaks

**Build**: `ReliabilityKit` — Implement the hallucination debugging decision tree, prompt versioning workflow, and model upgrade protocol for your capstone.

### Week 29: Fine-Tuning & Open-Source Models

- [ ] When fine-tuning wins vs prompting vs RAG (decision framework)
- [ ] OpenAI fine-tuning API (GPT-4o-mini)
- [ ] PEFT/LoRA on Llama 3 with Hugging Face
- [ ] Ollama for local inference
- [ ] LoRA mechanics: understand what low-rank decomposition does
- [ ] Benchmark: base prompting vs fine-tuned on accuracy, latency, cost, privacy

**Build**: `SpecialistModel` — Fine-tune a model on your domain data (ticket classification or config validation). Benchmark against base prompting. Write a decision memo.

### Week 30: FinOps & Cost Optimisation

- [ ] Token counting and per-request cost tracking
- [ ] Prompt caching (Anthropic/OpenAI)
- [ ] SLM routing: route simple tasks to smaller/cheaper models
- [ ] Cost budgets per request/user/day
- [ ] Cost dashboard with actual measurements

**Build**: `CostRouter` — Routing layer that classifies request complexity and routes to appropriate model (GPT-4o vs GPT-4o-mini vs local Llama). Weekly cost measurement report.

---

## Phase 6 — Portfolio Capstone & Job Prep (Weeks 31–36)

> **Goal**: Package everything into a portfolio that proves you can ship production AI systems.

### Week 31–33: Capstone — "Alight Ops Intelligence Platform"

Build a complete system that directly maps your RPA/automation domain:

```
┌─────────────────────────────────────────────────┐
│         Alight Ops Intelligence Platform         │
│                                                  │
│  ┌──────────┐  ┌──────────┐  ┌──────────────┐  │
│  │ Knowledge │  │  Triage  │  │    Action     │  │
│  │   Agent   │  │  Agent   │  │    Agent      │  │
│  │           │  │          │  │               │  │
│  │ RAG over  │  │ Classify │  │ JIRA create,  │  │
│  │ runbooks  │  │ & route  │  │ SP upload,    │  │
│  │ + docs    │  │ requests │  │ alert trigger │  │
│  └──────────┘  └──────────┘  └──────────────┘  │
│         │              │              │          │
│  ┌──────┴──────────────┴──────────────┴──────┐  │
│  │           Orchestration Layer              │  │
│  │    LangGraph + MCP Tools + A2A Service     │  │
│  └───────────────────────────────────────────┘  │
│         │              │              │          │
│  ┌──────┴──┐  ┌────────┴───┐  ┌──────┴──────┐  │
│  │ Guard   │  │ Eval &     │  │ Observ. &   │  │
│  │ Layer   │  │ Reliability│  │ Cost Router │  │
│  │ PII +   │  │ Kit        │  │ OpenTelemetry│ │
│  │ RBAC    │  │            │  │ + FinOps    │  │
│  └─────────┘  └────────────┘  └─────────────┘  │
└─────────────────────────────────────────────────┘
```

This capstone directly leverages:
- Your JIRA, SharePoint, Genesys, ServiceNow integrations (as agent tools)
- Your PII detection work (as the guard layer)
- Your validation scripts (as the eval framework pattern)
- Your domain knowledge (HR benefits, contact center operations)

### Week 34: Resume & Portfolio Polish

Write resume bullets that you can actually defend:

```
BEFORE (RPA resume):
"Developed Python automation scripts for data validation and reporting"

AFTER (GenAI resume):
"Built multi-agent ops intelligence platform with RAG over technical runbooks,
 PII-scrubbed citations, MCP tool integration, and automated eval pipeline —
 deployed with OpenTelemetry observability and cost-aware model routing"
```

**Portfolio Checklist:**
- [ ] GitHub repos with clean READMEs, architecture diagrams, and eval reports
- [ ] Live deployed demo (even on free tier)
- [ ] Blog post or technical write-up explaining one system design decision
- [ ] AGENTS.md in every repo
- [ ] Video demo (2-3 minutes) walking through the capstone

### Week 35–36: Interview Preparation

**Top 8 questions you must be able to answer from experience:**

1. "When would you use RAG vs fine-tuning vs agents?" → Your SpecialistModel benchmarks
2. "What do you do when your LLM hallucinates?" → Your ReliabilityKit decision tree
3. "How do you evaluate an LLM application?" → Your EvalHarness with golden datasets
4. "How do you handle PII in an AI system?" → Your GuardLayer with Presidio
5. "Explain MCP and A2A" → Your MCPToolServer and A2AService
6. "Walk through designing a system like [X]" → Your capstone architecture
7. "When would you choose open-source vs proprietary?" → Your SpecialistModel decision memo
8. "When is multi-agent overkill?" → Your explicit rejection exercise

---

## 7. Portfolio Projects That Get Interviews

| # | Project | What It Proves | Week |
|---|---------|---------------|------|
| 1 | `ModelCompare` | You understand multi-provider LLM usage | 4 |
| 2 | `OpsHelper` | You can build tool-calling LLM systems | 7 |
| 3 | `KnowledgeBot` | You can build and improve RAG systems | 10–11 |
| 4 | `EvalHarness` | You measure and improve AI quality | 12–13 |
| 5 | `TriageSystem` | You can build multi-agent systems | 17–19 |
| 6 | `MCPToolServer` | You know production agent protocols | 20 |
| 7 | `GuardLayer` | You handle security and PII properly | 23 |
| 8 | `ReliabilityKit` | You solve reliability at scale | 28 |
| 9 | `SpecialistModel` | You can fine-tune and benchmark models | 29 |
| 10 | **Capstone** | You can architect and ship complete AI systems | 31–33 |

---

## 8. Learning Resources — Curated & Prioritised

### Tier 1: Start Here (Free)

| Resource | What It Covers | Priority |
|----------|---------------|----------|
| [DeepLearning.AI Short Courses](https://www.deeplearning.ai/short-courses/) | RAG, agents, prompt engineering, LangChain | ★★★★★ |
| [LangChain Documentation + Tutorials](https://python.langchain.com/) | LangChain, LangGraph, LCEL | ★★★★★ |
| [OpenAI Cookbook](https://cookbook.openai.com/) | Structured outputs, embeddings, evals | ★★★★★ |
| [Anthropic Prompt Engineering Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering) | Production prompt patterns | ★★★★☆ |
| [MCP Specification](https://modelcontextprotocol.io/) | MCP architecture and implementation | ★★★★☆ |
| [A2A Protocol Spec](https://github.com/google/A2A) | Agent-to-agent communication | ★★★☆☆ |

### Tier 2: Go Deeper (Free / Low Cost)

| Resource | What It Covers | Priority |
|----------|---------------|----------|
| [Hugging Face NLP Course](https://huggingface.co/learn) | Transformers, fine-tuning, embeddings | ★★★★☆ |
| [Full Stack LLM Bootcamp (YouTube)](https://fullstackdeeplearning.com/) | Production LLM systems | ★★★★☆ |
| [RAGAS Documentation](https://docs.ragas.io/) | RAG evaluation framework | ★★★★☆ |
| [Microsoft Presidio](https://microsoft.github.io/presidio/) | PII detection (you already have the intuition) | ★★★★☆ |
| [Docker for Python Developers](https://docs.docker.com/guides/python/) | Containerisation | ★★★☆☆ |

### Tier 3: Books (Invest When Ready)

| Book | What It Covers |
|------|---------------|
| *Building LLM Apps* by Valentina Alto (O'Reilly) | End-to-end LLM application development |
| *Designing Machine Learning Systems* by Chip Huyen | System design for ML (applies to LLMs) |
| *AI Engineering* by Chip Huyen (2024) | Production AI patterns |

### Tier 4: Paid Courses (If Budget Allows)

| Course | Cost | Value |
|--------|------|-------|
| **CoreSmart Applied GenAI** (17 weeks) | ₹85K–₹175K | Best if you want structured live mentoring + cohort |
| DataCamp AI Engineer Track | ~₹15K/year | Good for foundations, weak on agentic/production |
| Udemy/Coursera LangChain courses | ~₹500–₹2K | Good supplementary, not sufficient alone |

---

## 9. Certifications Worth Getting

| Certification | Issuer | Value | When to Get |
|--------------|--------|-------|-------------|
| AWS Certified AI Practitioner | AWS | Broad recognition | After Phase 2 |
| DeepLearning.AI Generative AI with LLMs | Coursera | Good foundation credential | After Phase 2 |
| LangChain Certified Developer | LangChain (if available) | Shows framework proficiency | After Phase 4 |
| GitHub Copilot Certification | GitHub | Shows AI-assisted development | Anytime |

> **Reality check**: Certifications help pass HR filters but don't substitute for a portfolio. A deployed system with metrics beats any certificate.

---

## 10. Weekly Time Budget

Assuming you're working full-time at Alight and learning on the side:

| Activity | Hours/Week | Notes |
|----------|-----------|-------|
| Structured learning (courses/docs) | 5–6 hrs | Mornings or evenings |
| Hands-on building (projects) | 6–8 hrs | Weekends primarily |
| Code review & reflection | 1 hr | Review what you built, improve |
| Community/reading (blogs, Discord, X) | 1–2 hrs | Stay current on GenAI trends |
| **Total** | **13–17 hrs/week** | Sustainable pace for 9 months |

### Making It Sustainable

- **Apply learning at work immediately**: Propose an AI-assisted validation tool at Alight. Even a small LLM integration into your existing RPA workflow counts as production experience.
- **Weekend deep dives**: Use Saturdays for project building, Sundays for review.
- **Don't context-switch**: Focus on one phase at a time. Resist the urge to jump ahead.

---

## 11. How to Leverage Your RPA Background

Your RPA experience is not a liability — it's a **strategic advantage** if framed correctly.

### Direct Mappings

| RPA Concept | GenAI Equivalent | Your Advantage |
|-------------|-----------------|----------------|
| Bot orchestration | Multi-agent orchestration | You understand sequencing, error handling, fallbacks |
| Attended vs unattended bots | Human-in-the-loop vs autonomous agents | You know when humans must approve |
| Exception handling (business vs system) | Hallucination categories, tool failures | You already categorise failures |
| Data validation scripts | Evaluation pipelines | Same pattern: expected vs actual |
| Process mining | Agent trace analysis | Understanding workflow patterns |
| UiPath/AA360 tool execution | MCP tool calling | Same concept, different protocol |

### Story to Tell in Interviews

> "I spent [X] years automating enterprise processes with RPA — I understand the full lifecycle from requirements to production monitoring. What I've done in the last [Y] months is apply that same systems thinking to AI-powered automation. RPA handles deterministic processes; GenAI handles the judgment-heavy parts that RPA couldn't touch. I've built systems that combine both — deterministic workflow orchestration with AI-powered decision-making at the judgment points."

### Internal Opportunities at Alight

Before looking externally, explore:
1. **Propose an AI-enhanced RPA project**: e.g., LLM-powered ticket classification before routing to existing RPA bots
2. **Build a RAG system over internal runbooks**: Your Genesys/auth documentation is already structured for this
3. **Automate your own validation work with LLMs**: Your config comparison scripts could use LLM reasoning for edge cases
4. **Join or start an AI guild/community of practice** within Alight

---

## 12. Red Flags to Avoid

### In Learning

- ❌ Tutorial hell: Watching 50 hours of courses without building anything
- ❌ Framework tourism: Learning LangChain AND LlamaIndex AND CrewAI AND AutoGen before mastering one
- ❌ Ignoring evaluation: Building RAG without measuring if it actually works
- ❌ Skipping fundamentals: Jumping to agents before understanding prompt engineering
- ❌ Over-engineering: Building multi-agent when single-agent suffices

### In Job Search

- ❌ Listing "OpenAI API" as a skill without a project to show
- ❌ Certificate-only resume with no deployed code
- ❌ Hiding RPA background (frame it as a strength instead)
- ❌ Applying only to "GenAI Engineer" titles — also look for "AI Solutions Engineer", "Applied AI", "Automation + AI" hybrid roles
- ❌ Ignoring domain specialisation: Your HR/contact center knowledge is valuable in vertical AI

### In Career

- ❌ Waiting for the "perfect" time to transition — the market window is now
- ❌ Only targeting Big Tech — mid-size companies and product startups are hiring faster for GenAI roles
- ❌ Ignoring the "boring" parts: security, reliability, cost control are what separate senior from junior GenAI engineers

---

## 13. Decision: Self-Study vs Bootcamp vs Hybrid

| Path | Duration | Cost | Best If... |
|------|----------|------|-----------|
| **Self-study (this roadmap)** | 9 months | ₹0–5K (tools/APIs) | You're disciplined, can build solo, want flexibility |
| **Bootcamp (CoreSmart)** | 17 weeks (~4 months) | ₹85K–₹175K | You want structured mentoring, cohort pressure, faster pace |
| **Hybrid (recommended)** | 6–9 months | ₹5K–₹20K | Use this roadmap + free courses + 1-2 paid short courses for gaps |

### My Recommendation: **Hybrid Path**

1. **Weeks 1–8**: Follow this roadmap's Phase 1–2 using free resources (DeepLearning.AI short courses + OpenAI Cookbook)
2. **Weeks 9–14**: Take a focused RAG course (DeepLearning.AI has free ones) + build your own eval harness
3. **Weeks 15–22**: LangGraph documentation + build your agent projects
4. **Weeks 23–30**: Production skills from blog posts, docs, and hands-on deployment
5. **Weeks 31–36**: Portfolio polish + interview prep

**Consider CoreSmart IF**:
- You have the budget (₹85K+)
- You want live mentoring and code review
- You want the cohort network (40 students doing A2A together)
- You want to compress the timeline to 17 weeks
- Ask them your due-diligence questions first (see previous analysis)

---

## 14. 90-Day Quick Wins

Things you can do **right now** to start the transition:

### Week 1 (This Week)
- [ ] Move all hardcoded API keys in your workspace to `.env` files
- [ ] Set up a GitHub account/profile and push 3 clean repos
- [ ] Take DeepLearning.AI's "ChatGPT Prompt Engineering for Developers" (1 hour, free)

### Week 2–4
- [ ] Build `ModelCompare` (compare 3 LLM providers on same task)
- [ ] Dockerise one of your existing Genesys validation scripts
- [ ] Add `pytest` tests to one validation script

### Month 2
- [ ] Build a RAG system over your documentation
- [ ] Create your first golden dataset (20 QA pairs) and measure accuracy
- [ ] Write one blog post about "What I learned building my first RAG system"

### Month 3
- [ ] Build a tool-calling agent using your JIRA/SharePoint integrations
- [ ] Learn LangGraph basics and refactor the agent
- [ ] Update your LinkedIn headline: "Python Engineer | Building GenAI Systems | Ex-RPA"

### By Day 90
You should have:
- ✅ 3+ GitHub repos with GenAI projects
- ✅ 1 RAG system with eval metrics
- ✅ 1 tool-calling agent using your existing APIs
- ✅ Updated LinkedIn and resume
- ✅ 1 published blog post or technical write-up
- ✅ Foundation for everything in Phases 4–6

---

## Final Note

You're not starting from zero. Your Python skills, API integration experience, PII detection work, and automation pipeline thinking are **exactly** what production GenAI engineering needs. Most GenAI bootcamp graduates have the theory but lack the production instinct you already have.

The gap is specific and fixable: RAG, prompt engineering, agents, evaluation, and deployment practices. This roadmap fills those gaps while building on the strengths you already have.

The transition window is open now. RPA is being absorbed into AI-powered automation. Engineers who can bridge both worlds — deterministic process automation AND AI-powered decision-making — are uniquely valuable.

Start with Phase 1 this week. Don't wait for perfect conditions.

---

*Last updated: June 2026*
