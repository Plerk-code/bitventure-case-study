theme: Titillium, 1
footer: Benjamin Hinson | ABC Technologies Case Study
slidenumbers: true
autoscale: true
footer-style: #999999
header-strong: #FFFFFF
text-strong: #FFFFFF

---

![](https://images.pexels.com/photos/29327972/pexels-photo-29327972.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] Stabilise · Scale · Accelerate
## A Strategic Blueprint for ABC Technologies

**Benjamin Hinson**
March 2026

^
Good morning. I'm Benjamin Hinson. Over the past 20 years I've built, rescued, and scaled engineering organisations across financial services — from transforming DevOps culture at ABSA serving pan-African markets, to architecting cloud-native platforms at AXA and John Lewis, to leading delivery for North America's largest insurer at Discovery. Every recommendation today is grounded in what I've delivered in practice. I'll walk you through my diagnosis, strategy, 90-day plan, and the hard trade-offs I expect to face. Let me start with where ABC stands today.

---

# The Vital Signs

| Metric | ABC Today | Target | Delta |
|--------|-----------|--------|-------|
| On-time delivery | **62%** | 85%+ | **+23%** |
| Critical bugs/month | **18** | <5 | **-13** |
| MTTR | **6–10 hrs** | <1 hr | **-5 to 9 hrs** |
| Deploy frequency | **2–3 weeks** | Daily | **~10–15x** |
| Test automation | **~45%** | 75%+ | **+30%** |
| Cloud migration | **25%** | 100% | **+75%** |
| Attrition | **18%** | <10% | **-8%+** |
| Support tickets | **+40%** | Declining | **Lagging** |

^
Every metric is trending the wrong way. But the fundamentals are strong — revenue is up, customers growing, partnerships expanding. This is a systems problem, not a talent problem. I've seen this pattern before and resolved it. Here's where each target comes from: On-time delivery 85%+ — Standish Group CHAOS reports and Agile maturity benchmarks; high-performing teams consistently hit 80–90% sprint commitment reliability. Critical bugs <5/month — DORA Change Failure Rate; elite performers sustain <5% change failure rate, which at ABC's deploy cadence maps to fewer than 5 critical bugs per month. Also aligns with Google SRE error budget practices. MTTR <1 hour — directly from the DORA 2024 State of DevOps Report; this is the Elite benchmark. ABC currently sits between Low and Medium. Deploy frequency daily — DORA 2024; Elite is on-demand, High is weekly. Daily sits between the two. ABC is currently in the Low tier at fortnightly. Test automation 75%+ — Martin Fowler's Testing Pyramid and Google's engineering practices target 70–80% unit coverage. Microsoft research shows defect leakage drops significantly above 70% — 75% is the inflection point where automated testing becomes a reliable safety net. Cloud migration 100% — this is a board-mandated objective, not an industry benchmark. The 12-month operational target is 80%, with 95%+ by month 18. Attrition <10% — LinkedIn Talent Insights and Mercer SA tech compensation surveys. SA tech industry average is 13–15%. Top SA employers like Discovery and Investec tech achieve 7–10%. At 18%, ABC is in crisis territory — replacing nearly 1 in 5 engineers annually. Support tickets declining — this is a lagging indicator, not a benchmarked target. It follows from improvements in MTTR, defect rates, and platform stability. The leading indicators are the other seven metrics.

---

# Root Cause: Four Types of Debt

**Structural** — Silos across 6 teams. Handoffs multiply, context is lost. Nobody owns delivery end-to-end.

**Process** — Inconsistent code reviews, partial QA embedding. Quality is a lottery, not a system property.

**Architectural** — 25% cloud migration with monolithic heritage. Every new feature risks destabilising production.

**Cultural** — 18% attrition signals engineers don't see a path to mastery, purpose, or autonomy — the three intrinsic motivators that retain top talent.

^
At ABSA, I inherited the same pattern — siloed teams, no DevOps culture, manual processes. Within 12 months we halved cycle times. The fix isn't heroism — it's system design. Conway's Law tells us organisations create systems that mirror their communication structures. Silos create barriers to velocity. That's exactly what we need to break.

---

# Five Pillars — Phased for Reality

| Phase | Timeline | Focus |
|-------|----------|-------|
| **Stabilise** | Months 1–6 | Delivery predictability, incident response, quality gates |
| **Standardise** | Months 4–12 | Engineering standards, DevOps pipelines, architecture governance |
| **Scale** | Months 6–18 | Cloud-native migration, API-first platform, team growth to 25+ |
| **Accelerate** | Months 12–24 | New markets, new products, AI experimentation, innovation capacity |
| **Culture** | Continuous | High-performance engineering as the throughline |

These overlap deliberately. You can't do everything at once with 10 people — sequence ruthlessly.

^
At AXA, I ran shadow deployments at 20% traffic while stabilising the main system. Parallel tracks, managed risk. At Barclays ABSA, I built a multi-year capability-based technology roadmap for digital banking across Africa. The quarterly breakdown: Q1 — incident management, MTTR <2hrs, CI/CD baseline, code review 100%. Q2 — deploy weekly, bugs <8, Architecture Review Board, microservices pilot, Country 1 prep. Q3 — DevOps maturity L3, migration 60%, Country 1 launch. Q4 — migration 80%, API gateway, real-time payments MVP, AI/ML pilot.

---

# Days 1–30: Listen, Assess, Quick Wins

**Listen** — 1:1 with every engineer, PO, stakeholder. Shadow incidents and deployments. Review 6 months of production data. Meet the banking partner.

**Quick wins** — Daily cross-team standup (break silos). Mandatory code review — "Law of 4 Eyes". Incident war room with escalation paths. DORA metrics dashboard live.

**Support ticket feedback loop** — Top 10 ticket categories analysed. Root causes fed into sprint backlog as tech debt items. Self-service knowledge base for repeat queries. Weekly ticket-to-bug triage with product and support.

**Sequencing principle** — Remove load before adding process. Contractors absorb BAU burden first. New practices roll in incrementally — not a big bang on day 31.

^
At ABSA, I called these the "Practices of Mastery" — five non-negotiable habits: Check It In, Code Review, Code Style, TDD, Automation. You don't need a strategy document to start. Code review compliance alone typically reduces defect leakage by 30-40%. Critically, the existing team must feel relief before they feel new demands — otherwise transformation becomes just another burden on already-stretched people. The support ticket feedback loop is critical — tickets are up 40% and that's a lagging indicator of platform instability. In month 1 we analyse the top 10 categories, identify root causes, and feed them directly into the sprint backlog. A self-service knowledge base handles repeat queries immediately. By month 3, ticket-to-bug triage is a weekly ritual.

---

# Days 31–90: Structure, Standards & Governance

**Delivery** — "Two Product Principle": every sprint = customer value + technical improvement. Quality gates. Smaller batches → weekly releases. MTTR target: under 2 hours.

**Teams** — QA fully embedded. "You build it, you run it." Clear ownership of build, test, deploy, AND operate.

**Architecture** — API and service inventory. Top 5 tech debt items. Draft target-state architecture.

**Governance** — Architecture Review Board. POPIA compliance checklist. Partner SLA framework. Monthly EXCO delivery dashboard. Cloud migration plan to EXCO. Hiring plan: 10 → 20–25 in 12 months.

**Culture** — Engineering guild. Blameless post-mortems. On-call rotation — no more heroics.

*By day 90: EXCO sees improving delivery, a credible roadmap, and a team that believes they can win.*

^
The Two Product Principle prevents the false choice between "features or debt." I developed this at ABSA — every release carries both customer value and technical improvements, by design. At Discovery, I ran monthly delivery reports to Manulife leadership tracking exactly these dimensions. Transparency builds trust. The governance structures — ARB, POPIA checklist, partner SLAs — are all established by day 90 so the system can run without heroics.

---

# DevOps Maturity Phases

**Foundation (Months 1–3)** — CI for all repos. Code review gates. Basic monitoring. Coverage 45% → 60%.

**Acceleration (Months 4–9)** — CD with staging automation. Contract testing. Terraform IaC. Feature flags. Coverage 60% → 75%.

**Excellence (Months 10–18)** — Continuous deployment. Canary releases. Chaos engineering. Security scanning. Coverage 75% → 85%+.

**Key insight:** Most teams discover 80%+ of lead time is **waiting**, not working. The biggest gains come from eliminating queues and handoffs — not making people work faster. *(Flow Engineering, Pereira & Davis)*

^
At ABSA, I built this culture from scratch. At AXA, I used shadow deployments at 20% traffic to validate ML models before full rollout. The DORA + Flow metrics framework gives us both sides: DORA tells us if we're shipping quality at speed; Flow metrics tell us where the waste lives. I'd run a Value Stream Mapping exercise in the first 30 days. At AXA, CI/CD pipelines cut deployment lead times by 30% — most of that gain came from removing wait states, not making people work faster.

---

# Target Architecture — Cloud-native, API-first

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
        Events · Auth · Audit · Monitoring          │
                    │                               │
           Cloud Infrastructure                     │
        Kubernetes · IaC · CI/CD · Observability     │
```

**Security baked in:** SAST/DAST in CI/CD · Zero-trust · TLS 1.3 · Container scanning · Immutable infrastructure · Quarterly pen testing

^
Domain-Driven Design. Each domain independently deployable with clear API contracts. Security is automated into the pipeline, not bolted on after — at Old Mutual I used Auth0 CIAM for enterprise-grade security; at Sanlam, regulatory architecture alignment during de-merger. This is how I architected pan-African digital banking at Barclays ABSA and the microservices transformation at John Lewis.

---

# Cloud Migration: Strangler Fig Pattern

| Phase | Timeline | Migration | Action |
|-------|----------|-----------|--------|
| **Lift & Stabilise** | Months 1–6 | 25% → 50% | Containerise, Terraform, non-critical first |
| **Decompose** | Months 6–12 | 50% → 75% | Extract payments, API gateway, events |
| **Optimise** | Months 12–18 | 75% → 95% | Auto-scaling, multi-region for Africa |

Not big-bang. Wrap the legacy system, route new traffic to new services, gradually retire the old.

^
At John Lewis, I led legacy-to-modern migration while safeguarding continuity. At Equal Experts, we saved them from £1M/month losses using exactly this approach.

---

# AI & Data Platform

**AI use cases — sequenced, not simultaneous:**

| Use Case | Timeline | Approach |
|----------|----------|----------|
| **Credit scoring ML** | Q4 Y1 | Shadow model alongside existing rules |
| **Fraud detection** | Y2 — gated on data readiness | Event stream analysis on payments data |
| **AI-assisted KYC** | Y2 — gated on data readiness | Document extraction + identity verification |
| **Intelligent support** | Y2 — gated on data readiness | LLM triage — deflect 30–40% of tickets |

**Data foundation:** Data lake/lakehouse · dbt + Airflow · Feature store · Schema registry · Great Expectations for data quality · Model registry with explainability (NCA compliance) · Data residency per market (POPIA, NDPR, Kenya DPA)

**Fallback:** Country 1 launches with rule-based scoring if data isn't model-ready. Data readiness audit in first 60 days.

^
At AXA, I took ML models from research to production — shadow deployments at 20% traffic, automated retraining pipelines, and model governance. AI without engineering discipline is a liability. AI on a well-architected platform is a competitive moat. The AI timeline is a target, not a commitment — the 60-day data readiness audit determines the real schedule. Data engineering is embedded in the platform team with joint planning with Data & Analytics in the first 30 days — co-own the strategy, don't build a parallel silo. Model risk committee co-owned with Data & Analytics and Compliance. Bias auditing and drift monitoring are non-negotiable for regulated lending.

---

# Board Priorities → Technology Response

| Board Priority | Tech Response | Timeline | Outcome |
|---------------|---------------|----------|---------|
| 2 new countries | Multi-tenant, data residency | Q3–Q4 Y1 | Revenue diversification |
| Real-time payments | Event-driven microservice | Q4 Y1–Q2 Y2 | New product revenue |
| Cloud migration | Strangler fig, IaC | 18 months | 20–30% cost reduction |
| Partner confidence | SLA framework, monitoring | Q1 | Retain banking partner |
| Regulatory | POPIA automation, audit trails | Q1–Q2 | Licence to operate |
| Innovation & AI | ML credit scoring, fraud detection, AI-assisted KYC | Q4 Y1–Y2 | Product differentiation |

*Every tech investment maps to a board-approved initiative. Technology as revenue enablement, not overhead.*

^
The OAR model — Objective, Assumption, Reflection — frames every decision. What business outcome? What must be true? How do we know we're wrong? At Accenture, I benchmarked delivery value chains to ensure every tech investment had a clear line to priorities. The biggest mistake in engineering-led transformations is building technically excellent solutions that don't map to business outcomes.

---

# Risk, Governance & Partners

**POPIA (Critical 2026)** — Information Officer. Data localisation per market. Breach notification automation. Consent management in KYC engine.

**Financial Services** — SARB payments alignment. AML controls. Transaction monitoring. Full audit trail.

**Governance** — Architecture Review Board. Change Advisory Board. Quarterly reporting. Annual pen testing.

**Banking Partner — Restore Trust:**
Days 1–30: Meet leadership, joint incident review, commit to SLAs, dedicated monitoring.
Days 30–90: Automated health checks, staging mirror, monthly reviews, shared milestones.
Ongoing: Status page, quarterly business reviews, joint DR testing.

*They don't need perfection on day one. They need a credible plan with measurable progress.*

^
At Barclays ABSA I built and governed the Architecture Review Board. At Sanlam, regulatory architecture alignment during de-merger. At Discovery, I managed the Manulife partnership — aligning roadmaps, managing escalation, building trust through transparency.

---

# People: Scale, Retain, Transform

**Team structure** (Team Topologies): 3 stream-aligned (Payments, Lending, KYC) · 1 platform · 1 enabling (temp). "You build it, you run it."

**Retain** — Purpose (every sprint connects to R500M) · Autonomy (teams own backlog, architecture, deploys) · Mastery (guilds, conference budget, blameless post-mortems)

**Hire** — Months 1–3: 3–4 senior contractors scoped to absorb BAU load. Months 3–12: permanent hires, SA fintech pool + diaspora. Graduate pipeline: WeThinkCode_, Umuzi, university partnerships by Year 2.

**Comp** — Match-to-lead SA market. Dual career ladder (IC: Senior → Staff → Principal Engineer). Equity/LTI for senior hires.

**EE** — Diverse shortlists (min 50% designated groups). Structured interviews. I own the EE targets personally.

**If hiring lags:** prioritise stream-aligned teams. Platform runs lean. Timelines flex, commitments don't disappear.

^
At Discovery, the biggest retention factor wasn't compensation — it was whether engineers felt their work mattered. At ABSA I built the engineering brand from zero — community events, internal tech talks, open coaching sessions. The contractor bridge reduces load on existing staff, not adds to it — they arrive with onboarding documentation and are scoped to tech debt work. Existing team members are the anchors — first consideration for leadership roles. Nobody who held this company together gets sidelined without a conversation and a real option. Purpose, Autonomy, and Mastery are necessary but not sufficient — people also need fair comp and a credible future. The IC track matters: our best engineers didn't want to manage people.

---

# 12-Month Targets

| Metric | Current | 6 months | 12 months |
|--------|---------|----------|-----------|
| On-time delivery | 62% | 75% | **85%+** |
| Deploy frequency | 2–3 weeks | Weekly | **2x/week** |
| Critical bugs/month | 18 | <8 | **<3** |
| Test automation | 45% | 65% | **80%** |
| MTTR | 6–10 hrs | <2 hrs | **<1 hr** |
| Attrition | 18% | 14% | **<10%** |
| Cloud migration | 25% | 55% | **80%** |
| Support tickets | +40% YoY | Flat | **-20% YoY** |

^
Every metric has an owner and a clear "how" in this deck. DORA metrics for delivery performance, Flow metrics for where waste lives, Business metrics for value delivery, People metrics for culture health. At AXA: real-time dashboards with probabilistic forecasting — 15% better predictability, 20% faster approvals.

---

# Stakeholder Communication

| Stakeholder | What They Hear | Cadence |
|------------|----------------|---------|
| **CEO** | Deploy frequency + lead time. Capacity vs ambition. | Weekly 1:1 |
| **CPO** | Innovation time. Feature flags. Joint roadmap. | Weekly sync |
| **CRO** | ARB decisions. Compliance dashboards. | Bi-weekly |
| **COO** | DORA dashboard. SLAs. Incident trends. | Weekly |
| **Banking Partner** | Dedicated monitoring. Joint reviews. | Monthly |
| **EXCO** | Delivery report. Quarterly roadmap. | Monthly |

*One set of metrics, different lenses for different stakeholders.*

---

# When Stakeholders Collide

**The scenario:** CEO says "ship the payments feature now." CRO says "not until the security audit clears." Both are right.

**How I handle it:**

1. **Quantify both sides** — "Shipping now = R2M revenue/month. Shipping without audit = R50M exposure if breached."
2. **Find the third option** — Feature flags. Ship to 5% of users behind a flag, run the audit in parallel.
3. **Own the recommendation** — "I recommend option 3. Here's why, here's the risk, and here's the rollback plan."
4. **48-hour escalation SLA** — If we can't resolve it, we escalate jointly to CEO/COO with a recommendation. No sandbagging, no unilateral vetoes.

^
At Discovery, I navigated this exact dynamic between Manulife's product ambitions and regulatory constraints across three markets. When the commercial case was clear and risk was bounded, I found a way to make it work — sometimes by conceding engineering priorities with a documented payback plan. The answer is never "pick a side" — it's "find the sequencing that serves both." This is the difference between a technical leader and an executive. Technical leaders solve engineering problems. Executives solve organisational ones — with data, sequencing, and the courage to make a recommendation and own it.

---

# Trade-off 1: Speed vs. Stability

**The call:** Invest in stability FIRST — it unlocks speed.

| Phase | Stability | Features |
|-------|-----------|----------|
| Months 1–3 | **70%** | 30% |
| Months 4–6 | 50% | 50% |
| Months 7+ | 30% | **70%** |

**Evidence:** At ABSA, halved cycle times by investing in DevOps practices first. DORA: elite performers ship 182x more frequently AND have 8x lower failure rates.

*If you want to go faster in 6 months, invest in the foundations today.*

---

# Trade-off 2: Build vs. Buy · Debt vs. Expansion

**Build vs. Buy** — Buy the commodity, build the differentiator.

| Buy | Build |
|-----|-------|
| API Gateway, IAM, Monitoring, CI/CD | Payment processing, Lending engine, KYC orchestration, Partner adapters |

**Debt vs. African Expansion** — Parallel tracks with a hard gate.

**Track 1 — Platform** (engineering) → Cloud to 50%+, multi-tenant, data residency, POPIA
**Track 2 — Market** (no eng dependency) → Regulatory analysis, partnerships, localisation

**Hard Gate — No launch until:** MTTR < 2 hrs · Deploy weekly · Critical bugs < 5/month

*Launching into new markets on an unstable platform risks losing both the new market AND the existing one.*

^
At Old Mutual, I used Auth0 rather than building IAM. At John Lewis, I advised on sunset vs. modernise. With 10 engineers, every hour matters — preserve capacity for what makes ABC unique. At Barclays ABSA, I designed architecture for digital banking across Africa. We sequenced on platform readiness, not market ambition alone.

---

# Why Me

**The ABSA Story:** No DevOps culture. Six siloed teams. Manual deployments. Engineers leaving. Sound familiar? Built the "Six Conditions for Transformation." **Result:** Halved cycle times. +5% engagement. 50% of teams with automated builds in 6 months. ARB still governing today.

**Proof across eight organisations:**
**Scaled:** ABSA (pan-African DevOps), Discovery/Manulife (multi-market), Accenture (delivery value chains)
**Migrated:** John Lewis (£1M/month losses → cloud-native), AXA (ML to production), Old Mutual (AWS + Auth0)
**Regulated:** Sanlam (de-merger architecture), Barclays ABSA (ARB governance), Discovery (cross-border compliance)

*Every recommendation in this deck comes from something I've shipped, scaled, or rescued.*

---

# What This Requires

| Investment Area | Year 1 | Year 2 | Payback |
|----------------|--------|--------|---------|
| **Headcount** (10 → 25) | R15–20M | R25–30M | Capacity to deliver R500M revenue target |
| **Tooling** (CI/CD, monitoring, security) | R2–3M | R1–2M | 60%+ reduction in MTTR and manual effort |
| **Cloud migration** | R3–5M | R2–3M | 20–30% infra cost reduction by month 18 |
| **Training & culture** | R500K–1M | R500K | Attrition 18% → <10% saves R3M+/year |

**Total Year 1: ~R22–29M · ROI: platform that supports R500M+ revenue at scale**

*This isn't a cost centre request — it's the investment required to unlock the board's growth ambitions.*

^
At Discovery, I built Capex/Opex models for Manulife leadership to justify exactly this kind of investment. The key is framing technology spend as revenue enablement, not overhead. Every rand here maps to a board-approved initiative.

---

# My Commitment

**90 Days** — Stabilised delivery. Quality gates. Partner confidence restored. Roadmap to EXCO.

**12 Months** — Weekly deploys. MTTR <2hrs. Cloud at 80%. Team at 20+. Country 1 live.

**24 Months** — Elite engineering. Full cloud-native. Two new markets. Real-time payments generating revenue.

---

![](https://images.pexels.com/photos/1287145/pexels-photo-1287145.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] Thank You

**Benjamin Hinson**
bhinson@plerk.co.za · 082 565 4665

> *"We cannot sacrifice quality for velocity or vice-versa.*
> *We can and must have both."*

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
