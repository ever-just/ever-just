# ever-just

**Weldon Makori** — building AI-native tools, self-hosted platforms, and research infrastructure.

---

## Active Repos

### [textmyagent-desktop](https://github.com/ever-just/textmyagent-desktop)
**AI executive assistant for macOS via iMessage. Runs entirely on-device — no cloud, no API keys.**

Electron app powered by Google Gemma 4 E4B via `node-llama-cpp`. Reads and responds to iMessages directly from `Messages.app`. All data stored locally in SQLite. Includes a Next.js dashboard for monitoring conversations, memory, reminders, automation triggers, and security controls.

- macOS 12+, Apple Silicon and Intel
- 155 passing tests
- GPU layer offloading for fast inference on M-series chips
- Contact name resolution via macOS Contacts

---

### [TextMyAgent](https://github.com/ever-just/TextMyAgent)
**The original TextMyAgent service — Claude-powered executive assistant accessible via iMessage/SMS.**

Built on BlueBubbles for native iMessage routing. The assistant (named Grace) maintains long-term memory across conversations, manages usage budgets and rate limits, and replies in real time. Everything runs on your own infrastructure — no vendor lock-in, no external conversation storage.

- Claude-powered with persistent per-user memory
- BlueBubbles integration for delivery receipts, read states, and typing indicators
- Self-hosted: credentials and conversations never leave your hardware
- Flutter mobile companion app

---

### [ww.everjust.app](https://github.com/ever-just/ww.everjust.app)
**Self-hosted, multi-tenant SaaS platform. Organizations get an isolated workspace at `<org>.everjust.app`.**

Each tenant gets its own PostgreSQL database, fully branded as EVERJUST.APP. The control plane (FastAPI) handles signup, Stripe billing, and automated provisioning. Nginx wildcard SSL routes each subdomain to its tenant database at the infrastructure level.

- Stripe billing: $100/mo base (up to 5 users) + $15/user overage
- Automated provisioning on payment success via Stripe webhook
- Per-tenant database isolation — no shared state between orgs
- `debrand_check.sh` scans live tenants for upstream reference leaks

---

### [agentskills](https://github.com/ever-just/agentskills)
**Structured `SKILL.md` files that give AI coding agents deep expertise in specific tools and workflows.**

Instead of relying on generic training data, each skill file gives an agent step-by-step instructions, code templates, decision trees, pitfall lists, and combination patterns. Works with Windsurf, Claude Code, Cursor, or any agent that can read a file.

Skill categories:
- **Visual asset creation** — Remotion, Motion Canvas, Manim, GSAP, Slidev, D3.js, Lottie, MoviePy, Framer Motion
- **Platform operations** — deployment testing, email processing, UI/UX audit, MongoDB schema audit, Sentry instrumentation
- **Research & due diligence** — legal/reputation research using only free public sources
- **Writing & marketing** — 19 sub-skills covering prose quality, copywriting, content strategy, doc export

*Maintained in coordination with [Custom Agents](https://customagents.io).*

---

### [twincitiesstartupweek](https://github.com/ever-just/twincitiesstartupweek)
**OSINT research archive and operating repo for Twin Cities Startup Week 2026.**

12 years of TCSW history (2014–2026): sponsor database, 600+ speaker records, session data from 2018–2025, attendance and financials, press coverage by year and publication, and Wayback Machine archives. Active planning for TCSW 2026 (September 14–18, Minneapolis + St. Paul) lives alongside the research. The event management platform runs at [tcsw.everjust.app](https://tcsw.everjust.app).

Key files: `master-findings-report.md`, `sponsors-database.csv`, `speakers-database.csv`, `all-sessions.csv`

---

### [status](https://github.com/ever-just/status)
**Uptime monitor and status page for Custom Agents services.**

Powered by Upptime. Tracks availability and response times for Custom Agents infrastructure. Live at [status.customagents.io](https://status.customagents.io).

---

### [facesmash-dev-portal](https://github.com/ever-just/facesmash-dev-portal)
**Developer portal for FaceSmash — API keys, billing, usage analytics, and team management.**

Developers sign up with face login (biometric + liveness detection), register applications, and get API credentials to integrate FaceSmash face auth into their products. Live at [developers.facesmash.app](https://developers.facesmash.app).

- Next.js 15, Drizzle ORM, PostgreSQL
- API key lifecycle management via Unkey (create, revoke, rate limit)
- Stripe subscriptions: Free, Pro ($29/mo), Enterprise
- Team RBAC (Owner/Member), activity audit log, transactional email via Resend

---

### [weldonmakori.com](https://github.com/ever-just/weldonmakori.com)
**Personal website — live at [weldonmakori.com](https://weldonmakori.com).**

Built with Next.js 16 (App Router), TypeScript, Tailwind CSS 4, and Framer Motion. Covers career history, education (UST + Normandale), and ventures. Data-driven: work history and education records are structured JSON, not hardcoded markup.

---

### [OSINDO](https://github.com/ever-just/OSINDO)
**Landing page and customer portal for Osindo Mechanical Services — HVAC, auto, and mechanical repair in the Twin Cities.**

Static HTML/CSS/JS site deployed on Netlify. DNS managed programmatically via GoDaddy API. Primary CTA routes to the Assembly customer portal for scheduling and service requests.

---

### [gasolina.ai](https://github.com/ever-just/gasolina.ai)
**AI talent agency for creators — brand deal management from inbox to invoice.**

Research and product architecture for an AI agent (Emma) that sits between creators and brands, handling inbound email triage, negotiation, contract review, invoicing, and payment follow-up at a lower commission than traditional agencies. Creators get text-based updates and approve or decline deals in one reply — the agent handles everything else.

- Lower commission model: earns only when the creator earns
- Real-time rate intelligence drawn from deal data across creators
- 24/7 inbox coverage: Emma responds to brand outreach at any hour
- Manages full deal lifecycle: outreach → negotiation → contract → payment

---

## Contact

weldon@everjust.co · [everjust.org](https://everjust.org)
