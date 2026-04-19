# Hi, I'm Oluwabusayo 👋
### AI Engineer · Agent Architect · AI Orchestrator

> *I don't just build AI tools — I design intelligent systems that think, reason, and act in the real world.*

---

## 🧠 What I Do

I specialize in **designing and orchestrating multi-agent AI systems** — from knowledge graphs powering legal intelligence, to stateful image editing pipelines, to real-time WhatsApp business automation. My work sits at the intersection of **AI architecture, agent orchestration, and production-grade engineering**.

I think in systems. I build in Python and TypeScript. I ship agents that work.

---

## 🚀 Featured Projects

### ⚖️ [LegalMind — AI-Powered Legal Document Intelligence](https://github.com/oluwabusayoagentzero/Legal-Draft-AI)
> *Because legal intelligence is not retrieval — it is traversal.*

A full-stack agentic platform that transforms how legal professionals create, query, and validate documents. Instead of naive RAG, LegalMind models legal documents as **knowledge graphs** — where clauses, parties, obligations, and regulations are nodes connected by typed relationships.

**What makes it interesting architecturally:**
- Multi-agent orchestration with **Pydantic AI** — a dedicated Orchestrator agent coordinates Query, Draft, and Playbook agents
- **Neo4j knowledge graph** for cross-reference resolution and structural dependency validation (not flat text retrieval)
- **Regulatory Intelligence Layer** — auto-fetches current jurisdiction-specific laws on every draft, with conflict detection (CRITICAL / HIGH / MEDIUM / LOW severity) and a user-guided resolution UI
- **Streaming SSE API** — real-time draft progress via Server-Sent Events
- Dual intake system: Lawyer Form (technical) and Business Owner Form (plain English)
- Containerized with Docker Compose; **Chainlit** chat UI + **FastAPI** REST backend

**Stack:** Python 3.12 · FastAPI · Pydantic AI · Anthropic Claude · Neo4j · pgvector · Docling · Chainlit · Docker

---

### 🖼️ [Antigravity Image Generation Fix — Stateful AI Image Editing](https://github.com/oluwabusayoagentzero/Antigravity-image-generation-fix)
> *Solving context amnesia in multimodal AI agents.*

Identified and engineered a fix for a **critical context management failure** in multi-turn AI image editing workflows: subsequent edit instructions were always applied to the original uploaded image instead of the latest edited output — making iterative edits impossible.

**What makes it interesting architecturally:**
- Designed a **two-tier implementation strategy**:
  - *Tier 1* — Lightweight `ImageEditingAgent` class with rolling `current_image_path` state (prototypes, scripts)
  - *Tier 2* — **LangGraph** stateful graph with typed `ImageEditState`, checkpointed sessions, and thread-safe concurrency (production)
- Full rollback capability to any prior edit by index
- Session isolation for concurrent users (MemorySaver → SQLite → PostgreSQL backends)
- State management overhead under 50ms per turn
- Chainlit UI for interactive multi-turn editing sessions

**Stack:** Python 3.10+ · LangChain · LangGraph · Google Gemini · Pillow · Chainlit · SQLite/PostgreSQL

---

### 🍟 [Brezzy — WhatsApp Restaurant Order Management Agent](https://github.com/oluwabusayoagentzero/brezzy-whatsapp-restaurant-agent)
> *Bringing AI-powered order automation to a real food business.*

A production-ready, real-time order management dashboard built for **Brezzy Stirs & Fries** — a WhatsApp-based food delivery business. The system connects a WhatsApp Business AI agent to a live Supabase database, with a React dashboard that updates in real time.

**What makes it interesting architecturally:**
- **Supabase Realtime subscriptions** — live sync for new orders, payment updates, and customer changes with zero polling
- **Webhook endpoint** (`/api/webhook`) for receiving WhatsApp Business API events serverlessly on Vercel
- Notification system with toast alerts, sound toggles, and a notification history panel
- Full TypeScript codebase with typed database schema and client
- Deployed on **Vercel** (serverless) with clear ARCHITECTURE, DEPLOYMENT, and TESTING documentation

**Stack:** React 18 · TypeScript · Tailwind CSS · Supabase · Supabase Realtime · Vite · Vercel · Node.js

---

## 🛠️ Tech & Tools

**AI & Agents**
`Anthropic Claude` · `Pydantic AI` · `LangChain` · `LangGraph` · `Google Gemini` · `OpenAI` · `Chainlit`

**Backend & APIs**
`Python 3.12` · `FastAPI` · `Node.js` · `Uvicorn` · `Pydantic` · `Structlog`

**Databases & Search**
`Neo4j` · `PostgreSQL + pgvector` · `Supabase` · `SQLite`

**Frontend**
`React 18` · `TypeScript` · `Tailwind CSS` · `Vite`

**DevOps & Infra**
`Docker` · `Docker Compose` · `Vercel` · `GitHub Actions`

**Document & Media**
`Docling` · `python-docx` · `LlamaParse` · `Pillow`

---

## 🎯 How I Think About AI Engineering

**Agents are not chatbots.** They are systems with memory, tools, decision logic, and failure modes. I design them with that in mind.

**State is everything.** Whether it's a legal clause dependency graph, an image edit history, or a live order feed — the intelligence is in how state is modeled, propagated, and recovered.

**Orchestration is the real skill.** Picking a model is easy. Designing how multiple agents coordinate, hand off context, handle failures, and produce coherent outputs — that's the hard part. That's what I focus on.

---

## 📬 Let's Connect

- **GitHub:** [@oluwabusayoagentzero](https://github.com/oluwabusayoagentzero)
- Open to collaborations on agentic AI systems, LLM infrastructure, and AI-powered product engineering.

---

*Building the infrastructure layer for intelligent systems — one agent at a time.*

<!--
**oluwabusayoagentzero/oluwabusayoagentzero** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
