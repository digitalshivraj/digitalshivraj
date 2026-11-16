# Shivraj Chincholkar

**AI Automation & GTM Engineer** · Pune, India · [LinkedIn](https://linkedin.com/in/digitalshivraj)

I build multi-agent AI systems and growth automation — end to end, in production. 10+ years running B2B revenue funnels, now designing and shipping the AI systems that run them.

---

## What I Build

### 🛡️ Streakstone — Lead Qualification Firewall & Verified Appointment Engine *(Private — commercial)*
*Live · formerly Kasauti*

A multi-tenant platform for businesses that run lead ads: every incoming lead is qualified before it reaches the sales team, and appointments are verified before they are counted.

- **Built around real cost per real lead**, replacing the ad platform's count of every submitted form
- **AI voice agent** calls and qualifies leads; self-serve onboarding lets one operator run many client accounts
- **Stack:** Next.js · Supabase (Postgres + RLS) · Vercel · AI voice agent · WhatsApp API

### 🪪 Parichay — Government ID Card Platform *(Private — client work)*

Data collection and card generation platform for a state school programme: 420+ schools across 20 districts, about 469,000 student records, around 70 field agents.

- **AI quality-check agent** on Claude vision for student photos, with a human review queue
- **Print pipeline** that turns each school into one print-ready PDF pack
- **Stack:** Next.js · Supabase · Vercel · Claude vision · n8n

### 🚚 Mahima One — Franchise Logistics Platform *(Private — client work)*

Franchise booking and head-office platform for a packers and movers company: 32 screens covering booking, consignment lifecycle, exceptions, trips, payments, rate cards, public tracking and partner onboarding.

- **Tenant isolation** between franchises with Row-Level Security; deployed with zero open ports
- **Stack:** Next.js · Postgres (Docker) · Cloudflare Tunnel

### 🚀 [OutreachOS](https://github.com/digitalshivraj/OutreachOS) — Multi-Agent Compliance-Gated Outreach Engine
*Built for the Band of Agents Hackathon (June 2026) · [Live Demo](https://outreachos-e9mgyjq68ymhz3ubddqxtz.streamlit.app/)*

An open-source AI outreach engine where agents review and reject each other's work before anything ships — not a linear pipeline, a deliberation loop.

- **4 coordinated agents on Band:** Researcher (prospect/company context) → Copywriter (drafts personalized outreach) → Compliance Reviewer (approves, rejects with reasons, or escalates to a human) → Human Approval (final sign-off on flagged cases)
- **The core mechanic:** Compliance Reviewer can send work *backward* to the Copywriter for revision — agents coordinating and disagreeing, not just executing in sequence
- **Stack:** Band SDK · Python · Claude API (AI/ML API) · Featherless AI (open-source inference) · Next.js demo UI · Vercel
- **Why it exists:** I've run real cold-outreach campaigns. Bad AI-written outreach destroys sender reputation faster than no outreach at all — this system makes that failure mode structurally hard to ship.

### 🤖 [Headliner](https://github.com/digitalshivraj/headliner) — 9-Agent B2B Outreach Automation *(Private — commercial)*
A production multi-agent pipeline running real cold-outreach campaigns for paid editorial placements, at $999–$1,200 per placement.

- **9 coordinated agents:** Theme Mapper → Prospect Researcher (Apollo/LinkedIn enrichment) → Fit Scorer (7/10 gate) → Personalizer (trained voice corpus) → Reply Classifier → Follow-up Composer → Compliance Monitor → Scheduler → Sheets Sync / Telegram Control Hub
- **Stack:** n8n · Supabase Postgres · Instantly.ai · Claude API · Google Sheets API · Telegram Bot API
- **Design principle:** Human sign-off before every send. OutreachOS (above) is the open-source distillation of this system's core architecture — built fresh, without exposing the commercial pipeline or client data.

### 🎓 Astra Global *(Private)* — AI-Assisted Early Childhood Coaching Platform
*[Live Demo](https://astraglobal.vercel.app)*

Full-stack coaching dashboard built and deployed solo in 6 weeks.

- **48 curriculum units** across two learning levels with progress loops and celebration mechanics
- **Stack:** Next.js · Supabase (Postgres + RLS) · Vercel · TypeScript
- Owned everything: schema design, 8 migrations, seeding pipeline, auth, RLS hardening, analytics, production deployment

### 💊 CareSync *(Private)* — Senior Medication & Health Companion App
*[Live Demo](https://caresync-f6f24.web.app)*

A premium, senior-friendly medication and health companion app built solo, designed for accessibility-first use by elderly users and their caregivers.

- **Dual-role context switcher** — a single account seamlessly toggles between senior and caregiver views, each with its own permissions and UI
- **Voice vitals logging** — hands-free health data entry for users who struggle with small-screen typing
- **Dynamic pill rendering** with low-stock warnings, built for real medication-adherence workflows, not a generic to-do list
- **Accessibility-first design** — large touch targets, high-contrast modes, and voice-first interaction patterns throughout
- **Stack:** JavaScript · Firebase (Hosting + backend)

### 📊 [MIDAS](https://github.com/digitalshivraj/MIDAS) — Algorithmic Trading System (XAUUSD)
Institutional-style ensemble trading system: Kalman Filter, Discrete Wavelet Transform, Hidden Markov Model regime detection, Hurst Exponent, and order-flow analysis feeding an XGBoost gatekeeper with Kelly Criterion position sizing.

- **Stack:** Python · XGBoost · statsmodels · MetaTrader5 API
- Part of a closed research arc (MIDAS → APEX → ARIA) — see Background below.

---

## More Systems I've Built

Most of my repositories are private because they are client work or commercial products. These are the ones not shown above. Happy to walk through any of them on a call.

| Project | What it does | Stack | Status |
|---|---|---|---|
| **Citeloop** | Multi-tenant SEO, AEO and GEO platform: site audit engine with 34 checks, AI citation radar across Claude, OpenAI and Perplexity, and a client portal | Python · Supabase (RLS) · Next.js · CI eval gate | Built; first full scan covered 442 pages |
| **SmartDine** | QR dine-in and takeaway ordering for restaurants: table menu, parcel tokens, kitchen order tickets, counter voice announcements, UPI billing, owner reports | Vercel · Supabase | Live; first restaurants onboarding |
| **ZeroBaki** | B2B dues recovery agent for small firms | Supabase · Claude API | In build |
| **Anudan Sarathi** | Subsidy application tracking for an agri-equipment dealer: five access roles, stage-by-stage farmer tracking, Marathi interface | Vercel · Supabase | Built for a client |
| **PropDesk** | Prop firm management CRM with trader, admin and support portals | Vercel | Client demo live |
| **Campaign management system** | War-room dashboard with booth-level tracking, plus a field worker mobile app with role-based access, in Marathi and English | Vercel | Client demo live |
| **Devdoot** | Doctor booking and patient waiting-queue platform | Supabase | In build |
| **JanSeva** | Citizen-service CRM for an elected representative's office | Supabase | Built |
| **MT5 Relay** | Bridge that sends TradingView signals to MetaTrader 5 | Python | In build |
| **PDF Editor** | Edits PDF text while keeping the original font, with bulk find and replace | FastAPI · PyMuPDF | Built |

---

## Skills

**AI & Agents**
`Multi-Agent Systems` `Agent Orchestration` `LLM Integration (Claude API)` `Prompt Engineering` `Human-in-the-Loop Guardrails` `Agent Memory & State Design` `Band SDK` `n8n`

**Backend & Data**
`Python` `Postgres` `Supabase` `REST APIs` `Webhooks` `Google Sheets API` `SQL`

**Frontend & Deployment**
`Next.js` `React` `TypeScript` `JavaScript` `Vercel` `Git`

**GTM & Growth**
`Cold Outreach Systems` `Email Deliverability (SPF/DKIM/DMARC)` `Google Ads` `Meta Ads` `LinkedIn Ads` `GA4` `SEO/GEO/AEO` `Funnel Analytics` `HubSpot` `CRM`

---

## Background

10+ years across digital marketing roles, including 4+ years driving revenue through paid and organic channels for a multi-city aesthetics clinic chain (11 centers across India + Dubai) — Google/Meta/LinkedIn ads, SEO/GEO, email infrastructure, funnel analytics. I understand the GTM funnel from lead acquisition to booked revenue, and now build the AI systems that automate it.

Earlier, I built and formally closed a three-phase algorithmic trading research program on XAUUSD (gold spot), each phase testing a different hypothesis about whether short-term price direction is predictable:

- **MIDAS** — a 5-model mathematical ensemble: Kalman Filter (trend extraction), Discrete Wavelet Transform (multi-resolution signal decomposition), Hidden Markov Model (regime detection), Hurst Exponent (trend-vs-mean-reversion classification), and an Order Flow Analyzer, fed into an XGBoost gatekeeper for trade filtering with Kelly Criterion position sizing.
- **APEX** — a Transformer-based forecaster predicting short-horizon price movement directly from sequence data. Diagnosed and fixed a critical failure mode here: the model was trading on randomly-initialized weights due to a checkpoint load failure, and separately, MSE loss on a near-zero-mean target was incentivizing the model to always predict near-zero (the "safe" loss-minimizing answer, not a useful signal).
- **ARIA** — a regime-adaptive reinforcement learning system using PPO agents conditioned on detected market regime.

I ran forensic walk-forward backtesting against realistic transaction costs (spread, slippage, commission) across 5 folds. Result: directional AUC of 0.5022 — statistically indistinguishable from a coin flip — and negative net return per trade after friction in all 5 folds. I formally closed the program rather than keep iterating on reward functions or model architecture once the underlying premise (predictable short-term direction) failed to hold under honest evaluation. I treat the kill decision as seriously as the build decision.

---

## Currently

- 🚀 Building **Streakstone**, a lead qualification platform for businesses that run lead ads
- 🚀 Shipped **OutreachOS** for the Band of Agents Hackathon (June 12–19, 2026)
- 🎯 Open to **GTM Engineer / AI Automation Specialist** roles — India-based or remote globally
- 📬 [chincholkar.shivraj1@gmail.com](mailto:chincholkar.shivraj1@gmail.com)
