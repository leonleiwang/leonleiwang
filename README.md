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

我专注于 **AI Agent、多智能体系统、RAG 检索增强、Tool Calling、LLM Application 与生产级 AI 系统工程化**，持续探索智能客服、企业知识库、电商、智能运维与工作流自动化等场景中的 AI 原生产品与 Agent Skill。

当前重点关注：

- **Agentic Systems**：任务规划、工具调用、多智能体协作、上下文管理与执行链路控制
- **RAG / 企业知识库**：混合检索、证据引用、低置信转人工、RAG 评测与知识库运营
- **Agent Governance**：风险控制、HITL 人工审批、权限边界、审计日志与安全策略
- **Harness Engineering**：Agent 测试、运行、回放、评测、成本控制与可观测性
- **Full-stack AI Products**：从后端 API、数据库建模、前端交互到 Docker 部署的端到端交付

---

## 🚀 核心项目 Featured Projects

### 🛒 ShopMind AI

**多智能体对话式电商系统**  [![GitHub release](https://img.shields.io/github/v/release/leonleiwang/ShopMind-AI?include_prereleases&label=v1.1.1&style=flat-square)](https://github.com/leonleiwang/ShopMind-AI)

面向电商场景的 AI 智能导购、运营、客服与 Agent 评测系统，整合商品搜索、推荐、对比、加购、下单、客服工单、HITL 治理、AgentOps 可观测性与 Data Agent 查询能力。

> 🎉 **Agent Eval + Data Agent v1.1.1 已发布**：[查看 Release](https://github.com/leonleiwang/ShopMind-AI/releases/tag/v1.1.1)  
> 在客服联络中心 v1.1.0 的基础上，新增 Agent Eval + Data Agent 模块，包含 50 条业务评测任务、Baseline Eval、正常任务通过率、Guardrail 拦截率、失败分类、只读 SQL 安全策略、JSON/CSV 报告导出、自然语言数据查询 Console，以及订单异常、客服 SLA、商品表现、退款风险等数据分析场景。

*Multi-Agent Conversational Commerce System powered by LangGraph, MCP-style Tool Calling, RAG, Agent Governance, Agent Eval and Data Agent.*

---

### 🎧 ContactFlow AI

**企业客服工单与 AI 坐席辅助系统**  [![GitHub branch](https://img.shields.io/badge/branch-feature%2Fv0.2--rag--infra-blue?style=flat-square)](https://github.com/leonleiwang/ContactFlow-AI)

面向企业客服与工单处理场景的 AI Contact Center 原型系统，采用 **Java Spring Boot + Python AI Service + React** 构建，围绕工单流转、AI 坐席辅助、企业知识库 RAG、异步事件处理与服务治理，探索大模型能力在客服 SaaS 中的工程化落地。

> 🚧 **V0.2 RAG Infrastructure 更新中**：[查看分支](https://github.com/leonleiwang/ContactFlow-AI/tree/feature/v0.2-rag-infra)  
> 已实现工单状态机、并发抢单、审计事件、AI Assist 幂等写入、Python RAG Query API、120 条企业客服评估样本、Markdown 知识库 ingestion、Hybrid Retrieval、Query Rewrite 漂移过滤、证据引用、租户隔离、低置信转人工与 RAG 评估指标。

*Enterprise AI Contact Center prototype with Spring Boot, Python AI Service, React, RAG, Redis/MQ-ready architecture, evidence trace and evaluation-driven AI Assist.*

---

### 🛠 DevMind AI Sentinel

**多智能体智能运维平台**  [![GitHub release](https://img.shields.io/github/v/release/leonleiwang/DevMind-AI-Sentinel?include_prereleases&label=v1.0.0-GA&style=flat-square)](https://github.com/leonleiwang/DevMind-AI-Sentinel)

面向云原生微服务环境的智能 Agent 运维助手，支持故障定位、指标分析、Incident Timeline、RCA 分析、多 Agent 协作与智能治理。

> 🎉 **正式版 v1.0.0 已发布**：[查看 Release](https://github.com/leonleiwang/DevMind-AI-Sentinel/releases/tag/v1.0.0)  
> 新增 Incident Timeline / RCA 分析、模糊输入处理、前端优化与效果视频演示。

*AI-native intelligent operations platform for cloud-native services with multi-agent collaboration and observability.*

---

### 🎬 OneClick Viral Shorts Skill

**短视频研究与发布包生成 Agent Skill**  

面向短视频内容创作场景的 AI Agent Skill，根据内容类型、平台、风格与时长自动生成研究分析、剪辑策略、字幕、标题与发布包，支持内容生产与发布工作流自动化。

*AI-powered short-video research and publishing workflow for generating content analysis, editing strategies, subtitles and publishing assets through reusable agent workflows.*

---

### 🛍 OneClick Store Marketing Skill

**实体店营销素材生成 Agent Skill**

面向本地门店场景的 AI Agent Skill，通过一句话输入自动生成营销宣传包，覆盖海报、橱窗广告、活动方案、社媒文案与商品图 Prompt 等多渠道营销素材。

*AI-powered local store marketing skill for generating promotional assets, social content and campaign materials through reusable agent workflows.*

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
- Conversational Systems：对话式电商、客服与企业知识助手
- AI Commerce：AI 电商、智能运营、货架 AI 与商家 Copilot
- Production-ready LLM Applications：生产级 LLM 应用工程、成本控制与稳定性治理

---

## 📫 联系方式 Contact

📧 leileonwang@163.com  
📧 leonlei.wang@outlook.com  

🌍 求职地：南京 / 上海 / 杭州 / 苏州，可快速到岗  
🌍 Based in Nanjing, China · Open to opportunities in China, Australia, New Zealand and Europe.

