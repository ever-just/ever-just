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

### [ww.everjust.app](https://github.com/ever-just/ww.everjust.app)
**Self-hosted, multi-tenant SaaS platform built on a debranded Odoo 19 base.**

Organizations sign up, pay via Stripe, and get an isolated workspace at `<org>.everjust.app`. Each tenant gets its own PostgreSQL database. Debranding and theming are done through add-on modules — not a core fork — so the platform stays upgradeable.

- Nginx wildcard SSL + `dbfilter` subdomain routing
- Stripe billing: $100/mo base (up to 5 users) + $15/user overage
- `everjust_brand` module replaces every upstream touchpoint at install
- `debrand_check.sh` scans live tenants for leaks

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

## Contact

weldon@everjust.co · [everjust.org](https://everjust.org)
