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
Good morning. I'm Benjamin Hinson. Over the past 20 years I've built, rescued, and scaled engineering organisations across financial services — from transforming DevOps culture at ABSA serving pan-African markets, to architecting cloud-native platforms at AXA and John Lewis, to leading delivery for North America's largest insurer at Discovery. Every recommendation today is grounded in what I've delivered in practice. Let me show you how I'd approach ABC Technologies.

---

# Agenda

1. **Diagnosis** — Where ABC stands today
2. **Strategic Priorities** — 12–24 month roadmap
3. **90-Day Plan** — Stabilise first, then accelerate
4. **Delivery & DevOps** — From inconsistent to elite
5. **Architecture & Scale** — Cloud-native, API-first
6. **AI & Data Platform** — Sequenced bets with data foundations
7. **Business Alignment** — One roadmap, one language
8. **Risk & Governance** — POPIA, partners, audit
9. **Engineering Culture** — Team, talent, comp & transformation
10. **Metrics & Flow** — What I'd track and why
11. **Stakeholders** — CEO, Product, Risk, Ops, Partners
12. **Hard Trade-offs** — The decisions that define us

---

![](https://images.pexels.com/photos/3912478/pexels-photo-3912478.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 1. Diagnosis
## Where ABC stands today

^
Conway's Law tells us organisations create systems that reflect their communication structures. Silos create barriers to velocity — informal structures form anyway, working around the process. When I led our DevOps transformation at ABSA, this was exactly the pattern we had to break. It's the same pattern at ABC. Let me show you the numbers.

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
At ABSA, I inherited the same pattern — siloed teams, no DevOps culture, manual processes. Within 12 months we halved cycle times. The fix isn't heroism — it's system design.

---

![](https://images.pexels.com/photos/7652039/pexels-photo-7652039.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 2. Strategic Priorities
## The 12–24 month roadmap

^
Strategy planning — mapping team structures, coaching cadence, delivery metrics, and maturity journeys. This is the real, messy work of transformation. At ABSA, I ran sessions exactly like this to map our path from silos to cross-functional delivery.

---

# Five Pillars — Phased for Reality

| Phase | Timeline | Focus |
|-------|----------|-------|
| **Stabilise** | Months 1–6 | Delivery predictability, incident response, quality gates |
| **Standardise** | Months 4–12 | Engineering standards, DevOps pipelines, architecture governance |
| **Scale** | Months 6–18 | Cloud-native migration, API-first platform, team growth to 25+ |
| **Accelerate** | Months 12–24 | New markets, new products, AI experimentation, innovation capacity |
| **Culture** | Continuous | High-performance engineering as the throughline |

These overlap deliberately. At AXA, I ran shadow deployments at 20% traffic while stabilising the main system. Parallel tracks, managed risk.

^
You don't wait for perfection before moving forward. At Barclays ABSA, I built a multi-year capability-based technology roadmap for digital banking across Africa. The lesson: sequence ruthlessly — you can't do everything at once with 10 people.

---

# Quarterly Roadmap

| Quarter | Stabilise | Standardise | Scale | Accelerate |
|---------|-----------|-------------|-------|------------|
| **Q1** | Incident mgmt, MTTR <2hrs | CI/CD baseline, code review 100% | Cloud roadmap | — |
| **Q2** | Deploy weekly, bugs <8 | Architecture Review Board | Microservices pilot | Country 1 prep |
| **Q3** | — | DevOps maturity L3 | Migration 60% | Country 1 launch |
| **Q4** | — | Continuous improvement | Migration 80%, API gateway | Real-time payments MVP, AI/ML pilot |

---

![](https://images.pexels.com/photos/3756042/pexels-photo-3756042.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 3. The 90-Day Plan
## All hands on deck

^
The first 90 days are a sprint — not a strategy offsite. Every step counts, every day matters. We're building a functioning system under pressure, with clear roles and precise handovers. Not a document — momentum.

---

# Days 1–30: Listen, Assess, Quick Wins

**Listen** — 1:1 with every engineer, PO, stakeholder. Shadow incidents and deployments. Review 6 months of production data. Meet the banking partner.

**Quick wins** — Daily cross-team standup (break silos). Mandatory code review — "Law of 4 Eyes". Incident war room with escalation paths. DORA metrics dashboard live.

**Sequencing principle** — Remove load before adding process. Contractors absorb BAU burden first. New practices roll in incrementally — not a big bang on day 31.

^
At ABSA, I called these the "Practices of Mastery" — five non-negotiable habits. You don't need a strategy document to start. Code review compliance alone typically reduces defect leakage by 30-40%. Critically, the existing team must feel relief before they feel new demands — otherwise transformation becomes just another burden on already-stretched people.

---

# Days 31–60: Structure & Standards

**Delivery** — "Two Product Principle": every sprint = customer value + technical improvement. Quality gates. Smaller batches → weekly releases. MTTR target: under 2 hours.

**Teams** — QA fully embedded. "You build it, you run it." Clear ownership of build, test, deploy, AND operate.

**Architecture** — API and service inventory. Top 5 tech debt items. Draft target-state architecture.

^
The Two Product Principle prevents the false choice between "features or debt." I developed this at ABSA — every release carries both customer value and technical improvements, by design.

---

# Days 61–90: Governance & Roadmap

**Governance** — Architecture Review Board. POPIA compliance checklist. Partner SLA framework. Monthly EXCO delivery dashboard.

**Roadmap** — Cloud migration plan to EXCO. Honest capacity planning. Hiring plan: 10 → 20–25 in 12 months. Build-vs-buy decisions.

**Culture** — Engineering guild. Blameless post-mortems. On-call rotation — no more heroics.

*By day 90: EXCO sees improving delivery, a credible roadmap, and a team that believes they can win.*

^
At Discovery, I ran monthly delivery reports to Manulife leadership tracking exactly these dimensions. Transparency builds trust.

---

![](https://images.pexels.com/photos/546819/pexels-photo-546819.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 4. Delivery & DevOps
## From inconsistent to elite

^
DevOps isn't a tool or a role — it's a culture. And it has to be built with the local context in mind. At ABSA, our transformation programme taught me that the code is only half the story. The other half is the system that surrounds it.

---

# DORA + Flow: The Full Picture

| DORA Metrics | Flow Metrics |
|-------------|-------------|
| Deploy Frequency → Are we shipping? | Cycle Time → How long is actual work? |
| Lead Time → How fast can we respond? | Wait Time → Where are we blocked? |
| MTTR → How resilient are we? | WIP → Are we overloaded? |
| Change Failure Rate → Are we shipping quality? | Flow Efficiency → Active time vs. wait time |

**The insight from Flow Engineering (Pereira & Davis):**
Reducing **wait time** — not work time — often cuts lead time by 80%+. The biggest gains come from eliminating queues, handoffs, and dependencies.

^
This is why I'd run a Value Stream Mapping exercise in the first 30 days. At AXA, I designed CI/CD pipelines that cut deployment lead times by 30% — most of that gain came from removing wait states, not making people work faster.

---

# The Practices of Mastery

**1. Check It In** — If it's not in source control, it doesn't exist
**2. Code Review** — Law of 4 Eyes. Every change. Syntax, semantics, mentoring
**3. Code Style** — Automated linting. Consistency by tooling, not willpower
**4. TDD** — Tests are the specification that keeps the system honest
**5. Automation** — Build, test, deploy, infra, ops. If humans repeat it, automate it

*These are the foundations that make everything else possible.*

^
I built this framework at ABSA. Target: 30% cross-functional with DevOps practices per sprint in year one, 50% with automated builds in 6 months. We hit both. These practices compound — each amplifies the others.

---

![](https://images.pexels.com/photos/4164418/pexels-photo-4164418.jpeg?auto=compress&cs=tinysrgb&w=1920)

# DevOps Maturity Phases

**Foundation (Months 1–3)** — CI for all repos. Code review gates. Basic monitoring. Coverage 45% → 60%.

**Acceleration (Months 4–9)** — CD with staging automation. Contract testing. Terraform IaC. Feature flags. Coverage 60% → 75%.

**Excellence (Months 10–18)** — Continuous deployment. Canary releases. Chaos engineering. Security scanning. Coverage 75% → 85%+.

^
Real engineering excellence lives in the code — collaboration through pull requests, automated pipelines, continuous integration. At ABSA, I built this culture from scratch. At AXA, I used shadow deployments at 20% traffic to validate ML models before full rollout.

---

# 5. Target Architecture — Cloud-native, API-first

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

# AI as a Product Differentiator

**Not a science project — a sequenced bet with guardrails.**

| Use Case | Value to ABC | Timeline | Approach |
|----------|-------------|----------|----------|
| **Credit scoring ML** | Faster, more accurate SME lending decisions | Q4 Y1 | Shadow model alongside existing rules — prove it before you switch |
| **Fraud & anomaly detection** | Reduce transaction fraud, lower partner risk | Y2 — gated on data readiness | Real-time event stream analysis on payments data |
| **AI-assisted KYC** | Cut onboarding from days to minutes | Y2 — gated on data readiness | Document extraction + identity verification automation |
| **Intelligent support** | Deflect 30–40% of support tickets | Y2 — gated on data readiness | LLM-powered triage on existing ticket data |

**Two gating principles:**
1. AI only ships on a stable platform — cloud-native + API-first gives us the pipelines and compute AI requires
2. Data readiness audit in first 60 days — if historical data isn't model-ready, timelines flex. Credit scoring ships first; others sequence based on data maturity

**Fallback:** If data isn't ready for ML, Country 1 launches with enhanced rule-based scoring. We iterate to ML as the data estate matures.

^
At AXA, I took ML models from research to production — shadow deployments at 20% traffic, automated retraining pipelines, and model governance. The lesson: AI without engineering discipline is a liability. AI on a well-architected platform is a competitive moat. The AI timeline is a target, not a commitment — the 60-day data readiness audit determines the real schedule. Honest assessment beats aspirational slide decks.

---

# Data Platform & Governance

**Infrastructure** — Data lake/lakehouse for analytical and ML workloads. Pipeline orchestration (dbt + Airflow). Feature store for model training. Schema registry for event contracts.

**Governance** — Data quality framework (Great Expectations). Full lineage and cataloguing. Model registry with explainability — critical for NCA lending compliance. Bias auditing and drift monitoring. Model risk committee co-owned with Data & Analytics and Compliance.

**Data residency** — POPIA (SA), NDPR (Nigeria), Kenya DPA — data localisation per market, built into architecture from day one. Model training constrained to permissible jurisdictions.

**Org placement** — Data engineering embedded in platform team. Joint planning with Data & Analytics in first 30 days to co-own the data strategy — not build a parallel silo.

^
This is the foundation that makes AI possible. At AXA, I learned that ML without data governance is a liability — shadow deployments and automated retraining only work when the data pipeline is trusted. The 60-day data readiness audit feeds directly into this: we assess data quality, identify gaps, and build the platform before we build models. Co-ownership with Data & Analytics is non-negotiable.

---

![](https://images.pexels.com/photos/3861957/pexels-photo-3861957.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 6. Business Alignment
## One roadmap, one language

^
The OAR model — Objective, Assumption, Reflection — a framework from my ABSA playbook, refined at Equal Experts. It's product thinking applied to technology decisions: Act on objectives, Orient around assumptions, Reflect on measures. Data-driven decision making is the throughline.

---

# Technology → R500M Revenue

**Objective** — What business outcome?
Real-time payments → new revenue. Cloud → 20–30% cost cut. API-first → faster partner integration.

**Assumption** — What must be true?
Team capacity (hence hiring). Partner adoption (validate early). Regulatory compatibility.

**Reflection** — How do we know we're wrong?
Monthly metrics. Partner feedback. Market validation before full launch.

^
The biggest mistake in engineering-led transformations is building technically excellent solutions that don't map to business outcomes. At Accenture, I benchmarked delivery value chains to ensure every tech investment had a clear line to priorities.

---

# Board Priorities → Technology Response

| Board Priority | Tech Response | Timeline | Outcome |
|---------------|---------------|----------|---------|
| 2 new countries | Multi-tenant, data residency | Q3–Q4 Y1 | Revenue diversification |
| Real-time payments | Event-driven microservice | Q4 Y1–Q2 Y2 | New product revenue |
| Cloud migration | Strangler fig, IaC | 18 months | 20–30% cost reduction |
| Partner confidence | SLA framework, monitoring | Q1 | Retain banking partner |
| Regulatory | POPIA automation, audit trails | Q1–Q2 | Licence to operate |
| Innovation & AI | ML credit scoring, fraud detection, AI-assisted KYC | Q4 Y1–Y2 | Product differentiation + operational efficiency |

---

# 7. Compliance Framework

**POPIA (Critical 2026)** — Information Officer. Data localisation per market. Breach notification automation. Consent management in KYC engine.

**Financial Services** — SARB payments alignment. AML controls. Transaction monitoring. Full audit trail.

**Governance** — Architecture Review Board (built and governed at Barclays ABSA). Change Advisory Board. Quarterly reporting. Annual pen testing.

---

# Banking Partner: Restore Trust

**Days 1–30** — Meet leadership. Joint incident review. Commit to SLAs. Dedicated monitoring.

**Days 30–90** — Automated health checks. Staging mirror. Monthly reviews. Shared milestones.

**Ongoing** — Status page. Quarterly business reviews. Joint DR testing.

*They don't need perfection on day one. They need a credible plan with measurable progress.*

^
At Discovery, I managed the Manulife partnership — aligning roadmaps, managing escalation, building trust through transparency.

---

![](https://images.pexels.com/photos/3184360/pexels-photo-3184360.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 8. Engineering Culture
## Building a high-performance team

^
Culture is built by teams, together. The ELSA model — Event, Language, Structure, Agency — from my ABSA transformation shows how: create the right events, which change the language, which changes the structure, which gives people agency. Culture isn't posters on walls — it's systems that shape behaviour.

---

# Scale: 10 → 25+ Engineers

| Team Type | Count | Role |
|-----------|-------|------|
| **Stream-Aligned** | 3 | Payments, Lending, KYC — own delivery end-to-end |
| **Platform** | 1 | CI/CD, infra, shared services — reduce cognitive load |
| **Enabling** | 1 (temp) | Upskill cloud-native/DevOps — then dissolve |

"You build it, you run it." Cross-functional. Embedded QA.

^
Team Topologies combined with what I built at ABSA. When I moved from silos to cross-functional teams, we halved cycle times.

---

# Fixing 18% Attrition — and Hiring 15+

**Retain** (fix the bleed first):
**Purpose** — Every sprint connects to R500M. Engineers in customer feedback.
**Autonomy** — Teams own backlog, architecture, deploys. Error budgets.
**Mastery** — Guilds. Conference budget. Blameless post-mortems.

**Hire** (build the pipeline):
**Months 1–3** — 3–4 senior contractors scoped to absorb BAU load (not create onboarding burden). Pre-built onboarding packs. Paired with existing engineers — existing team as anchors, not afterthoughts.
**Months 3–12** — Permanent hires. SA fintech talent pool + diaspora network. Engineering brand: tech blog, open-source, conference talks.
**Graduate pipeline** — Partner with WeThinkCode_, Umuzi, and 1–2 SA universities. Intern-to-hire by Year 2.

**If hiring lags** (contingency): prioritise stream-aligned teams over enabling team. Platform runs lean. Roadmap flexes — timelines move, commitments don't disappear.

**Target: 18% → <10% attrition · 10 → 25+ headcount in 12 months**

^
At Discovery, the biggest retention factor wasn't compensation — it was whether engineers felt their work mattered. For hiring, at ABSA I built the engineering brand from zero — community events, internal tech talks, open coaching sessions. That pipeline became self-sustaining. The contractor bridge is specifically designed to reduce load on existing staff, not add to it — they arrive with onboarding documentation and are scoped to tech debt and stability work where deep domain knowledge isn't required.

---

# Compensation, Career Paths & Transformation

**Compensation philosophy** — Match-to-lead SA market for key roles. Annual benchmarking against fintech and remote-international rates. Equity or long-term incentive scheme for senior hires — essential for a scale-up targeting R500M.

**Dual career ladder:**

| IC Track | Management Track |
|----------|-----------------|
| Senior Engineer | Team Lead |
| Staff Engineer | Engineering Manager |
| Principal Engineer | Director of Engineering |

Equivalent comp, seniority, and organisational influence at each level. Not a token title — a real track with decision-making authority.

**Employment Equity** — Diverse shortlists (minimum 50% designated groups). Structured interviews to reduce bias. Diverse panels. Contractor cohort demographic intentionality from day one. I own the EE targets personally — this is not delegated to HR.

**Existing team commitment** — Current team members are the anchors. They get first consideration for leadership roles in the new structure. Nobody who held this company together gets sidelined without a conversation and a real option.

^
Purpose, Autonomy, and Mastery are necessary but not sufficient — people also need to be fairly compensated and see a credible future. The IC track matters: at ABSA and Discovery, our best engineers didn't want to manage people, and losing them to management-only career paths was a retention failure. Stay interviews, not just exit interviews. Regular market benchmarking, not annual surprises.

---

![](https://images.pexels.com/photos/7652039/pexels-photo-7652039.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 9. Metrics & Flow
## What I'd track and why

^
Metrics and flow — the messy, real work of transformation. At ABSA, I mapped team structures, coaching cadence, maturity journeys, and delivery metrics to build a system that could measure and improve itself.

---

# Engineering Health Dashboard

| Category | Metrics | Purpose |
|----------|---------|---------|
| **DORA** | Deploy frequency, lead time, MTTR, change failure rate | Delivery performance |
| **Flow** | Cycle time, wait time, WIP, flow efficiency | Where waste lives |
| **Business** | On-time delivery, support tickets, uptime, revenue enabled | Value delivery |
| **People** | Attrition, eNPS, on-call burden, learning days | Culture health |

**Key insight:** Most teams discover 80%+ of lead time is **waiting**, not working. The biggest gains come from eliminating queues and handoffs — not making people work faster.

^
At AXA: real-time dashboards with probabilistic forecasting — 15% better predictability, 20% faster approvals. Every metric has a clear owner and target. The Three Loops model from Flow Engineering gives us the framework: Inner Loop for developer experience, Middle Loop for team flow, Outer Loop for business outcomes.

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

---

# 10. Stakeholder Communication

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

1. **Quantify both sides** — "Shipping now = R2M revenue/month. Shipping without audit = R50M exposure if breached." Now EXCO can decide with data, not politics.
2. **Find the third option** — Feature flags. Ship to 5% of users behind a flag, run the audit in parallel. CEO gets momentum, CRO gets controls.
3. **Own the recommendation** — "I recommend option 3. Here's why, here's the risk, and here's the rollback plan."
4. **48-hour escalation SLA** — If Product and Engineering can't resolve a priority conflict within 48 hours, we escalate jointly to CEO/COO with a recommendation. No sandbagging, no unilateral vetoes.

*At Discovery, I navigated this exact dynamic between Manulife's product ambitions and regulatory constraints across three markets. When the commercial case was clear and risk was bounded, I found a way to make it work — sometimes by conceding engineering priorities with a documented payback plan. The answer is never "pick a side" — it's "find the sequencing that serves both."*

^
This is the difference between a technical leader and an executive. Technical leaders solve engineering problems. Executives solve organisational ones — with data, sequencing, and the courage to make a recommendation and own it.

---

![](https://images.pexels.com/photos/1094545/pexels-photo-1094545.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 11. Hard Trade-offs
## The decisions that define us

^
The road ahead isn't always clear. In any transformation, there are moments where you have to make a call that not everyone will agree with — and own the consequences. Here are the three I expect to face at ABC, and my position on each.

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

# Trade-off 2: Build vs. Buy

**The call:** Buy the commodity. Build the differentiator.

| Buy | Build |
|-----|-------|
| API Gateway (Kong/Apigee) | Payment processing logic |
| IAM (Auth0/Azure AD B2C) | Lending decision engine |
| Monitoring (Datadog/Grafana) | KYC workflow orchestration |
| CI/CD (GitHub Actions) | Partner integration adapters |

*Preserve engineering capacity for what makes ABC unique in the market.*

^
At Old Mutual, I used Auth0 rather than building IAM. At John Lewis, I advised on sunset vs. modernise. With 10 engineers, every hour matters.

---

# Trade-off 3: Debt vs. African Expansion

**The call:** Parallel tracks with a hard gate.

**Track 1 — Platform** (engineering) → Cloud to 50%+, multi-tenant, data residency, POPIA

**Track 2 — Market** (no eng dependency) → Regulatory analysis, partnerships, localisation

**Hard Gate — No launch until:**
MTTR < 2 hrs · Deploy weekly · Critical bugs < 5/month

*Launching into new markets on an unstable platform risks losing both the new market AND the existing one.*

^
At Barclays ABSA, I designed architecture for digital banking across Africa. We sequenced on platform readiness, not market ambition alone.

---

![](https://images.pexels.com/photos/839428/pexels-photo-839428.jpeg?auto=compress&cs=tinysrgb&w=1920)

# [fit] 12. Why Me

^
Strategy meets execution. In every transformation, you need someone who's played the game before — who knows the moves, anticipates the counter-moves, and can think several steps ahead. Unicorns aren't born — they're built. By people who do the hard, unglamorous work of fixing foundations, building systems, and creating culture where extraordinary outcomes become ordinary.

---

# The ABSA Story

When I arrived, there was no DevOps culture. Six siloed teams. Manual deployments. Engineers leaving. Sound familiar?

**What I did:** Built the "Six Conditions for Transformation" — starting with Conway's Law, restructuring teams for flow. Introduced the Practices of Mastery. Created community through coaching, guilds, and blameless post-mortems.

**The result:** Halved cycle times. +5% engagement. 50% of teams with automated builds within 6 months. Architecture Review Board that's still governing today.

**Why it matters for ABC:** Every challenge in this case study — silos, attrition, inconsistent DevOps, scaling across Africa — is one I've already solved. Not in theory. In practice.

---

# Proof Across Eight Organisations

**Scaled delivery:** ABSA (pan-African DevOps), Discovery/Manulife (multi-market at scale), Accenture (delivery value chains)

**Migrated platforms:** John Lewis (£1M/month losses → cloud-native), AXA (ML to production, 30% faster deploys), Old Mutual (AWS + Auth0 CIAM)

**Navigated regulation:** Sanlam (de-merger architecture), Barclays ABSA (ARB governance), Discovery (cross-border compliance)

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

*This isn't a cost centre request — it's the investment required to unlock the board's growth ambitions. Without it, we're scaling on a foundation that's already cracking.*

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

