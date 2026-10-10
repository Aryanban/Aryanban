# Aryan Bansal

<p align="left">
  <b>Software Engineer & Builder</b> · IIIT Delhi (CS &amp; Design '28)<br/>
  Building production geospatial platforms, autonomous AI systems, and developer tools.
</p>

<p align="left">
  <a href="https://www.webforge.me/"><img src="https://img.shields.io/badge/Portfolio-webforge.me-6366F1?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://dholeramap.com/"><img src="https://img.shields.io/badge/DholeraMap-Live%20GIS-0284C7?style=flat-square&logo=mapbox&logoColor=white" alt="DholeraMap" /></a>
  <a href="https://plotbook.webforge.me/"><img src="https://img.shields.io/badge/PlotBook-Live%20SaaS-059669?style=flat-square&logo=googlemaps&logoColor=white" alt="PlotBook" /></a>
  <a href="https://github.com/Aryanban/tasteguard"><img src="https://img.shields.io/badge/TasteGuard-AI%20Swarm-8B5CF6?style=flat-square&logo=openai&logoColor=white" alt="TasteGuard" /></a>
  <a href="https://www.linkedin.com/in/aryan-bansal-b29b69370/"><img src="https://img.shields.io/badge/LinkedIn-Aryan_Bansal-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:aryan24120@iiitd.ac.in"><img src="https://img.shields.io/badge/Email-aryan24120-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

### About Me

I am a 3rd-year Computer Science & Design undergraduate at **IIIT Delhi**. I like taking messy, complex real-world problems and turning them into fast, reliable software products with real users. 

My work spans **geospatial intelligence platforms**, **autonomous multi-agent swarms (LangGraph, MCP)**, and **systems engineering**. When I build, I focus on the entire loop: architecture, performance bottlenecks, user experience, and distribution.

---

### 🚀 Selected Projects

#### [DholeraMap](https://dholeramap.com/) — Greenfield Smart City GIS & Due-Diligence Engine
*Cadastral GIS platform and automated statutory land verification engine for India's Dholera Special Investment Region (Tata Semiconductor corridor).*
- Digitized and georeferenced **3,600+ survey numbers across 22 villages** with satellite GIS overlays and Town Planning demarcations.
- Engineered a 1-click legal dossier compiler with SHA-256 provenance and instant QR verification (`/verify/[id]`), executing in-memory on the client to bypass serverless payload limits.
- Built a programmatic SEO architecture with **3,700+ Google-indexed parcel pages** for organic zero-CAC discovery.
- Monetized with tiered recurring subscriptions (Razorpay auto-debit) and pay-per-report credits.
- **Stack:** `Next.js 15` · `TypeScript` · `MapLibre / Leaflet` · `pdf-lib` · `Supabase` · `Cloudflare Edge` · `Razorpay`  
- [Live App](https://dholeramap.com/) · [Architecture Case Study](https://github.com/Aryanban/dholeramap-showcase)

#### [TasteGuard](https://github.com/Aryanban/tasteguard) — Autonomous Cultural Intelligence & Brand Fit Engine
*A 6-agent LangGraph swarm analyzing multi-dimensional cultural affinity and sponsorship risk for brands and artists.*
- Orchestrates **6 specialized agents** (Entity Resolution, Taste Profiling, Friction Analysis, Mitigation Strategy, Compliance, Synthesis) with structured state handoffs.
- Performs vector affinity decomposition across 7 cultural domains using Qloo API with mathematical zone classification ($|Δ| < 0.30$ Green, $0.30 \le |Δ| < 0.60$ Yellow, $\ge 0.60$ Red).
- Built with strict 0-PII compliance, contract-tested via Pytest, with a FastAPI backend and interactive React 19 dashboard.
- **Stack:** `Python 3.12` · `LangGraph` · `LangChain` · `FastAPI` · `Qloo API` · `React 19` · `Pydantic v2` · `Pytest`  
- [GitHub Repository](https://github.com/Aryanban/tasteguard)

#### [PlotBook](https://plotbook.webforge.me/) — Real Estate Spatial Intelligence SaaS
*Geospatial intelligence platform digitizing Delhi Development Authority (DDA) layouts and circle rates.*
- Digitized **362+ official DDA town planning layout blueprints** across all 36 Rohini sectors.
- 60 FPS imperative camera engine manipulating direct CSS matrix transforms with zero React render overhead.
- Built 705 SSG static routes pre-rendered via Next.js 16 Turbopack for instant page loads.
- **Stack:** `Next.js 16` · `TypeScript` · `Turbopack` · `Leaflet` · `Supabase` · `Razorpay`  
- [Live App](https://plotbook.webforge.me/) · [Architecture Case Study](https://github.com/Aryanban/plotbook-showcase)

#### [LeadForge](https://github.com/Aryanban/leadforge) — Autonomous Lead Generation & Outreach Engine
*Self-hosted lead scraping, multi-source contact enrichment, and cold outreach sequencer with native Model Context Protocol (MCP).*
- Native **MCP server** allowing AI agents to autonomously trigger scraping, verification, and CRM sequencing.
- Stealth Google Maps scraping via Playwright with fingerprint rotation, Apollo-style email permutation, and live SMTP MX validation.
- **Stack:** `Python 3.11` · `FastAPI` · `Playwright` · `MCP SDK` · `Docker` · `Next.js 15`  
- [GitHub Repository](https://github.com/Aryanban/leadforge)

#### [SEOForge](https://github.com/Aryanban/seoforge) — Autonomous SEO & Answer Engine Optimization (AEO)
*Local SEO crawler, site audit engine, and Answer Engine Optimization scoring for Google AI Overviews and Perplexity.*
- Native **MCP server** enabling autonomous website crawling, sitemap inspection, and IndexNow protocol submission.
- Fast local web cockpit built with Hono, Cheerio, and React 19.
- **Stack:** `TypeScript` · `Hono` · `MCP SDK` · `React 19` · `Cheerio` · `IndexNow`  
- [GitHub Repository](https://github.com/Aryanban/seoforge)

#### [PostForge](https://github.com/Aryanban/postforge) — Algorithm-Native Content Engine
*Growth engine built by reverse-engineering Twitter's Heavy Ranker recommendation algorithm and X-AI ranking mechanics.*
- 7-point pre-flight anti-shadowban linter evaluating engagement multipliers and penalty weights before publishing.
- Zero-touch repository ingestion to turn code updates into engaging technical narratives.
- **Stack:** `React 19` · `TypeScript` · `Tailwind CSS` · `Vite` · `Algorithms`  
- [GitHub Repository](https://github.com/Aryanban/postforge)

---

### 🛠️ More Open Source & Systems Work

| Project | Stack | Overview |
| :--- | :--- | :--- |
| **[internship-engine](https://github.com/Aryanban/internship-engine)** | `Python 3.11` `Typst` `SQLite` | Autonomous ATS crawler (Greenhouse/Lever/Ashby) with programmatic Typst single-page resume compilation and personalized outreach drafting. |
| **[monoply_dbms](https://github.com/Aryanban/monoply_dbms)** | `Python` `Flask` `MySQL 8.0` | Multiplayer Monopoly engine with an ACID-compliant relational ledger tracking player transactions, property trades, and mortgages. |
| **[webforge-portfolio](https://github.com/Aryanban/webforge-portfolio-showcase)** | `React 19` `Vite` `Framer` | Personal portfolio platform at [webforge.me](https://www.webforge.me/) featuring interactive terminal and dark glassmorphic design. |
| **[university-erp](https://github.com/Aryanban/university-erp)** | `Java` `Swing` `MySQL` | Desktop ERP system with role-based access control (RBAC) and dual-database transactional integrity. |
| **[pdf-ai-ml-bot](https://github.com/Aryanban/pdf-ai-ml-bot)** | `Python` `NLP` `Embeddings` | Conversational document Q&A pipeline for dense academic and legal PDFs. |

---

### ⚡ Tech Stack & Tools

- **Languages:** TypeScript, Python, JavaScript, Java, C/C++, SQL, Typst
- **AI Agents & LLMs:** LangGraph (Multi-Agent Swarms), Model Context Protocol (MCP), LangChain, Vector Embeddings, Playwright Automation
- **Frontend & UI:** Next.js (App Router), React 19, Tailwind CSS v4, Framer Motion, Hono
- **Backend & Systems:** FastAPI, Node.js, Express, Flask, Pydantic v2, REST APIs
- **Databases & Cloud:** PostgreSQL, Supabase, MySQL 8.0, SQLite, Cloudflare (Edge/Cache), Vercel, Docker, Git

---

### 🎓 Education & Campus Leadership

- **B.Tech in Computer Science and Design (CSD)** — **IIIT Delhi** (2024 – Present)
- **Organizing & Leadership:**
  - **Odyssey IIITD:** Managed tech registration workflows and on-ground logistics for 10,000+ attendees.
  - **E-Summit IIITD:** Organized startup pitch cohorts, founder panels, and jury workflows.

---

### 📬 Connect

- **Portfolio:** [www.webforge.me](https://www.webforge.me/)
- **LinkedIn:** [linkedin.com/in/aryan-bansal-b29b69370](https://www.linkedin.com/in/aryan-bansal-b29b69370/)
- **Email:** [aryan24120@iiitd.ac.in](mailto:aryan24120@iiitd.ac.in) · [aryanbanc@gmail.com](mailto:aryanbanc@gmail.com)

<p align="center">
  <sub>© 2026 Aryan Bansal · Designed with care</sub>
</p>
