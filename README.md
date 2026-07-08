# Hi, I'm Godspower Anthony-Ikpe 👋

Backend engineer building production systems in **Node.js/NestJS** and **Python/FastAPI**, with deep AI integration work — LangChain, LangGraph, CrewAI, and the Anthropic API.

---

## Production backend systems (NestJS)

### Stradha — Food Ordering Platform
Backend built from scratch in an Nx monorepo — customer API, restaurant dashboard API, and shared database/auth libraries.

- NestJS + TypeORM + PostgreSQL, 15+ entities across users, restaurants, menus, orders, payments, and loyalty
- 6-state order state machine with role-based cancellation rules and a guest checkout flow (Uber Eats pattern) using signed JWTs
- AWS Cognito authentication — token verification, automatic user provisioning, role resolution from Cognito groups
- Hierarchical menu customization system (item → group → option) with min/max rules and price modifiers, validated at order placement

### Schoolix — School Management SaaS
NestJS monorepo REST API (staff-api, student-api) with shared entity/DTO/mailer libraries.

- Full school onboarding as a single atomic transaction
- Invite-based staff onboarding with JWT token versioning — invalidates all tokens on password reset
- Fuzzy student search using PostgreSQL `pg_trgm` composite scoring with privacy masking

### NRL — Music Label Platform
Full REST API (NestJS, TypeORM, PostgreSQL) covering auth, music catalog, media uploads, CMS, and metrics.

- Transactional release management via TypeORM QueryRunner
- Reusable Cloudinary media service with Sharp pre-processing and atomic rollback on transaction failure
- RBAC with a secure admin invitation system

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

### Trywaka
Co-founded gamified fitness app, live with test users.

- NestJS + PostgreSQL backend with AWS Cognito auth shared across mobile and API
- Server-side validation of synced activity data to prevent client-side tampering in reward mechanics

### Content Agent
An AI-powered personal content automation system. Passively monitors my daily development activity — git commits, Claude Code sessions, VSCode file edits, GitHub PRs — and snapshots everything every 3 hours. A single Telegram command triggers a multi-agent CrewAI pipeline that reads the snapshots, identifies the most compelling work, generates platform-specific drafts, creates matching AI-generated images, and runs an automated quality review. Drafts land in Telegram with approve/reject buttons.

- Multi-agent orchestration with CrewAI (aggregator → strategist → writers → reviewer)
- Deployed on Hetzner VPS via Docker Compose
- FastAPI receiver endpoint behind nginx with SSL
- Content history persistence to prevent topic repetition over a 30-day rolling window
- Stack: Python, CrewAI, Claude API, FastAPI, Tweepy, LinkedIn UGC API, Telegram Bot API, Docker, nginx, APScheduler

---

## Other projects

### Synergy ERP (subcontract)
Full-stack work on a large-scale enterprise platform (CodeIgniter, PHP, MySQL, Vue 3) in production across procurement, HR, finance, and operations for multiple enterprise clients.

**HR Employee Evaluation Module** — Full evaluation system with configurable criteria, multi-stage approval workflow, email notifications, PDF export, and audit trail (6-table schema).

Also delivered: procurement approval routing, payment request notifications, purchase order PDF generation, and a multi-root-cause production bug fix spanning PHP, webpack, and CSS layers.

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

**Backend** NestJS · Express.js · FastAPI · PHP/CodeIgniter · RESTful APIs · WebSockets

**Languages** TypeScript · Python · Dart · PHP · JavaScript

**AI & Agents** LangChain · LangGraph · CrewAI · Anthropic Claude API · OpenAI API · RAG pipelines · Tool calling · Multi-agent orchestration

**Databases** PostgreSQL · TypeORM · MySQL · Redis

**DevOps & Infrastructure** Docker · Docker Compose · nginx · Linux · Hetzner VPS · AWS (EC2, Cognito) · GitHub Actions · Systemd

**Other** Telegram Bot API · Instagram Graph API · Tweepy · Git

---

## Writing

I write about LangChain, LangGraph, and the practical side of building AI-powered backend systems.

- [LangChain fundamentals: the mental model that makes everything click](https://dev.to/youngtee100/langchain-fundamentals-the-mental-model-that-makes-everything-click-4101)
- [LangChain fundamentals part 2: structured outputs and tool calling](https://dev.to/youngtee100)
