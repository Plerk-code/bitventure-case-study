theme: Titillium, 1
footer: Benjamin Hinson | Executive Head: Software Development
slidenumbers: true
autoscale: true
footer-style: #999999
header-strong: #FFFFFF
text-strong: #FFFFFF

---

![](https://images.pexels.com/photos/29327972/pexels-photo-29327972.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] The R500M Question
## Can ABC's engineering organisation deliver what the board has promised?

**Benjamin Hinson** · March 2026

^
Good morning. The board has approved expansion into two new African markets, a new real-time payments product, and a full cloud migration — all on top of a R500M revenue target. The question isn't whether these are the right bets. It's whether the engineering organisation can deliver them. Right now, the honest answer is: not yet. But I've been here before. I've turned "not yet" into "done" at ABSA, Discovery, AXA, John Lewis, and five other organisations. Let me show you how I'd do it here.

---

# The Business Case for This Conversation

The board has approved three growth bets. Each depends on engineering delivery:

| Board Bet | Revenue at Stake | Engineering Dependency |
|-----------|-----------------|----------------------|
| 2 new African markets | R80–120M new revenue | Multi-tenant architecture, data residency, POPIA/NDPR compliance |
| Real-time payments product | R40–60M new revenue | Event-driven microservices, partner API integration |
| Cloud-native migration | R15–25M annual savings | Strangler fig migration, Kubernetes, IaC |

**The risk:** Launching these on today's platform — 62% on-time delivery, 18 critical bugs/month, 6–10 hour recovery times — doesn't just risk failure. It risks losing the existing business while chasing the new one.

**The opportunity:** Fix the foundation first, and all three bets become achievable within 24 months.

^
I'm framing this as a business problem, not a technology problem, because that's what it is. The board didn't approve a cloud migration for its own sake — they approved revenue growth that requires cloud migration. Every engineering decision I'll present today maps directly to one of these three bets. Source for revenue estimates: SA fintech growth projections (USD 3.7–14.9B by 2033, ZAR 2.9T card transactions in 2025), sized proportionally to ABC's market position.

---

# The Cost of Doing Nothing

If we don't act, here's what the next 12 months look like:

**Partner risk** — Banking partner is already threatening penalties. One more major outage could trigger SLA exit clauses. Estimated exposure: **R20–50M** in lost partnership revenue.

**Regulatory risk** — POPIA data localisation enforcement in 2026. Without automated compliance and data residency architecture, we risk **regulatory action** that blocks market entry.

**Talent risk** — 18% attrition means we lose 2 of our 10 engineers this year. Each senior replacement costs 6–9 months of productivity. We're not just losing people — we're losing **institutional knowledge** that can't be replaced.

**Competitive risk** — 92% of SA fintechs are already cloud-native and API-first. Every month we delay, competitors widen the gap.

*Inaction is not a neutral position. It's a decision to accept these outcomes.*

^
This slide exists because EXCO needs to feel the urgency before I present the solution. Most transformation pitches start with "here's my plan." I start with "here's what happens if we don't." At Discovery, I used this exact framing with Manulife leadership to secure a R30M+ technology investment. The numbers focus attention.

---

# Diagnosis: A Systems Problem, Not a Talent Problem

| Metric | ABC Today | DORA Elite | Delta | Source |
|--------|-----------|-----------|-------|--------|
| On-time delivery | **62%** | 85%+ | +23% | Standish CHAOS |
| Critical bugs/month | **18** | <5 | -13 | DORA CFR |
| MTTR | **6–10 hrs** | <1 hr | -5 to 9 hrs | DORA 2024 |
| Deploy frequency | **2–3 weeks** | Daily | ~15x | DORA 2024 |
| Test automation | **~45%** | 75%+ | +30% | Fowler/Google |
| Cloud migration | **25%** | 100% | +75% | Board mandate |
| Attrition | **18%** | <10% | -8%+ | Mercer SA |
| Support tickets | **+40% YoY** | Declining | Lagging | Symptom |

**Root causes:** Structural debt (silos, handoffs) · Process debt (inconsistent reviews, partial QA) · Architectural debt (monolith at 75%) · Cultural debt (no path to mastery, purpose, or autonomy)

**The good news:** Revenue is up, customers are growing, partnerships are expanding. The fundamentals are strong. This is fixable.

^
I'm combining the Vital Signs and Root Cause into one slide because the panel doesn't need two slides to understand the problem. The delta column and source column are there for when someone asks "where does 85% come from?" — I can answer immediately without fumbling. At ABSA, I inherited the same pattern: siloed teams, no DevOps culture, manual processes. Within 12 months we halved cycle times. The fix isn't heroism — it's system design. Conway's Law tells us organisations ship their org chart. Silos create silos in the code.

---

# My Approach: Stabilise · Scale · Accelerate

| Phase | Timeline | Focus | Business Outcome |
|-------|----------|-------|-----------------|
| **Stabilise** | Months 1–6 | Delivery predictability, incident response, quality gates, partner confidence | COO gets reliability, CRO gets controls, partner stays |
| **Scale** | Months 4–18 | Cloud migration, API-first platform, team 10→25+, data platform | Architecture supports all three board bets |
| **Accelerate** | Months 12–24 | New markets live, real-time payments, AI/ML differentiation | CEO gets growth, CPO gets innovation |

These overlap deliberately. Parallel tracks, managed risk — not sequential waterfall.

**The key constraint:** You can't do everything at once with 10 engineers. My job is to sequence ruthlessly so the board's ambitions land on a foundation that can support them.

^
Notice the "Business Outcome" column — every phase is framed in terms of what the C-suite stakeholder gets, not what engineering does. At AXA, I ran shadow deployments at 20% traffic while stabilising the main system. At Barclays ABSA, I built a multi-year capability roadmap for digital banking across Africa. The lesson: sequence on platform readiness, not market ambition alone.

---

# 90 Days: What I Actually Do

**Week 1–2:** Listen. 1:1 with every engineer, PO, and stakeholder. Shadow incidents. Shadow deployments. Meet the banking partner. Understand what the team has been saying for two years that nobody acted on.

**Week 3–4:** Quick wins that reduce team pain — not add process. Daily cross-team standup. Mandatory code review ("Law of 4 Eyes"). Incident war room with clear escalation. DORA dashboard live. Support ticket top-10 analysis → root causes into backlog.

**Month 2:** Structure. "Two Product Principle" — every sprint carries customer value AND technical improvement. QA fully embedded. Smaller batches → weekly releases. MTTR target: <2 hours. Contractors arriving — scoped to absorb BAU load, not create onboarding burden.

**Month 3:** Governance + Roadmap. Architecture Review Board. POPIA compliance checklist. Partner SLA framework. Cloud migration plan to EXCO. Hiring plan. Monthly delivery dashboard to EXCO.

*By day 90: EXCO sees improving metrics, a credible roadmap, and a team that believes it can win.*

^
Two things that are different here from a typical 90-day plan. First, I lead with listening — I don't arrive with a playbook and impose it. I arrive with hypotheses and validate them. At ABSA, my first month was spent understanding what people had been asking for. Most of what I "introduced" was what the team already knew they needed but couldn't get leadership to prioritise. Second, the sequencing principle: remove load before adding process. The contractors in month 2 are specifically scoped to absorb grunt work so the existing team can breathe. You cannot ask an exhausted team to simultaneously deliver and transform. The Practices of Mastery — Check It In, Code Review, Code Style, TDD, Automation — roll in incrementally, not as a big bang. Code review alone reduces defect leakage 30-40%.

---

# Delivery & DevOps: The Maturity Journey

**Foundation (Months 1–3)** — CI for all repos. Code review gates. Basic monitoring + alerting. Test coverage 45% → 60%.

**Acceleration (Months 4–9)** — CD with staging. Contract testing. Terraform IaC. Feature flags for progressive delivery. Coverage 60% → 75%.

**Excellence (Months 10–18)** — Continuous deployment. Canary releases. Chaos engineering. Security scanning in pipeline. Coverage 75% → 85%+.

**The insight that changes everything:** Most teams discover 80%+ of their lead time is **waiting**, not working. Reducing handoffs, queues, and dependencies — not making people work faster — is where the real gains live. *(Pereira & Davis, Flow Engineering)*

^
At AXA, I designed CI/CD pipelines that cut deployment lead times by 30% — most of that gain came from removing wait states. At ABSA, I built this culture from scratch: 50% of teams with automated builds within 6 months, 30% cross-functional with DevOps practices per sprint in year one. These practices compound — each amplifies the others. The DORA + Flow metrics framework gives us both lenses: DORA tells us if we're shipping quality at speed; Flow metrics tell us where the waste is. I'd run a Value Stream Mapping exercise in the first 30 days to make the waste visible.

---

# Architecture: What We're Building Toward

```
              ┌──────────────────────────────────┐
              │     API Gateway (Kong/Apigee)      │
              │  Rate limiting · Auth · Routing     │
              └─────┬─────────┬──────────┬────────┘
                    │         │          │
         ┌─────────┤         │          ├──────────┐
         ▼         ▼         ▼          ▼          │
    Payments   Lending     KYC     Integration     │
    Service    Service    Engine    Gateway         │
         │         │         │          │          │
         └─────────┴─────────┴──────────┘          │
                    │                               │
           Platform Services                        │
      Events · Auth · Audit · Data · Monitoring     │
                    │                               │
           Cloud Infrastructure                     │
        Kubernetes · IaC · CI/CD · Observability     │
```

**Security baked in:** SAST/DAST in CI/CD · Zero-trust · TLS 1.3 · Container scanning · Immutable infra
**Migration:** Strangler Fig — 25%→50% (M1–6) → 75% (M6–12) → 95% (M12–18). Not big-bang.

^
Domain-Driven Design. Each domain independently deployable with clear API contracts. The Strangler Fig pattern wraps the legacy system, routes new traffic to new services, and gradually retires the old. At John Lewis, I led exactly this migration while safeguarding continuity — they were losing £1M/month before the transformation. At Equal Experts, same approach. Security is automated into the pipeline: at Old Mutual I used Auth0 CIAM for enterprise-grade identity; at Sanlam, regulatory architecture alignment during de-merger. Build vs Buy principle: buy commodity (API Gateway, IAM, Monitoring, CI/CD), build differentiators (payment processing, lending engine, KYC orchestration, partner adapters). With 10 engineers, every hour matters.

---

# AI & Data: Sequenced Bets, Not Science Projects

| Use Case | Business Value | Timeline | Gate |
|----------|---------------|----------|------|
| **Credit scoring ML** | Faster, more accurate SME lending | Q4 Y1 | Shadow model alongside rules — prove before switch |
| **Fraud detection** | Lower transaction fraud, partner confidence | Y2 | Data readiness audit passes |
| **AI-assisted KYC** | Onboarding: days → minutes | Y2 | Data readiness audit passes |
| **Intelligent support** | Deflect 30–40% of tickets (+40% is unsustainable) | Y2 | Knowledge base from M1–3 ticket analysis |

**Data foundation (built in, not bolted on):** Data lake/lakehouse · dbt + Airflow · Feature store · Schema registry · Great Expectations for quality · Model registry with NCA-required explainability · Data residency per market (POPIA, NDPR, Kenya DPA) · Data engineering in platform team, co-owned with Data & Analytics from day 30.

**Fallback:** Country 1 launches with rule-based scoring if data isn't model-ready. Data readiness audit in first 60 days determines the real schedule.

^
At AXA, I took ML models from research to production — shadow deployments at 20% traffic, automated retraining pipelines, and model governance. The gating principle is critical: AI only ships on a stable platform, and only when the data is ready. The 60-day data readiness audit is one of the first activities, not something discovered at month six. Credit scoring first because it has the clearest revenue impact and likely the most available training data. The other three are Year 2 candidates, sequenced on data maturity. Model risk committee co-owned with Data & Analytics and Compliance — bias auditing and drift monitoring are non-negotiable for regulated lending. If asked about analytics consumers: the event-driven architecture emits schema-versioned events via schema registry, ensuring downstream analytics can consume without coupling.

---

# Business Alignment: Every Rand Maps to a Board Bet

| Board Priority | What Engineering Delivers | When | Revenue/Risk Impact |
|---------------|--------------------------|------|-------------------|
| 2 new countries | Multi-tenant architecture, data residency | Q3–Q4 Y1 | R80–120M new revenue |
| Real-time payments | Event-driven microservice, partner APIs | Q4 Y1–Q2 Y2 | R40–60M new revenue |
| Cloud migration | Strangler fig, IaC, Kubernetes | 18 months | R15–25M annual savings |
| Partner confidence | SLA framework, monitoring, joint DR | Q1 | Protect R20–50M partnership |
| Regulatory | POPIA automation, audit trails, data localisation | Q1–Q2 | Licence to operate |
| AI/Innovation | ML credit scoring → fraud → KYC → support | Q4 Y1–Y2 | Product differentiation |

*This isn't a technology roadmap. It's the board's growth strategy, expressed as engineering work.*

^
The OAR model frames every decision: Objective (what business outcome?), Assumption (what must be true?), Reflection (how do we know we're wrong?). At Accenture, I benchmarked delivery value chains to ensure every tech investment mapped to business priorities. The biggest mistake in engineering-led transformations is building technically excellent solutions that don't connect to revenue. Notice I've added a Revenue/Risk Impact column — EXCO doesn't think in "microservices" and "Kubernetes." They think in rands, risk, and competitive position.

---

# Risk, Compliance & the Banking Partner

**POPIA (2026 enforcement)** — Information Officer appointed. Data localisation per market baked into architecture. Breach notification automation. Consent management in KYC engine.

**Financial Services** — SARB payments alignment. AML controls. Transaction monitoring. Full audit trail.

**Governance** — Architecture Review Board (I built and governed this at Barclays ABSA). Change Advisory Board. Quarterly reporting to EXCO. Annual pen testing.

**Banking Partner — a 90-day trust restoration:**
**Week 1:** Meet their leadership. Joint incident review. Commit to SLAs with teeth.
**Month 1–3:** Dedicated monitoring dashboard. Staging mirror. Monthly joint reviews. Shared milestones.
**Ongoing:** Status page. Quarterly business reviews. Joint DR testing.

*They don't need perfection. They need a credible plan, measurable progress, and a leader who picks up the phone.*

^
At Discovery, I managed the Manulife partnership across three markets — aligning roadmaps, managing escalation, building trust through radical transparency. The banking partner situation is urgent but solvable: most partner crises are communication failures, not technical ones. At Sanlam, I navigated regulatory architecture during a de-merger. The compliance framework isn't optional — it's the licence to operate. POPIA's 2026 data localisation enforcement and the varying African data sovereignty laws (Nigeria NDPR, Kenya DPA) are material architectural constraints that affect where data can be stored, processed, and used for model training.

---

# People: The 10 Who Stayed Are Your Greatest Asset

**The truth about 18% attrition:** The 10 engineers who are still here chose to stay through chaos. They are not the problem — they are the foundation. My first commitment is to them.

**Retain** (fix the bleed before you hire):
Comp: match-to-lead SA market, annual benchmarking vs remote-international rates, equity/LTI for seniors
Career: dual ladder — Senior → Staff → Principal Engineer (IC) alongside Team Lead → EM → Director (management). Equal comp, equal influence.
Culture: guilds, conference budget, blameless post-mortems, on-call rotation that's sustainable

**Hire** (10 → 25+ in 12 months):
M1–3: 3–4 senior contractors — scoped to absorb BAU, pre-built onboarding packs, NOT to evaluate or replace existing staff
M3–12: permanent hires via SA fintech pool, diaspora network, engineering brand (tech blog, open source, talks)
Graduate pipeline: WeThinkCode_, Umuzi, university partnerships → intern-to-hire by Y2

**EE/B-BBEE:** Diverse shortlists (min 50% designated groups). Structured interviews. Diverse panels. I own the targets personally — not delegated to HR.

**If hiring lags:** Stream-aligned teams prioritised. Platform runs lean. Timelines flex, commitments don't disappear.

^
At Discovery, the biggest retention factor wasn't compensation — it was whether engineers felt their work mattered. But Purpose, Autonomy, and Mastery are necessary, not sufficient. People also need to be fairly compensated and see a credible future. At ABSA, I built the engineering brand from zero — community events, internal tech talks, open coaching sessions. That pipeline became self-sustaining. The contractor bridge is specifically designed to reduce load on existing staff. They arrive with onboarding documentation and are scoped to tech debt and stability work where deep domain knowledge isn't required. The existing team gets first consideration for leadership roles in the new structure. Nobody who held this company together gets sidelined without a conversation and a real option. Team structure follows Team Topologies: 3 stream-aligned (Payments, Lending, KYC), 1 platform (CI/CD, infra, data engineering, shared services), 1 enabling (temporary — upskill cloud-native/DevOps, then dissolve).

---

# How We Know It's Working

| Metric | Now | 6 Months | 12 Months | Owner |
|--------|-----|----------|-----------|-------|
| On-time delivery | 62% | 75% | **85%+** | Me + POs |
| Deploy frequency | 2–3 weeks | Weekly | **2x/week** | Platform lead |
| Critical bugs | 18/month | <8 | **<3** | Stream leads |
| Test automation | 45% | 65% | **80%** | Engineering |
| MTTR | 6–10 hrs | <2 hrs | **<1 hr** | On-call rotation |
| Attrition | 18% | 14% | **<10%** | Me + HR |
| Cloud migration | 25% | 55% | **80%** | Platform lead |
| Support tickets | +40% YoY | Flat | **-20% YoY** | Me + Support |

**Every metric has a name next to it.** Not a team. A person. Accountability is specific or it's performative.

^
The Owner column is the difference between a dashboard and a system. At AXA, I built real-time dashboards with probabilistic forecasting — 15% better predictability, 20% faster approvals. But dashboards don't drive change; ownership does. I'd track four categories: DORA (delivery performance), Flow (where waste lives — cycle time, wait time, WIP, flow efficiency), Business (on-time delivery, support tickets, uptime, revenue enabled), and People (attrition, eNPS, on-call burden, learning days). The key insight from Flow Engineering: most teams discover 80%+ of lead time is waiting, not working. The biggest gains come from eliminating queues and handoffs.

---

# Stakeholders: One Set of Data, Five Conversations

| Who | What They Actually Need | What I Tell Them | Cadence |
|-----|------------------------|-----------------|---------|
| **CEO** | "Are we going fast enough?" | Deploy frequency, lead time, capacity vs ambition | Weekly 1:1 |
| **CPO** | "When do I get my features?" | Innovation allocation, feature flags, joint roadmap | Weekly sync |
| **CRO** | "Are we exposed?" | ARB decisions, compliance dashboards, audit readiness | Bi-weekly |
| **COO** | "Will it stay up?" | DORA dashboard, SLAs, incident trends, MTTR | Weekly |
| **Partner** | "Can I trust you?" | Dedicated monitoring, joint milestones, shared DR | Monthly |

**When they collide** (and they will): Quantify both sides. Find the third option. Own the recommendation. 48-hour escalation SLA if Product and Engineering can't resolve — escalate jointly to CEO/COO. No sandbagging, no unilateral vetoes.

^
Here's a specific example: CEO says "ship the payments feature now." CRO says "not until the security audit clears." Both are right. My approach: quantify it — "shipping now = R2M revenue/month. Shipping without audit = R50M exposure if breached." Then find the third option — feature flags: ship to 5% of users behind a flag, run the audit in parallel. CEO gets momentum, CRO gets controls. I recommend option 3, explain the risk, and present the rollback plan. At Discovery, I navigated this exact dynamic between Manulife's product ambitions and regulatory constraints across three markets. When the commercial case was clear and risk was bounded, I found a way to make it work — sometimes by conceding engineering priorities with a documented payback plan.

---

# Hard Trade-off 1: Speed vs. Stability

**The call:** Invest in stability FIRST. It unlocks speed.

| Phase | Stability | Features | Trigger to Shift |
|-------|-----------|----------|-----------------|
| Months 1–3 | **70%** | 30% | MTTR <2hrs and deploy weekly → shift to 50/50 |
| Months 4–6 | 50% | 50% | Critical bugs <5/month → shift to 30/70 |
| Months 7+ | 30% | **70%** | Maintain via Two Product Principle |

**This is not negotiable in month 1. It IS negotiable based on data.**

If MTTR hits target by week 8, I accelerate to 50/50 in month 3 instead of month 4. The ratio is a starting position calibrated to severity — not a decree. I'd co-present this trade-off to the board with the CPO, not as a unilateral engineering decision.

**Evidence:** DORA — elite performers ship 182x more frequently AND have 8x lower failure rates. At ABSA, I halved cycle times by investing in foundations first.

^
The "Trigger to Shift" column is what the original version was missing. It turns a rigid 70/30 decree into a data-driven contract: here's the deal, and here's exactly when you get your features back. The CPO should see this and think "that's fair — show me the data and I'll hold you to the triggers." At ABSA, investing in DevOps practices first is what unlocked velocity. If you want to go faster in 6 months, invest in the foundations today. The Two Product Principle — every sprint carries both customer value and technical improvement — prevents the false choice from recurring after month 7.

---

# Hard Trade-off 2: Build vs. Buy

**The call:** Buy commodity. Build what makes ABC unique. With 10 engineers, every hour is a strategic choice.

| Buy (commodity) | Build (differentiator) | Why |
|----------------|----------------------|-----|
| API Gateway (Kong/Apigee) | Payment processing logic | Gateway is table stakes; payment logic IS the product |
| IAM (Auth0/Azure AD B2C) | Lending decision engine | Identity is solved; credit risk modelling is ABC's edge |
| Monitoring (Datadog/Grafana) | KYC workflow orchestration | Observability is commodity; KYC compliance is hard-won IP |
| CI/CD (GitHub Actions) | Partner integration adapters | Pipeline tooling is mature; partner integrations are bespoke |

**Cost awareness:** Auth0 scales per-authentication — model costs at projected volume before committing. Datadog per-container pricing with Kubernetes can surprise you. R2–3M tooling budget needs stress-testing against multi-region, multi-service growth. OpenTelemetry as an abstraction layer protects portability.

^
At Old Mutual, I used Auth0 rather than building IAM — saved months of engineering time. At John Lewis, I advised on sunset vs. modernise decisions. The "Why" column is what elevates this from a list to a strategy: it shows I understand where ABC's competitive advantage lives. The cost awareness section pre-empts the IT exec's vendor lock-in question. I've added the OpenTelemetry note because it's the answer to "what's your exit strategy if Datadog gets expensive?" — abstract the instrumentation layer so you can swap backends without re-instrumenting.

---

# Hard Trade-off 3: Growth vs. Stability — African Expansion

**The call:** Parallel tracks with a hard gate. No launch on an unstable platform.

**Track 1 — Platform** (engineering): Cloud to 50%+, multi-tenant architecture, data residency per market, POPIA/NDPR/Kenya DPA compliance

**Track 2 — Market** (no engineering dependency): Regulatory analysis, commercial partnerships, localisation, go-to-market planning

**Hard Gate — Country 1 does NOT launch until:**
MTTR < 2 hrs · Deploy weekly · Critical bugs < 5/month

**Why the gate matters:** Launching into Kenya or Nigeria on today's platform risks losing *both* the new market AND the existing South African business. A production outage in a new market with no local engineering presence becomes a reputational crisis that spreads back home.

*The market track runs in parallel. The engineering track sets the pace. When the gate clears — and it will — we launch with confidence, not hope.*

^
At Barclays ABSA, I designed architecture for digital banking across Africa. We sequenced on platform readiness, not market ambition alone. Multi-region in Africa is harder than most people realise: AWS has Cape Town but limited presence elsewhere, data sovereignty laws vary by country, latency to West Africa from SA is 150-200ms. The hard gate protects the business from itself — the temptation to launch early because commercial pressure demands it is exactly how companies blow up their reputation in new markets.

---

# The ABSA Mirror

When I arrived at ABSA, I found **this exact situation:**

Six siloed teams. No DevOps culture. Manual deployments. Engineers leaving. Platform instability. Pan-African ambitions on a foundation that couldn't support them.

**What I built:**
- "Six Conditions for Transformation" — starting with Conway's Law, restructuring teams for flow
- Practices of Mastery — five non-negotiable engineering habits
- Community through coaching, guilds, and blameless post-mortems

**What changed:**
- Halved cycle times within 12 months
- +5% employee engagement
- 50% of teams with automated builds in 6 months
- Architecture Review Board that is still governing today, years after I left

**Why this matters for ABC:** Every challenge in this case study — silos, attrition, inconsistent DevOps, scaling across Africa, partner pressure, regulatory complexity — is one I've already solved. Not in a book. In a codebase, with a team, under pressure.

^
I'm telling the ABSA story as a mirror, not a trophy. The panel should hear this and think "that IS our situation." The other proof points: Discovery/Manulife (multi-market delivery at scale, partner management, Capex/Opex modelling), AXA (ML to production, CI/CD pipelines, 30% faster deploys), John Lewis (£1M/month losses fixed via cloud migration), Old Mutual (AWS + Auth0 CIAM), Sanlam (de-merger regulatory architecture), Accenture (delivery value chain benchmarking). Every recommendation in this deck comes from something I've shipped, scaled, or rescued.

---

# The Investment

| Area | Year 1 | Year 2 | What It Unlocks |
|------|--------|--------|-----------------|
| **Headcount** (10→25) | R15–20M | R25–30M | Capacity for all three board bets |
| **Tooling** (CI/CD, monitoring, security) | R2–3M | R1–2M | 60%+ MTTR reduction, automated compliance |
| **Cloud migration** | R3–5M | R2–3M | R15–25M annual infra savings by month 18 |
| **Training & culture** | R500K–1M | R500K | Attrition savings: R3M+/year |

**Total Year 1: ~R22–29M**

**ROI framing:** This isn't R25M of cost. It's R25M to unlock R120–200M of board-approved revenue, R15–25M of annual savings, and R3M+ of avoided attrition cost. The alternative — doing nothing — costs more.

^
At Discovery, I built Capex/Opex models for Manulife leadership to justify exactly this kind of investment. The key is the last line: frame the alternative. EXCO isn't choosing between "spend R25M" and "spend nothing." They're choosing between "spend R25M and unlock R200M" or "spend nothing and lose R50M+ in partner risk, regulatory exposure, and competitive decay." Every rand maps to a board-approved initiative.

---

# My Commitment — Hold Me to This

| Horizon | Deliverable | How You'll Know |
|---------|------------|-----------------|
| **Day 30** | Listened to every engineer. Quick wins live. Banking partner has a plan. | DORA dashboard is live. Partner has signed SLA framework. |
| **Day 90** | Delivery stabilising. Governance in place. Roadmap to EXCO. | MTTR trending <2hrs. Weekly deploys started. Attrition: zero unplanned departures. |
| **Month 12** | Platform supports growth. Team scaled. Country 1 live. | MTTR <1hr. Deploy 2x/week. Cloud 80%. Team 20+. Hard gate cleared. |
| **Month 24** | Elite engineering. Full cloud-native. Revenue flowing from new markets. | Two countries live. Real-time payments generating revenue. AI/ML in production. |

*If after 90 days the team doesn't see a material difference, hold me accountable. I'm putting my credibility on the line — not theirs.*

^
The "How You'll Know" column makes this testable. The last line is deliberate — it's the answer to the team leader who asks "why should I believe you?" I'm not asking the existing team to trust me on faith. I'm asking them to give me 90 days and judge me on results. At every organisation I've transformed, the turning point wasn't a strategy document — it was the moment the team believed the leader would actually follow through. That moment is earned, not declared.

---

![](https://images.pexels.com/photos/1287145/pexels-photo-1287145.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] Thank You

**Benjamin Hinson**
bhinson@plerk.co.za · 082 565 4665

> *"The team that wins isn't the one with the most talent.*
> *It's the one with the best system."*

I welcome your questions.

^
Every challenge in the ABC Technologies case study maps directly to something I've delivered — DevOps transformation at ABSA, African expansion architecture at Barclays, cloud migration at John Lewis, partner management at Discovery, CI/CD excellence at AXA, regulatory governance at Sanlam. This isn't theory — it's pattern recognition built over two decades. I'd be honoured to build it here. Thank you.

---

# Appendix: DORA 2024 Benchmarks

| Metric | Elite | High | Medium | Low |
|--------|-------|------|--------|-----|
| Deploy Frequency | On demand | Weekly | Monthly | Quarterly |
| Lead Time | <1 hour | Days | Weeks | Months |
| MTTR | <1 hour | <1 day | <1 week | >6 months |
| Change Failure Rate | <5% | 10% | 15% | 25%+ |

The gap is widening: high performance shrank 31% → 22% (2023–2024).

---

# Appendix: SA Fintech 2025–2026

- SA fintech projected USD 3.7–14.9 billion by 2033
- Card transactions: ZAR 2.9 trillion (2025), +10.4% annually
- POPIA data localisation enforcement: 2026
- SARB payments modernisation — first overhaul in ~3 decades
- PAPSS under AfCFTA enabling pan-African settlement
- 92% of fintech startups use public cloud and API-first
