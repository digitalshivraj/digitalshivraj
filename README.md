# Shivraj Chincholkar

**AI Automation & GTM Engineer** · Pune, India · [LinkedIn](https://linkedin.com/in/digitalshivraj)

I build multi-agent AI systems and growth automation — end to end, in production. 9+ years running B2B revenue funnels, now designing and shipping the AI systems that run them.

---

## What I Build

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

### 🎓 [Astra Global](https://github.com/digitalshivraj/Astra-Global) — AI-Assisted Early Childhood Coaching Platform
*[Live Demo](https://astraglobal.vercel.app)*

Full-stack coaching dashboard built and deployed solo in 6 weeks.

- **48 curriculum units** across two learning levels with progress loops and celebration mechanics
- **Stack:** Next.js · Supabase (Postgres + RLS) · Vercel · TypeScript
- Owned everything: schema design, 8 migrations, seeding pipeline, auth, RLS hardening, analytics, production deployment

### 📊 [MIDAS](https://github.com/digitalshivraj/MIDAS) — Algorithmic Trading System (XAUUSD)
Institutional-style ensemble trading system: Kalman Filter, Discrete Wavelet Transform, Hidden Markov Model regime detection, Hurst Exponent, and order-flow analysis feeding an XGBoost gatekeeper with Kelly Criterion position sizing.

- **Stack:** Python · XGBoost · statsmodels · MetaTrader5 API
- Part of a closed research arc (MIDAS → APEX → ARIA) — see Background below.

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

9+ years across digital marketing roles, including 4+ years driving revenue through paid and organic channels for a multi-city aesthetics clinic chain (11 centers across India + Dubai) — Google/Meta/LinkedIn ads, SEO/GEO, email infrastructure, funnel analytics. I understand the GTM funnel from lead acquisition to booked revenue, and now build the AI systems that automate it.

Earlier, I built and formally closed a three-phase algorithmic trading research program on XAUUSD (gold spot), each phase testing a different hypothesis about whether short-term price direction is predictable:

- **MIDAS** — a 5-model mathematical ensemble: Kalman Filter (trend extraction), Discrete Wavelet Transform (multi-resolution signal decomposition), Hidden Markov Model (regime detection), Hurst Exponent (trend-vs-mean-reversion classification), and an Order Flow Analyzer, fed into an XGBoost gatekeeper for trade filtering with Kelly Criterion position sizing.
- **APEX** — a Transformer-based forecaster predicting short-horizon price movement directly from sequence data. Diagnosed and fixed a critical failure mode here: the model was trading on randomly-initialized weights due to a checkpoint load failure, and separately, MSE loss on a near-zero-mean target was incentivizing the model to always predict near-zero (the "safe" loss-minimizing answer, not a useful signal).
- **ARIA** — a regime-adaptive reinforcement learning system using PPO agents conditioned on detected market regime.

I ran forensic walk-forward backtesting against realistic transaction costs (spread, slippage, commission) across 5 folds. Result: directional AUC of 0.5022 — statistically indistinguishable from a coin flip — and negative net return per trade after friction in all 5 folds. I formally closed the program rather than keep iterating on reward functions or model architecture once the underlying premise (predictable short-term direction) failed to hold under honest evaluation. I treat the kill decision as seriously as the build decision.

---

## Currently

- 🚀 Shipped **OutreachOS** for the Band of Agents Hackathon (June 12–19, 2026)
- 🎯 Open to **GTM Engineer / AI Automation Specialist** roles — India-based or remote globally
- 📬 [chincholkar.shivraj1@gmail.com](mailto:chincholkar.shivraj1@gmail.com)
