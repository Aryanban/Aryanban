# Aryan Bansal

<p align="left">
  <b>Software Engineer &amp; Builder</b> · IIIT Delhi (Computer Science &amp; Design '28)<br/>
  Building low-level systems, database architectures, autonomous AI engines, and production full-stack platforms.
</p>

<p align="left">
  <a href="https://www.webforge.me/"><img src="https://img.shields.io/badge/Portfolio-webforge.me-6366F1?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://dholeramap.com/"><img src="https://img.shields.io/badge/DholeraMap-Live%20GIS-0284C7?style=flat-square&logo=mapbox&logoColor=white" alt="DholeraMap" /></a>
  <a href="https://plotbook.webforge.me/"><img src="https://img.shields.io/badge/PlotBook-Live%20SaaS-059669?style=flat-square&logo=googlemaps&logoColor=white" alt="PlotBook" /></a>
  <a href="https://github.com/Aryanban/leadforge"><img src="https://img.shields.io/badge/LeadForge-Autonomous%20Outreach-F59E0B?style=flat-square&logo=python&logoColor=white" alt="LeadForge" /></a>
  <a href="https://github.com/Aryanban/seoforge"><img src="https://img.shields.io/badge/SEOForge-MCP%20Crawler-10B981?style=flat-square&logo=typescript&logoColor=white" alt="SEOForge" /></a>
  <a href="https://www.linkedin.com/in/aryan-bansal-b29b69370/"><img src="https://img.shields.io/badge/LinkedIn-Aryan_Bansal-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:aryan24120@iiitd.ac.in"><img src="https://img.shields.io/badge/Email-aryan24120-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

### About Me

I am a Computer Science & Design undergraduate at **IIIT Delhi** who builds across the entire software stack. 

My work spans **low-level systems and kernel drivers**, **database architectures and enterprise software**, **autonomous AI agent engines (MCP & LangGraph)**, and **production full-stack SaaS platforms**. I like tackling complex, real-world problems from scratch—whether that involves simulating packet drops inside the Linux kernel, architecting dual-database ACID systems, or building sub-second spatial engines.

---

### 🖥️ Systems, OS Kernel & Database Architectures

#### [Linux Kernel E1000 Driver](https://github.com/Aryanban/e1000-driver-showcase) — In-Kernel Network Driver Packet Drop Simulation
*Systems architecture case study simulating probabilistic packet drop inside the Linux Kernel 6.12 Intel E1000 NIC driver.*
- Intercepted packet transmission at Layer 2/3 in `struct sk_buff`, silently freeing buffer memory via `dev_kfree_skb_any()` to trigger upstream TCP transport-layer recovery (Fast Retransmit, exponential RTO backoff).
- Benchmarked 100,000 transmitted packets across drop rates; proved that doubling host server receive buffers reduced `recv()` syscall invocations by ~50% due to stream-oriented socket coalescing (`buf[64]` vs `buf[128]`).
- **Stack:** `C` · `Linux Kernel 6.12` · `QEMU` · `Intel E1000 Driver` · `TCP/IP Networking`  
- [Systems Case Study](https://github.com/Aryanban/e1000-driver-showcase)

#### [Monopoly Digital Engine & Relational DBMS](https://github.com/Aryanban/monoply_dbms) — ACID Ledger & Multiplayer Backend
*Multiplayer board game engine and transactional backend built with Python, Flask, and MySQL 8.0.*
- Designed an **ACID-compliant relational schema** tracking double-entry balance ledgers, dynamic rent multipliers, player-to-player property trade negotiations, and mortgage states.
- Implemented transactional concurrency controls and a RESTful API managing live game state for up to 6 players across 40 spaces.
- Built an interactive client with Vanilla JavaScript, server polling synchronization, and CSS variable theming.
- **Stack:** `Python 3` · `Flask` · `MySQL 8.0` · `ACID Transactions` · `Relational DBMS` · `REST API`  
- [GitHub Repository](https://github.com/Aryanban/monoply_dbms)

#### [University Desktop ERP](https://github.com/Aryanban/university-erp) — Enterprise Management System
*Enterprise desktop ERP system built in Java Swing and Maven with dual-database transactional logic.*
- **Dual-Database Architecture:** Engineered isolated authentication database (`auth_schema.sql`) and academic operations database (`erp_schema.sql`) to separate security boundaries from operational records.
- Built **Role-Based Access Control (RBAC)** supporting Student, Instructor, and Administrator roles with course registration/drop rules, section filters, grade auditing, and CSV exports.
- **Stack:** `Java 17` · `Maven` · `MySQL` · `Swing UI` · `RBAC` · `Dual-Database Architecture`  
- [GitHub Repository](https://github.com/Aryanban/university-erp)

---

### 🗺️ Production Geospatial SaaS & Spatial Engines

#### [DholeraMap](https://dholeramap.com/) — Greenfield Smart City GIS & Statutory Due Diligence
*Cadastral GIS platform and automated statutory land verification engine for India's Dholera Special Investment Region (Tata Semiconductor corridor).*
- Digitized and georeferenced **3,600+ survey numbers across 22 villages** (18,161 cadastral parcels) with Town Planning demarcations and Satellite GIS overlays.
- Engineered a 1-click legal dossier compiler with SHA-256 provenance and instant QR verification (`/verify/[id]`), executing in-memory on the client to bypass serverless payload limits.
- Custom `DPB1` delta-int32 binary serialization cutting payload size by >80% with off-thread Web Worker raycasting.
- Built a programmatic SEO architecture with **3,700+ Google-indexed parcel pages** for organic zero-CAC discovery.
- Monetized with tiered recurring subscriptions (Razorpay auto-debit) and pay-per-report credits.
- **Stack:** `Next.js 15` · `TypeScript` · `MapLibre / Leaflet` · `pdf-lib` · `Supabase` · `Cloudflare Edge` · `Razorpay`  
- [Live Platform](https://dholeramap.com/) · [Architecture Case Study](https://github.com/Aryanban/dholeramap-showcase)

#### [PlotBook](https://plotbook.webforge.me/) — Real Estate Spatial Intelligence SaaS
*Geospatial intelligence platform digitizing Delhi Development Authority (DDA) layouts and circle rates.*
- Digitized **362+ official DDA town planning layout blueprints** across all 36 Rohini sectors.
- 60 FPS imperative camera engine manipulating direct CSS matrix transforms with zero React render overhead.
- Built **705 SSG static routes** pre-rendered via Next.js 16 Turbopack for instant sub-second page loads.
- Automated 2025 Delhi circle rate valuation engine and dynamic client-side PDF brochure generator.
- **Stack:** `Next.js 16` · `TypeScript` · `Turbopack` · `Leaflet` · `Supabase` · `Razorpay`  
- [Live Platform](https://plotbook.webforge.me/) · [Architecture Case Study](https://github.com/Aryanban/plotbook-showcase)

---

### 🤖 Autonomous AI Agents & Intelligent Pipelines

#### [LeadForge](https://github.com/Aryanban/leadforge) — Autonomous Lead Generation & Cold Outreach Platform
*Self-hosted lead scraping, multi-source contact enrichment, and cold outreach sequencer with native Model Context Protocol (MCP).*
- Native **MCP server** allowing AI agents to autonomously trigger scraping, verification, and CRM sequencing.
- Stealth Google Maps scraping via Playwright with browser fingerprint rotation and anti-bot evasions.
- Multi-source contact enrichment (Apollo-style email permutation, DNS MX/SMTP server validation).
- Multi-mailbox cold outreach sequencer with Twenty CRM synchronization and 0–100 AI lead scoring.
- **Stack:** `Python 3.11` · `FastAPI` · `Playwright` · `MCP SDK` · `Docker` · `Next.js 15`  
- [GitHub Repository](https://github.com/Aryanban/leadforge)

#### [SEOForge](https://github.com/Aryanban/seoforge) — Screaming Frog-Grade Autonomous SEO/AEO Crawler
*Local SEO crawler, site audit engine, and Answer Engine Optimization (AEO) scoring for Google AI Overviews and Perplexity.*
- Native **Model Context Protocol (MCP)** agent server enabling LLMs to audit websites, inspect sitemaps, and trigger IndexNow submissions.
- Fast local web cockpit built with Hono, Cheerio, and React 19.
- Programmatic issue diagnosis: Core Web Vitals, canonical graph loops, and schema entity validation.
- **Stack:** `TypeScript` · `Hono` · `MCP SDK` · `React 19` · `Cheerio` · `IndexNow`  
- [GitHub Repository](https://github.com/Aryanban/seoforge)

#### [EduGraph AI (pdf-ai-ml-bot)](https://github.com/Aryanban/pdf-ai-ml-bot) — Local Textbook Parsing & Conversational RAG
*Local intelligent tutoring and textbook Q&A assistant using retrieval-augmented generation.*
- Locally hosted language model inference via Ollama (Qwen 2.5:7B + BGE embeddings) with ChromaDB vector store.
- Multi-agent orchestration for grounded citation Q&A, automated quiz generation (MCQ/short answer), and misconception evaluation.
- **Stack:** `Python 3.12` · `Ollama` · `ChromaDB` · `Streamlit` · `RAG` · `Vector Embeddings`  
- [GitHub Repository](https://github.com/Aryanban/pdf-ai-ml-bot)

#### [TasteGuard](https://github.com/Aryanban/tasteguard) — Autonomous Cultural Intelligence & Brand Fit *(Active Prototype)*
*A 6-agent LangGraph swarm analyzing multi-dimensional cultural affinity and sponsorship fit for brands and artists.*
- Explores a **6-agent swarm** (Entity Resolver, Taste Profiler, Friction Analyst, Mitigation Strategist, Compliance Auditor, Synthesis Agent).
- Vector affinity decomposition across 7 cultural domains using Qloo API with quantitative zone classification ($|Δ| < 0.30$ Green, $0.30 \le |Δ| < 0.60$ Yellow, $\ge 0.60$ Red).
- Built with strict 0-PII compliance and contract-tested with Pytest.
- **Stack:** `Python 3.12` · `LangGraph` · `FastAPI` · `Qloo API` · `React 19` · `Pydantic v2`  
- [GitHub Repository](https://github.com/Aryanban/tasteguard)

---

### ⚡ Algorithmic Tooling & Automation

#### [PostForge](https://github.com/Aryanban/postforge) — Algorithm-Native Social Growth Engine
*Growth engine built by reverse-engineering Twitter's Heavy Ranker recommendation algorithm and X-AI ranking mechanics.*
- 7-point pre-flight anti-shadowban linter evaluating engagement multipliers and penalty weights before publishing.
- Zero-touch repository and domain ingestion to turn code updates into engaging technical narratives.
- Jitter scheduling to mimic human engagement patterns and protect sender reputation.
- **Stack:** `React 19` · `TypeScript` · `Tailwind CSS` · `Vite` · `Algorithms`  
- [GitHub Repository](https://github.com/Aryanban/postforge)

#### [Internship-Engine](https://github.com/Aryanban/internship-engine) — Autonomous Opportunity Pipeline & Typst Compiler
*Autonomous ATS crawler and job discovery pipeline with programmatic single-page resume compilation.*
- Automated ATS fetchers streaming live postings from Greenhouse, Lever, and Ashby JSON endpoints.
- Deterministic Gate 1 filter (<1ms) and SQLite caching for rapid opportunity triage.
- Programmatic Typst / RenderCV resume compiler with automated single-page length enforcement test gates.
- Trigger-event personalized outreach draft generator.
- **Stack:** `Python 3.11` · `Typer CLI` · `SQLite` · `Typst` · `RenderCV` · `Pytest`  
- [GitHub Repository](https://github.com/Aryanban/internship-engine)

---

### 🛠️ Open-Source Directory & Project Index

| Repository | Domain | Tech Stack | Focus Area |
| :--- | :--- | :--- | :--- |
| **[dholeramap-showcase](https://github.com/Aryanban/dholeramap-showcase)** | Geospatial SaaS | `Next.js 15` `TypeScript` `MapLibre` `pdf-lib` | Cadastral GIS Atlas, in-memory PDF synthesis, Satellite GIS |
| **[plotbook-showcase](https://github.com/Aryanban/plotbook-showcase)** | Geospatial SaaS | `Next.js 16` `TypeScript` `Turbopack` `Leaflet` | 362 digitized DDA layout plans, 60 FPS camera, broker CRM |
| **[e1000-driver-showcase](https://github.com/Aryanban/e1000-driver-showcase)** | Systems / Kernel | `C` `Linux Kernel 6.12` `QEMU` `Networking` | Intel E1000 NIC driver in-kernel packet drop simulation |
| **[monoply_dbms](https://github.com/Aryanban/monoply_dbms)** | DBMS / Full-Stack | `Python 3` `Flask` `MySQL 8.0` `ACID` | Multiplayer game engine with ACID relational ledger tracking |
| **[university-erp](https://github.com/Aryanban/university-erp)** | Enterprise Systems | `Java 17` `Maven` `MySQL` `Swing` | Desktop ERP with dual-database architecture & RBAC security |
| **[leadforge](https://github.com/Aryanban/leadforge)** | AI / Automation | `Python` `FastAPI` `MCP SDK` `Playwright` | Autonomous lead generation, SMTP verification, cold outreach |
| **[seoforge](https://github.com/Aryanban/seoforge)** | AI / Crawlers | `TypeScript` `Hono` `MCP SDK` `React 19` | Screaming Frog-grade SEO/AEO crawler & native MCP server |
| **[postforge](https://github.com/Aryanban/postforge)** | Algorithms / Web | `TypeScript` `React 19` `Tailwind` `Vite` | Heavy Ranker algorithm scoring & anti-shadowban linter |
| **[internship-engine](https://github.com/Aryanban/internship-engine)** | Automation / CLI | `Python 3.11` `Typst` `SQLite` `RenderCV` | ATS job crawler, Typst resume compiler & outreach generator |
| **[pdf-ai-ml-bot](https://github.com/Aryanban/pdf-ai-ml-bot)** | AI / RAG | `Python` `Ollama` `ChromaDB` `Streamlit` | Local textbook parsing & conversational multi-agent RAG |
| **[tasteguard](https://github.com/Aryanban/tasteguard)** | AI Swarms (WIP) | `Python 3.12` `LangGraph` `FastAPI` `React 19` | Cultural affinity vector decomposition & 6-agent swarm |
| **[webforge-portfolio-showcase](https://github.com/Aryanban/webforge-portfolio-showcase)** | Frontend Design | `React 19` `Vite` `Tailwind CSS v4` `Framer` | Personal portfolio platform at [webforge.me](https://www.webforge.me/) |

---

### ⚡ Tech Stack & Core Competencies

- **Systems & Languages:** C, Linux Kernel (Device Drivers, `sk_buff`, Sockets), Java 17, Python 3.12, TypeScript, SQL (MySQL 8.0, PostgreSQL, SQLite), Typst
- **Databases & Architecture:** ACID Transactions, Normalized Relational Modeling, Dual-Database Isolation, Supabase, Redis, Connection Pooling
- **AI Agents & Protocols:** Model Context Protocol (MCP Native), LangGraph, LangChain, ChromaDB, Ollama, Vector Embeddings, Playwright Automation
- **Frontend & Geospatial:** Next.js (App Router), React 19, MapLibre GL, Leaflet, Web Workers, Turbopack, Tailwind CSS v4, Framer Motion
- **Backend & Cloud:** FastAPI, Node.js, Express, Flask, Pydantic v2, RESTful APIs, Cloudflare (Edge/Cache), Docker, Vercel

---

### 🎓 Education & Campus Leadership

- **B.Tech in Computer Science and Design (CSD)** — **IIIT Delhi** (2024 – Present)
- **Organizing & Leadership:**
  - **Odyssey IIITD:** Managed tech registration workflows, server polling systems, and on-ground logistics for 10,000+ attendees.
  - **E-Summit IIITD:** Organized startup pitch cohorts, founder panels, and jury evaluation workflows.

---

### 📬 Connect

- **Portfolio:** [www.webforge.me](https://www.webforge.me/)
- **LinkedIn:** [linkedin.com/in/aryan-bansal-b29b69370](https://www.linkedin.com/in/aryan-bansal-b29b69370/)
- **Email:** [aryan24120@iiitd.ac.in](mailto:aryan24120@iiitd.ac.in) · [aryanbanc@gmail.com](mailto:aryanbanc@gmail.com)

<p align="center">
  <sub>© 2026 Aryan Bansal · Designed with care</sub>
</p>
