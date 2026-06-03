<div align="center">

# Lei Wang / Leon Wang

**AI Agent Engineer | LLM Application Engineer | Fullstack Developer | Fullstack AI Products**

<p>
  English · <a href="./README.md">中文</a>
</p>

</div>

---

## 👋 About Me

I focus on building **AI-native applications powered by LLMs, Agentic Systems, RAG, Tool Calling, Multi-Agent Workflows, and production-ready AI engineering practices**.

My current work explores how AI agents can be applied to realistic business scenarios such as conversational commerce, customer support, enterprise knowledge bases, intelligent operations, workflow automation, and reusable Agent Skills.

Current focus areas:

- **Agentic Systems**: planning, tool use, multi-agent collaboration, context management, and controlled execution
- **RAG / Enterprise Knowledge Base**: hybrid retrieval, evidence citation, low-confidence escalation, RAG evaluation, and knowledge operations
- **Agent Governance**: human-in-the-loop review, permission boundaries, audit logs, risk control, and safe execution
- **Harness Engineering**: agent testing, replay, evaluation, cost tracking, observability, and runtime debugging
- **Full-stack AI Products**: end-to-end delivery from backend APIs, database modeling, frontend dashboards, LLM integration, and Docker deployment

---

## 🚀 Featured Projects

### 🛒 ShopMind AI

**Multi-Agent Conversational Commerce System**  
[![GitHub release](https://img.shields.io/github/v/release/leonleiwang/ShopMind-AI?include_prereleases&label=v1.1.1&style=flat-square)](https://github.com/leonleiwang/ShopMind-AI)

ShopMind AI is an AI-native commerce and customer support platform that integrates conversational shopping, product search, recommendation, comparison, cart and order workflows, customer support tickets, HITL governance, AgentOps observability, and Data Agent analytics.

> 🎉 **Agent Eval + Data Agent v1.1.1 released**: [View Release](https://github.com/leonleiwang/ShopMind-AI/releases/tag/v1.1.1)  
> Built on top of the v1.1.0 customer support module, v1.1.1 adds Agent Eval + Data Agent capabilities, including 50 business evaluation cases, baseline evaluation, normal task pass rate, guardrail probe capture rate, failure taxonomy, SELECT-only SQL safety policy, JSON/CSV report export, natural language data query console, and analytics scenarios for order exceptions, support SLA, product performance, and refund risk.

**Tech focus:** LangGraph, MCP-style Tool Calling, RAG, Agent Governance, Agent Eval, Data Agent, FastAPI, PostgreSQL, Redis, Next.js, React, TypeScript.

---

### 🎧 ContactFlow AI

**Enterprise Customer Support Ticketing, AI Agent Assist and RAG Knowledge Base System**
[![GitHub release](https://img.shields.io/badge/release-v0.3.0-blue?style=flat-square)](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)

ContactFlow AI is an enterprise AI Contact Center prototype built with **Java Spring Boot + Python FastAPI AI Service + React**. It brings ticket workflow management, AI-assisted replies, enterprise knowledge base RAG, asynchronous events, idempotency, evidence tracing, and evaluation metrics into one support SaaS engineering workflow.

> 🚀 **V0.3.0 released**: [View Release](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)
> Built on top of the V0.2 traceable RAG and RabbitMQ / Redis infrastructure, V0.3.0 adds optional Qwen3-Max / qwen-plus LLM integration, template fallback, optional qwen3-rerank, local lightweight rerank fallback, 20 frontend demo tickets, stricter API contracts, edge behavior documentation, Docker environment propagation, and release-readiness checks. The system is designed to remain demoable even when the real LLM is unavailable.

**Engineering scope:**

- **Ticket workflow**: Spring Boot domain model, state machine, concurrent ticket claiming, audit events, Flyway MySQL schema, and idempotent AI Assist persistence.
- **Agent Assist**: rule-based engine plus optional Qwen3-Max generation; falls back to safe templates when the LLM is disabled, missing credentials, timed out, or returns invalid output.
- **RAG knowledge base**: Markdown ingestion, dynamic NLP-aware chunking, parent-child chunks, query rewrite validation, vector + BM25 hybrid retrieval, citations, and low-confidence handoff.
- **Rerank and evaluation**: optional qwen3-rerank with local lightweight fallback; includes context recall, faithfulness, citation coverage, hallucination risk, tenant leak count, and retrieval latency metrics.
- **Frontend demo**: React three-column agent workspace with 20 realistic support tickets across logistics, refund, invoice, cross-border, complaint, unsupported entitlement, and supervisor escalation scenarios.
- **Engineering readiness**: Docker Compose, environment templates, API contract docs, edge behavior docs, RAG build/eval scripts, and tests; real vector DB, production knowledge governance, Kafka, live ticket integration, and RAG ops dashboards are planned for V0.4.0.

**Tech focus:** Spring Boot, FastAPI AI Service, React, Qwen3-Max, qwen3-rerank, RAG, hybrid retrieval, evidence trace, fallback-first AI Assist, API contract validation, Docker, Redis, RabbitMQ, evaluation-driven workflow.

---

### 🛠 DevMind AI Sentinel

**Multi-Agent Intelligent Operations Platform**  
[![GitHub release](https://img.shields.io/github/v/release/leonleiwang/DevMind-AI-Sentinel?include_prereleases&label=v1.0.0-GA&style=flat-square)](https://github.com/leonleiwang/DevMind-AI-Sentinel)

DevMind AI Sentinel is an AI-native intelligent operations assistant for cloud-native microservice environments. It supports incident diagnosis, metrics analysis, incident timeline, RCA analysis, multi-agent collaboration, and observability-oriented operations workflows.

> 🎉 **v1.0.0 GA released**: [View Release](https://github.com/leonleiwang/DevMind-AI-Sentinel/releases/tag/v1.0.0)  
> Added Incident Timeline / RCA analysis, fuzzy input handling, frontend improvements, and demo video support.

**Tech focus:** Multi-agent operations, RCA, observability, incident analysis, FastAPI, tool integration, intelligent operations workflow.

---

### 🎬 OneClick Viral Shorts Skill

**Short-video Research and Publishing Agent Skill**

An AI-powered Agent Skill for short-video content creation. Based on content type, platform, style, and target duration, it generates content analysis, editing strategies, subtitles, titles, and publishing assets to support automated content production workflows.

**Tech focus:** Agent Skill design, content workflow automation, video research, subtitle generation, publishing package generation.

---

### 🛍 OneClick Store Marketing Skill

**Local Store Marketing Asset Generation Agent Skill**

An AI-powered Agent Skill for local store marketing. From a simple natural language input, it generates promotional assets such as posters, window ads, campaign plans, social media copy, and product-image prompts.

**Tech focus:** Agent Skill design, marketing automation, prompt workflow, campaign asset generation, local business use cases.

---

## 🧰 Tech Stack

### Backend

Python · FastAPI · Java · Spring Boot · PostgreSQL · MySQL · Redis · RabbitMQ / Kafka · Celery · Docker

### Frontend

React · Next.js · Vue3 · TypeScript · Tailwind CSS

### AI / Agentic Systems

LangChain · LangGraph · Agent Harness · RAG · Hybrid Retrieval · Tool Calling · MCP-style Tools · Multi-Agent Workflow

### Governance / Harness Engineering

Agent Governance · RAG Evaluation · Evidence Trace · Observability · Routing · Prompt Versioning · Workflow Debugging · Resilience · Retry / Fallback / Circuit Breaker

---

## 🌱 Currently Exploring

- **Agent Governance**: risk control, permission boundaries, audit logs, and safe execution
- **Harness Engineering**: agent testing, runtime evaluation, replay, observability, and debugging
- **Conversational Systems**: conversational commerce, customer support, and enterprise knowledge assistants
- **AI Commerce**: AI shopping, seller operations, product shelf intelligence, and merchant copilot workflows
- **Production-ready LLM Applications**: cost control, reliability engineering, evaluation, and deployment practices

---

## 📫 Contact

📧 leileonwang@163.com  
📧 leonlei.wang@outlook.com  

🌍 Based in Nanjing, China · Open to opportunities in China, Australia, New Zealand and Europe.  
🌍 China job locations: Nanjing / Shanghai / Hangzhou / Suzhou, available for quick onboarding.
