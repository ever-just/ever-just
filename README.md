# ever-just

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

### [facesmash-dev-portal](https://github.com/ever-just/facesmash-dev-portal)
**Developer portal for FaceSmash — API keys, billing, usage analytics, and team management.**

Developers sign up with face login (biometric + liveness detection), register applications, and get API credentials to integrate FaceSmash face auth into their products. Live at [developers.facesmash.app](https://developers.facesmash.app).

- Next.js 15, Drizzle ORM, PostgreSQL
- API key lifecycle management via Unkey (create, revoke, rate limit)
- Stripe subscriptions: Free, Pro ($29/mo), Enterprise
- Team RBAC (Owner/Member), activity audit log, transactional email via Resend

---

### [JUST-WORK](https://github.com/ever-just/JUST-WORK)
**Business directory and opportunity tracking platform for mid-market Minnesota companies ($100K–$100M ARR).**

React + TypeScript + Vite search and discovery tool built on a normalized dataset of 2,762 Minnesota companies. Designed for surfacing legitimate mid-market businesses for partnerships, outreach, and deal sourcing.

- 2,762 deduplicated company records from CSV source data
- Advanced search and filtering across the full dataset
- CSV-to-JSON conversion pipeline for keeping data current

---

### [project-fosh](https://github.com/ever-just/project-fosh)
**Chrome extension for secure, local API key management.**

Stores API keys in Chrome's secure local storage — no cloud, no sync, no external requests. Supports add, edit, delete, search, one-click copy, and masked display. Built for developers who work with multiple services and want keys off their clipboard and out of their shell history.

---

### [bid-bot-buddy](https://github.com/ever-just/bid-bot-buddy)
**AI-powered RFP automation platform for government contracts.**

Paste a public RFP URL and the system extracts scope, requirements, and deadlines; researches historical contract data and pricing trends; identifies and contacts relevant vendors; estimates pricing and profitability; and generates a complete proposal document. Built initially for Minnesota state contracts.

- Flask + Python backend, React + shadcn/ui frontend
- Playwright for universal government procurement site scraping
- AI agents handle each stage of the proposal pipeline end-to-end

---

