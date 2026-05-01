# Hi, I'm Godspower Anthony-Ikpe 👋

Backend engineer specializing in AI integration. I build production-grade systems that combine solid backend engineering with modern AI tooling — LangChain, LangGraph, CrewAI, and the Anthropic API.

---

## What I'm building

### IhuSale
A multi-tenant SaaS platform for Instagram vendors across Africa. Connects to Instagram's API and uses Claude AI to automatically classify customer intent and reply in real time — handling product inquiries, order placement, and follow-ups without manual intervention.

- FastAPI backend with Celery for async AI processing
- Multi-tenant data isolation
- End-to-end automation from DM receipt to AI reply delivery
- Analytics on response rates, conversions, and AI cost
- 170+ automated tests
- Sole backend engineer — designed and built from scratch

### Content Agent
An AI-powered personal content automation system. Passively monitors my daily development activity — git commits, Claude Code sessions, VSCode file edits, GitHub PRs — and snapshots everything every 3 hours. A single Telegram command triggers a multi-agent CrewAI pipeline that reads the snapshots, identifies the most compelling work, generates platform-specific drafts for Twitter, LinkedIn, Reddit, Facebook, and Instagram, creates matching AI-generated images, and runs an automated quality review. Drafts land in Telegram with approve/reject buttons.

- Multi-agent orchestration with CrewAI (aggregator → strategist → writers → reviewer)
- Deployed on Hetzner VPS via Docker Compose
- FastAPI receiver endpoint behind nginx with SSL
- Content history persistence to prevent topic repetition over a 30-day rolling window
- Per-platform brand voice configuration via live Telegram command
- Stack: Python, CrewAI, Claude API, FastAPI, Tweepy, LinkedIn UGC API, Telegram Bot API, Docker, nginx, APScheduler

---

## Other projects

### Enterprise CRM (subcontract)
Backend subcontract work on a multi-tenant enterprise CRM in PHP/CodeIgniter across procurement, HR, accounting, and inventory modules.

**HR Employee Evaluation Module** — Full performance evaluation system with configurable criteria, multi-stage submission/review/approval workflow, email notifications, PDF export, and audit trail. DB migration creating 6 new tables.

**Bulk Email for Leads** — Bulk email action on the leads module with per-lead merge field resolution.

Also delivered: stock withdrawal workflow, zero-balance filtering for accounting reports, vendor bank details on purchase PDFs, auto-populating vendor fields on invoices, approval notification bug fixes, full dark mode overhaul, and bulk import bug fixes.

### School Management System (subcontract)
Backend work on a full school management platform covering student records, attendance, and academic reporting.

### Mediasoup Video Call App
Real-time peer-to-peer video calling application. Stack: Node.js, MediaSoup, WebRTC, Socket.io.

### Web3 Carbon Credits Platform
Blockchain-integrated platform for carbon credit tracking and trading. Stack: TypeScript, Wagmi, Viem, Hardhat.

### Tour Bookings API
RESTful booking system for tour management. Stack: Node.js, Express.js.

### Real Estate App
Property listing and management application. Stack: Node.js, JavaScript.

---

## Tech stack

**AI & Agents**
Python · LangChain · LangGraph · CrewAI · Anthropic Claude API · OpenAI API · RAG pipelines · Tool calling · Multi-agent orchestration

**Backend**
FastAPI · NestJS · Express.js · PHP/CodeIgniter · Celery · APScheduler · RESTful APIs · WebSockets

**Databases**
PostgreSQL · MySQL · Redis

**DevOps & Infrastructure**
Docker · Docker Compose · nginx · Linux · Hetzner VPS · GitHub Actions · Systemd

**Other**
Telegram Bot API · Instagram Graph API · Tweepy · ActivityWatch · Git

---

## Writing

I write about LangChain, LangGraph, and the practical side of building AI-powered backend systems.

- [LangChain fundamentals: the mental model that makes everything click](https://dev.to/youngtee100/langchain-fundamentals-the-mental-model-that-makes-everything-click-4101)
- [LangChain fundamentals part 2: structured outputs and tool calling](https:
