<div align="center">

# 王磊 / Lei Wang / Leon Wang

**AI Agent 应用开发 | LLM 大模型应用开发 | 全栈工程师 | AI 全栈产品开发**  
**AI Agent Engineer | LLM Application Engineer | Fullstack Developer | Fullstack AI Products**

<p>
  中文 · <a href="./README.en.md">English</a>
</p>

</div>

---

## 👋 关于我

我专注于 **AI Agent、多智能体系统、RAG 检索增强、Function Calling & Tool Use、LLM Application 与生产级 AI 系统工程化**，持续探索智能客服、企业知识库、电商、智能运维与工作流自动化等场景中的 AI 原生产品与 Agent Skill。

当前重点关注：

- **Agentic Systems**：任务规划、工具调用、多智能体协作、上下文管理与执行链路控制
- **RAG / 企业知识库**：混合检索、证据引用、低置信转人工、RAG 评测与知识库运营
- **Agent Governance**：风险控制、HITL 人工审批、权限边界、审计日志与安全策略
- **Harness Engineering**：Agent 测试、运行、回放、评测、成本控制与可观测性
- **Full-stack AI Products**：从后端 API、数据库建模、前端交互到 Docker 部署的端到端交付
- **模型调优**：LLaMA-Factory等框架、vllm / ollama 部署、有监督微调SFT包含常用算法LoRA / QLoRA、PEFT、指令微调和训练参数配置、模型评估和幻觉控制及数据集的清洗和构建等

---

## 🚀 核心项目 Featured Projects

### 🛒 ShopMind AI

**多智能体对话式电商系统**  [![Release](https://img.shields.io/badge/release-v1.1.1-blue?style=flat-square)](https://github.com/leonleiwang/ShopMind-AI)

面向电商场景的 AI 智能导购、运营、客服与 Agent 评测系统，整合商品搜索、推荐、对比、加购、下单、客服工单、HITL 治理、AgentOps 可观测性与 Data Agent 查询能力。

> 🎉 **Agent Eval + Data Agent v1.1.1 已发布**：[查看 Release](https://github.com/leonleiwang/ShopMind-AI/releases/tag/v1.1.1)  
> 在客服联络中心 v1.1.0 的基础上，新增 Agent Eval + Data Agent 模块，包含 50 条业务评测任务、Baseline Eval、正常任务通过率、Guardrail 拦截率、失败分类、只读 SQL 安全策略、JSON/CSV 报告导出、自然语言数据查询 Console，以及订单异常、客服 SLA、商品表现、退款风险等数据分析场景。

*Multi-Agent Conversational Commerce System powered by LangGraph, MCP-style Tool Calling, RAG, Agent Governance, Agent Eval and Data Agent.*

---

### 🎧 ContactFlow AI

**企业客服工单、AI 坐席辅助与 RAG 知识库系统**  [![Release](https://img.shields.io/badge/release-v0.3.0-blue?style=flat-square)](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)

面向企业客服联络台与工单处理场景的 AI Contact Center 原型系统，采用 **Java Spring Boot + Python FastAPI AI Service + React** 构建，将工单状态机、并发抢单、AI Assist、企业知识库 RAG、异步事件、缓存幂等、证据追踪与评估指标整合到同一条客服 SaaS 工程链路中。

> 🚀 **V0.3.0 已发布**：[查看 Release](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)
> 在 V0.2 可追溯 RAG 和 RabbitMQ / Redis 基础设施之上，V0.3.0 新增 Qwen3-Max / qwen-plus 可选 LLM Provider、模板兜底降级、qwen3-rerank 可选重排序、本地 lightweight rerank fallback、20 条多类型前端演示工单、API 合约校验、边界行为文档、Docker 环境变量透传与发布前工程化检查。系统默认不强依赖真实模型，适合面试现场和本地演示时稳定展示。

**中文分段能力概览：**

- **工单主链路**：Spring Boot 工单领域模型、状态机、并发抢单、审计事件、Flyway MySQL 表结构与 AI Assist 幂等落库。
- **AI 坐席辅助**：规则引擎 + 可选 Qwen3-Max 真实生成；LLM 关闭、无 Key、超时或返回异常时自动降级到安全模板回复。
- **RAG 知识库**：Markdown ingestion、NLP 动态切块、父子 chunk、Query Rewrite 语义校验、Vector + BM25 混合召回、证据引用和低置信转人工。
- **重排序与评估**：可选 qwen3-rerank，失败时降级到本地轻量重排序；提供 Context Recall、Faithfulness、Citation Coverage、Hallucination Risk、Tenant Leak Count 等指标。
- **前端展示**：React 三栏坐席台，内置 20 条覆盖物流、退款、发票、跨境、投诉、无证据权益、主管升级等场景的演示工单，并保留 mock/degraded/failed 状态用于可靠演示。
- **工程边界**：Docker Compose、`.env.example`、接口契约文档、边界行为文档、RAG build/eval 脚本与测试覆盖，明确真实向量库、知识治理后台、Kafka、实时前后端联动等规划在 V0.4.0。

**English segmented overview:**

- **Ticket workflow**: Spring Boot domain model, state machine, concurrent ticket claiming, audit events, Flyway MySQL schema, and idempotent AI Assist persistence.
- **Agent Assist**: rule-based engine plus optional Qwen3-Max generation; falls back to safe templates when the LLM is disabled, missing credentials, timed out, or returns invalid output.
- **RAG knowledge base**: Markdown ingestion, dynamic NLP-aware chunking, parent-child chunks, query rewrite validation, vector + BM25 hybrid retrieval, citations, and low-confidence handoff.
- **Rerank and evaluation**: optional qwen3-rerank with local lightweight fallback; includes context recall, faithfulness, citation coverage, hallucination risk, tenant leak count, and retrieval latency metrics.
- **Frontend demo**: React three-column agent workspace with 20 realistic support tickets across logistics, refund, invoice, cross-border, complaint, unsupported entitlement, and supervisor escalation scenarios.
- **Engineering readiness**: Docker Compose, environment templates, API contract docs, edge behavior docs, RAG build/eval scripts, and tests; real vector DB, production knowledge governance, Kafka, live ticket integration, and RAG ops dashboards are planned for V0.4.0.

*Enterprise AI Contact Center prototype with Spring Boot, FastAPI AI Service, React, Qwen3-Max, qwen3-rerank, RAG evidence trace, fallback-first AI Assist, and evaluation-driven support workflows.*

---

### 🛠 DevMind AI Sentinel

**多智能体智能运维平台**  [![Release](https://img.shields.io/badge/release-v1.0.0--GA-blue?style=flat-square)](https://github.com/leonleiwang/DevMind-AI-Sentinel)

面向云原生微服务环境的智能 Agent 运维助手，支持故障定位、指标分析、Incident Timeline、RCA 分析、多 Agent 协作与智能治理。

> 🎉 **正式版 v1.0.0 已发布**：[查看 Release](https://github.com/leonleiwang/DevMind-AI-Sentinel/releases/tag/v1.0.0)  
> 新增 Incident Timeline / RCA 分析、模糊输入处理、前端优化与效果视频演示。

*AI-native intelligent operations platform for cloud-native services with multi-agent collaboration and observability.*

---

## ⚡ OneClick Agent Skills Series

一组面向垂直任务自动化的轻量级 AI Agent Skills，将高频、重复、流程化任务封装为“一句话输入 → 结构化交付包”的可复用智能工作流。系列方向不限定行业，包括内容创作、电商运营、跨境比价、金融分析、医疗信息整理、数据处理与个人效率工具等场景。

A lightweight AI Agent Skills series for vertical task automation, turning simple user inputs into structured, reusable deliverable packages. The series is not limited to one industry and can be extended to content creation, e-commerce operations, cross-border comparison, financial analysis, medical information organization, data processing and productivity workflows.

- **🎬 OneClick Viral Shorts Skill**：短视频研究与发布包生成，覆盖趋势分析、选题策略、剪辑方案、字幕、标题、封面建议与发布资产。
- **🛍 OneClick Store Marketing Skill**：本地门店营销素材生成，覆盖海报文案、橱窗广告、活动方案、社媒内容、商品图 Prompt 与多渠道推广素材。
- 🔜 Coming Next

---

## 🧰 技术栈 Tech Stack

### Backend

Python · FastAPI · Java · Spring Boot · PostgreSQL · MySQL · Redis · RabbitMQ / Kafka · Celery · Docker

### Frontend

React · Next.js · Vue3 · TypeScript · Tailwind CSS

### AI / Agentic Systems

LangChain · LangGraph · Agent Harness · RAG · Hybrid Retrieval · Tool Calling · MCP-style Tools · Multi-Agent Workflow

### Governance / Harness Engineering

Agent Governance · RAG Evaluation · Evidence Trace · Observability · Routing · Prompt Versioning · Workflow Debugging · Resilience · Retry / Fallback / Circuit Breaker

---

## 🌱 当前探索方向 Currently Exploring

- Agent Governance：Agent 治理、风险控制、权限边界与审计
- Harness Engineering：Agent 测试、运行、评测、回放与可观测性
- Conversational Systems：对话式电商、客服助手与企业知识助手、工单流转机、Agent 评估台
- AI Commerce：AI 电商、智能运营、货架 AI 与商家 Copilot
- Production-ready LLM Applications：生产级 LLM 应用工程、成本控制与稳定性治理

---

## 📫 联系方式 Contact

📧 leileonwang@163.com  
📧 leonlei.wang@outlook.com  

🌍 求职地：南京 / 上海 / 杭州 / 苏州，可快速到岗  
🌍 Based in Nanjing, China · Open to opportunities in China, Australia, New Zealand and Europe.

---

<details>
<summary><strong>English Version</strong></summary>

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

**Multi-Agent Conversational Commerce System**  [![GitHub release](https://img.shields.io/github/v/release/leonleiwang/ShopMind-AI?include_prereleases&label=v1.1.1&style=flat-square)](https://github.com/leonleiwang/ShopMind-AI)

ShopMind AI is an AI-native commerce and customer support platform that integrates conversational shopping, product search, recommendation, comparison, cart and order workflows, customer support tickets, HITL governance, AgentOps observability, and Data Agent analytics.

> 🎉 **Agent Eval + Data Agent v1.1.1 released**: [View Release](https://github.com/leonleiwang/ShopMind-AI/releases/tag/v1.1.1)  
> Built on top of the v1.1.0 customer support module, v1.1.1 adds Agent Eval + Data Agent capabilities, including 50 business evaluation cases, baseline evaluation, normal task pass rate, guardrail probe capture rate, failure taxonomy, SELECT-only SQL safety policy, JSON/CSV report export, natural language data query console, and analytics scenarios for order exceptions, support SLA, product performance, and refund risk.

**Tech focus:** LangGraph, MCP-style Tool Calling, RAG, Agent Governance, Agent Eval, Data Agent, FastAPI, PostgreSQL, Redis, Next.js, React, TypeScript.

---

### 🎧 ContactFlow AI

**Enterprise Customer Support Ticketing, AI Agent Assist and RAG Knowledge Base System**  [![GitHub release](https://img.shields.io/badge/release-v0.3.0-blue?style=flat-square)](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)

ContactFlow AI is an enterprise AI Contact Center prototype built with **Java Spring Boot + Python FastAPI AI Service + React**. It brings ticket workflow management, AI-assisted replies, enterprise knowledge base RAG, asynchronous events, idempotency, evidence tracing, and evaluation metrics into one support SaaS engineering workflow.

> 🚀 **V0.3.0 released**: [View Release](https://github.com/leonleiwang/ContactFlow-AI/releases/tag/v0.3.0)
> Built on top of the V0.2 traceable RAG and RabbitMQ / Redis infrastructure, V0.3.0 adds optional Qwen3-Max / qwen-plus LLM integration, template fallback, optional qwen3-rerank, local lightweight rerank fallback, 20 frontend demo tickets, stricter API contracts, edge behavior documentation, Docker environment propagation, and release-readiness checks. The system is designed to remain demoable even when the real LLM is unavailable.

**Tech focus:** Spring Boot, FastAPI AI Service, React, Qwen3-Max, qwen3-rerank, RAG, hybrid retrieval, evidence trace, fallback-first AI Assist, API contract validation, Docker, Redis, RabbitMQ, evaluation-driven workflow.

---

### 🛠 DevMind AI Sentinel

**Multi-Agent Intelligent Operations Platform**  [![GitHub release](https://img.shields.io/github/v/release/leonleiwang/DevMind-AI-Sentinel?include_prereleases&label=v1.0.0-GA&style=flat-square)](https://github.com/leonleiwang/DevMind-AI-Sentinel)

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

</details>
