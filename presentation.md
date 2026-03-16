theme: Ostrich, 1
footer: Benjamin Hinson | Executive Head: Software Development — ABC Technologies Case Study
slidenumbers: true
autoscale: true

---

[.background-color: #103554]
[.header: #FFFFFF]
[.text: #FFFFFF]

# Stabilise. Scale. Accelerate.
## A Strategic Blueprint for ABC Technologies

**Benjamin Hinson**
Executive Head: Software Development

March 2026

^
Good morning. I'm Benjamin Hinson. Over the past 20 years I've built, rescued, and scaled engineering organisations across financial services — from transforming DevOps culture at ABSA serving pan-African markets, to architecting cloud-native platforms at AXA and John Lewis, to leading delivery for North America's largest insurer at Discovery. Today I'll walk you through how I would approach the challenges at ABC Technologies. This is not a theoretical exercise — every recommendation I'll share is grounded in what I've delivered in practice.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]
[.text: #FFFFFF]

# Agenda

1. **Diagnosis** — Where ABC stands today
2. **Strategic Priorities** — 12–24 month roadmap
3. **90-Day Action Plan** — Stabilise first, then accelerate
4. **Delivery & DevOps Maturity** — From inconsistent to elite
5. **Architecture & Scalability** — Cloud-native, API-first
6. **Technology–Business Alignment** — One roadmap, one language
7. **Risk, Compliance & Governance** — POPIA, partners, auditability
8. **Engineering Culture** — Building a high-performance team
9. **Key Metrics** — What I'd track and why
10. **Stakeholder Management** — CEO, Product, Risk, Ops, Partners
11. **Hard Trade-offs** — The decisions that define us
12. **Why Me** — Proof points from 20+ years

^
I've structured this to follow the brief precisely. We'll start with diagnosis, move through strategy, and end with the hard trade-offs that any incoming executive must be prepared to navigate.

---

[.background-color: #FFFFFF]
[.header: #103554]

# 1. Diagnosis
## The Current State of ABC Technologies

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Reading the Vital Signs

| Metric | Current State | Industry Benchmark |
|--------|--------------|-------------------|
| On-time delivery | **62%** | 85%+ (high performers) |
| Critical bugs/month | **18** | <5 |
| MTTR | **6–10 hours** | <1 hour (elite) |
| Deploy frequency | **Every 2–3 weeks** | Daily/weekly |
| Test automation | **~45%** | 75%+ |
| Cloud migration | **25%** | Target: 100% |
| Engineering attrition | **18%** | <10% |
| Support tickets | **Up 40%** | Declining trend |

^
Let me be direct: these numbers tell the story of an organisation that has outgrown its engineering foundations. This is not a talent problem — this is a systems problem. At ABSA, I inherited similar metrics and within 12 months halved cycle times while increasing quality. The pattern here is one I've seen and resolved before.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Root Cause Analysis

**The core issue isn't technical — it's structural and cultural.**

**Structural Debt:**
Silos between 4 product teams and 2 platform teams mean handoffs multiply, context is lost, and nobody owns the full delivery pipeline end-to-end.

**Process Debt:**
Inconsistent code reviews, partial QA embedding, and mixed Agile maturity mean quality is a lottery rather than a system property.

**Architectural Debt:**
At 25% cloud migration with a monolithic heritage, every new feature risks destabilising the existing platform.

**Cultural Debt:**
18% attrition signals that engineers don't see a clear path to mastery, purpose, or autonomy — the three intrinsic motivators that retain top talent.

^
I learned this framework at ABSA — we called it the "Six Conditions for Transformation." Condition number one is Conway's Law: your org structure is a product of history, and silos beget supervision, which begets process. ABC is shipping its org chart. The good news? This is fixable — and I've done it before.

---

[.background-color: #103554]
[.header: #FFFFFF]
[.text: #FFFFFF]

# The Compounding Pressure

```
  CEO → "Ship faster"          CRO → "Lower risk"
          ↘                       ↙
      ┌────────────────────────────┐
      │   ENGINEERING TEAM (10)     │
      │   Caught in the middle      │
      └────────────────────────────┘
          ↗                       ↖
  CPO → "Innovate more"       COO → "Be predictable"

  + Banking partner threatening penalties
  + Board approved: 2 new countries + new product + cloud migration
```

The team is pulled in four directions while carrying technical debt, compliance pressure, and an ambitious growth agenda — all with 10 engineers.

^
This is the classic scale-up trap. You've succeeded because of scrappy, heroic effort. But heroics don't scale. What scales is systems, standards, and culture. My job is to build the system that lets talented people do their best work without burning out.

---

[.background-color: #FFFFFF]
[.header: #103554]

# 2. Strategic Priorities
## The 12–24 Month Roadmap

---

[.background-color: #F1B52F]
[.header: #103554]
[.text: #103554]

# Five Strategic Pillars

## Months 1–6: **Stabilise**
Foundation-setting — delivery predictability, incident response, quality gates

## Months 4–12: **Standardise**
Engineering standards, DevOps pipelines, architecture governance

## Months 6–18: **Scale**
Cloud-native migration, API-first platform, team growth to 25+

## Months 12–24: **Accelerate**
New markets, new products, innovation capacity

## Continuous: **Culture**
High-performance engineering culture as the throughline

^
These overlap deliberately. You don't wait for perfection before moving forward. At AXA, I ran shadow deployments at 20% traffic while the main system was still stabilising — we validated the new ML pricing model without risking production. The same principle applies here: parallel tracks, managed risk.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Strategic Priority Map

```
Quarter    Stabilise          Standardise         Scale              Accelerate
─────────────────────────────────────────────────────────────────────────────────
Q1         Incident mgmt      CI/CD baseline      Cloud roadmap      ─
           Quality gates      Code review 100%    API inventory
           MTTR < 2hrs        Test automation↑

Q2         Deploy weekly      Architecture         Microservices      Country 1
           Bug rate < 8       review board         pilot              prep
           Partner SLAs       POPIA audit

Q3         ─                  DevOps maturity      Migration 60%      Country 1
                              L3 across teams      Platform team      launch
                                                   scaled

Q4         ─                  Continuous            Migration 80%      Real-time
                              improvement           API gateway        payments
                              embedded              live               MVP
─────────────────────────────────────────────────────────────────────────────────
Year 2     Operational        Engineering           Migration          2nd country
           excellence         excellence            complete           + scale
```

^
This is not aspirational — it's sequenced based on dependencies and what I've seen work in similar transformations. At Barclays ABSA, I built a multi-year capability-based technology roadmap for digital banking across Africa. The key lesson: you must sequence ruthlessly because you can't do everything at once with 10 people.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 3. The 90-Day Plan
## First Things First

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Days 1–30: Listen, Assess, Quick Wins

**Listen & Learn**
- 1:1s with every engineer, product owner, and key stakeholder
- Shadow incident response and deployment processes
- Review last 6 months of production incidents and delivery data
- Understand the banking partner's specific pain points

**Quick Wins — Immediate Impact**
- Establish a daily stand-up across all teams (break silos)
- Implement mandatory code review policy (the "Law of 4 Eyes" from my ABSA playbook)
- Create a production incident war room with clear escalation paths
- Set up basic DORA metrics dashboard (deploy frequency, lead time, MTTR, change failure rate)

^
At ABSA, I called this the "Practices of Mastery" — five non-negotiable habits: check it in, code review, code style, TDD, and automation. You don't need a strategy document to start these. You need a decision and a Monday morning. Within the first month I'd have code review compliance at 100% — this alone typically reduces defect leakage by 30-40%.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Days 31–60: Structure & Standards

**Delivery Stabilisation**
- Implement the "Two Product Principle" — every sprint delivers customer value AND technical improvement
- Establish quality gates: no deployment without automated tests, code review, and staging validation
- Reduce deployment batch sizes to enable weekly releases
- Target: MTTR from 6–10 hours → under 2 hours

**Team Restructuring**
- Move QA from partially embedded to fully embedded in each team
- Assign clear ownership: each product team owns build, test, deploy, AND operate
- Introduce "you build it, you run it" accountability

**Architecture Foundation**
- Complete API and service inventory
- Identify the top 5 technical debt items blocking delivery
- Draft target-state architecture aligned to cloud-native, API-first vision

^
The Two Product Principle is something I developed at ABSA. Every release must carry both customer-facing value AND technical improvements. They're equally important but not always equal effort. This prevents the false choice between "features or debt" — you do both, every sprint, as a discipline.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Days 61–90: Governance & Roadmap

**Governance Framework**
- Establish Architecture Review Board (I created and governed this at Barclays ABSA for pan-African banking)
- Implement POPIA compliance checklist for every data-touching feature
- Create partner SLA framework with the banking partner — move from reactive to proactive
- Monthly delivery dashboards to EXCO (format proven at Discovery for Manulife)

**Technology Roadmap Delivery**
- Present cloud migration roadmap to EXCO with phased milestones
- Align product roadmap with technical capacity — honest about what 10 engineers can deliver
- Propose hiring plan to scale team to 20–25 over 12 months
- Define build-vs-buy decisions for key platform components

**Culture Foundation**
- Launch engineering guild for cross-team knowledge sharing
- Introduce blameless post-mortems (Google SRE model)
- Establish on-call rotation with clear escalation — no more heroics

^
By day 90, EXCO should see: delivery predictability improving, incident response times dropping, a clear roadmap they can hold me accountable to, and engineers who are energised rather than burning out. At Discovery, I ran monthly delivery reports to the Manulife leadership that tracked exactly these dimensions. Transparency builds trust.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]

# 4. Delivery, Quality & DevOps Maturity
## From Inconsistent to Predictable

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# The DORA Framework: Our North Star

| Metric | ABC Today | Target (12 months) | Elite Benchmark |
|--------|-----------|-------------------|-----------------|
| **Deploy Frequency** | Every 2–3 weeks | Weekly → Daily | On demand |
| **Lead Time for Changes** | Weeks | Days | < 1 hour |
| **MTTR** | 6–10 hours | < 2 hours | < 1 hour |
| **Change Failure Rate** | High (est. 25%+) | < 10% | < 5% |

Elite performers deploy **182x** more frequently and recover **2,293x** faster than low performers.
— *2024 DORA State of DevOps Report*

^
These aren't aspirational targets — they're achievable. At AXA, I designed CI/CD pipelines that cut deployment lead times by 30% and reduced errors by 25%. The key insight from DORA research is that speed and stability are NOT trade-offs — elite performers achieve both simultaneously. The secret is automation, small batch sizes, and fast feedback loops.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# The Practices of Mastery
## Five Non-Negotiable Engineering Habits

**1. Check It In** — Version control everything. Code, config, infrastructure. If it's not in source control, it doesn't exist.

**2. Code Review (Law of 4 Eyes)** — Every change reviewed before merge. Not just syntax — semantics, mentoring, and learning. This is how standards propagate.

**3. Code Style** — Automated linting and formatting. Local conventions enforced by tooling, not willpower. Consistency reduces cognitive load.

**4. Test-Driven Development** — Verify customer value at the code level. Tests are not overhead — they're the specification that keeps the system honest.

**5. Automation** — Build, test, deploy, infrastructure, operations. If a human is doing it repeatedly, automate it. This is how you scale from 10 to 30 engineers without chaos.

^
I built this framework at ABSA. The target was 30% of teams cross-functional with at least one DevOps improvement per sprint within the first year, and 50% of teams with automated builds and code review within 6 months. We hit both. These practices compound — each one amplifies the others.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# DevOps Maturity Roadmap

**Phase 1 — Foundation (Months 1–3)**
- CI pipelines for all repositories (automated build + unit tests)
- Mandatory code review gates in pull request workflows
- Basic monitoring and alerting on production systems
- Test automation coverage: 45% → 60%

**Phase 2 — Acceleration (Months 4–9)**
- CD pipelines with automated staging deployments
- Integration and contract testing between services
- Infrastructure as Code (Terraform) for all new environments
- Feature flags for progressive rollouts
- Test automation coverage: 60% → 75%

**Phase 3 — Excellence (Months 10–18)**
- Full continuous deployment with canary releases
- Chaos engineering and disaster recovery testing
- Automated security scanning (SAST/DAST) in pipeline
- Self-service platform for developer environments
- Test automation coverage: 75% → 85%+

^
At AXA, I used shadow deployments — routing 20% of traffic to new ML models before full rollout. This approach validated pricing accuracy while protecting production. I'd apply the same progressive delivery pattern here: feature flags, canary releases, and shadow mode for the real-time payments product.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 5. Architecture, Scalability & Security
## Cloud-Native, API-First

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Target Architecture Vision

```
                    ┌──────────────────────────────────────┐
                    │          API Gateway (Kong/Apigee)     │
                    │     Rate limiting · Auth · Routing      │
                    └──────────┬───────────┬─────────────────┘
                               │           │
              ┌────────────────┤           ├────────────────┐
              ▼                ▼           ▼                ▼
     ┌──────────────┐  ┌────────────┐  ┌──────────┐  ┌──────────────┐
     │   Payments    │  │  Lending   │  │   KYC    │  │  Integration │
     │   Service     │  │  Service   │  │  Engine  │  │   Gateway    │
     │  (Domain)     │  │  (Domain)  │  │ (Domain) │  │  (Banking)   │
     └──────┬───────┘  └─────┬──────┘  └────┬─────┘  └──────┬───────┘
            │                │              │                │
            └────────────────┴──────────────┴────────────────┘
                               │
                    ┌──────────┴───────────┐
                    │    Platform Services   │
                    │  Events · Auth · Audit │
                    │  Config · Monitoring   │
                    └──────────────────────┘
                               │
                    ┌──────────┴───────────┐
                    │  Cloud Infrastructure  │
                    │  Kubernetes · IaC      │
                    │  CI/CD · Observability  │
                    └──────────────────────┘
```

^
This is Domain-Driven Design applied to ABC's product portfolio. Each domain — payments, lending, KYC, integrations — becomes an independently deployable service with clear API contracts. This is the pattern I used at Barclays ABSA for pan-African digital banking: each country could consume shared services while maintaining local compliance requirements. It's also how I approached the monolith-to-microservices transformation at John Lewis.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Cloud Migration Strategy
## From 25% to Full Cloud-Native

**Approach: Strangler Fig Pattern — not big-bang**

**Phase 1: Lift & Stabilise (Months 1–6)**
- Containerise existing services (Docker + Kubernetes)
- Establish cloud infrastructure baseline (IaC with Terraform)
- Migrate non-critical services first to build team confidence
- Target: 25% → 50% migrated

**Phase 2: Decompose & Modernise (Months 6–12)**
- Extract payment processing into independent microservice
- Build API gateway for partner integrations
- Implement event-driven architecture for real-time capabilities
- Target: 50% → 75% migrated

**Phase 3: Optimise & Scale (Months 12–18)**
- Complete migration of core systems
- Auto-scaling for multi-country deployment
- Multi-region deployment for African expansion
- Target: 75% → 95%+ migrated

^
At John Lewis, I led the legacy-to-modern platform migration while safeguarding business continuity. The critical lesson: never migrate and rebuild simultaneously. Use the Strangler Fig pattern — wrap the legacy system, route new traffic to new services, and gradually retire the old. At Equal Experts we saved John Lewis from a product that was losing £1M/month by using exactly this approach.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Security by Design

**Application Security**
- SAST/DAST scanning integrated into every CI/CD pipeline
- Dependency vulnerability scanning (Snyk/Dependabot)
- API security: OAuth 2.0, rate limiting, input validation
- Secrets management (HashiCorp Vault or Azure Key Vault)

**Infrastructure Security**
- Zero-trust network architecture
- Encryption at rest and in transit (TLS 1.3)
- Container image scanning before deployment
- Immutable infrastructure — no manual changes to production

**Compliance & Audit**
- Full audit trail on every data access and modification
- Automated compliance checks in deployment pipeline
- Regular penetration testing (quarterly)
- Incident response playbook with regulatory notification procedures

^
In fintech, security isn't a feature — it's a licence to operate. At Old Mutual, I integrated Auth0-based CIAM for enterprise-grade security on the banking platform. At Sanlam, I aligned architecture decisions with regulatory requirements during the de-merger. Security and compliance need to be automated into the pipeline, not bolted on after the fact.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]

# 6. Technology–Business Alignment
## One Roadmap, One Language

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Aligning Technology to R500M Revenue Target

**The OAR Model — Objective, Assumption, Reflection**

Every technology initiative must answer three questions:

**Objective:** What customer or business outcome does this enable?
- Real-time payments → new revenue stream + competitive differentiation
- Cloud migration → operational cost reduction of 20–30% + scalability for new markets
- API-first → faster partner integration → faster time-to-revenue

**Assumption:** What must be true for this to work?
- The team has capacity to deliver migration AND new features (they don't yet — hence hiring plan)
- Partners will adopt new APIs (validate early with banking partner)
- Regulatory requirements in new markets are compatible with our architecture

**Reflection:** How will we know if we're wrong?
- Monthly metrics review against roadmap
- Partner feedback loops
- Market validation before full country launch

^
I developed this product-thinking approach at ABSA and refined it at Equal Experts. The biggest mistake I see in engineering-led transformations is building technically excellent solutions that don't map to business outcomes. At Accenture, I benchmarked delivery value chains to ensure every technology investment had a clear line to business priorities. That same discipline applies here.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Roadmap Alignment to Board Priorities

| Board Priority | Technology Response | Timeline | Business Outcome |
|---------------|-------------------|----------|-----------------|
| **2 new countries** | Multi-tenant architecture, data residency | Q3–Q4 Y1 | Revenue diversification |
| **Real-time payments** | Event-driven microservice, API gateway | Q4 Y1 – Q2 Y2 | New product revenue |
| **Cloud-native migration** | Strangler fig, containerisation, IaC | Continuous 18 months | 20–30% cost reduction |
| **Partner confidence** | SLA framework, incident response, monitoring | Q1 immediate | Retain banking partner |
| **Regulatory compliance** | POPIA automation, audit trails, security | Q1–Q2 foundation | Licence to operate |

^
The 2026 POPIA data localisation enforcement deadline is critical for the African expansion. Fintechs without in-country cloud zones will face operational risk. I'd ensure our cloud architecture supports multi-region data residency from day one — this is an architectural decision that's expensive to retrofit.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 7. Risk, Compliance & Governance
## POPIA, Partners, Auditability

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Regulatory & Compliance Framework

**POPIA Compliance (Critical for 2026)**
- Appoint and register Information Officer with the Information Regulator
- Data localisation: ensure cloud architecture supports in-country data zones for each market
- Mandatory breach notification "as soon as reasonably sure"
- Consent management built into KYC & onboarding engine
- Regular data protection impact assessments

**Financial Services Compliance**
- SARB payments ecosystem modernisation programme alignment
- Anti-money laundering (AML) controls in lending and payments
- Transaction monitoring and suspicious activity reporting
- Audit trail requirements for every financial transaction

**Partner & Regulatory Governance**
- Architecture Review Board for all infrastructure and solution designs
- Change Advisory Board for production deployments
- Quarterly compliance reporting to board
- Annual penetration testing and vulnerability assessments

^
At Barclays ABSA, I created and governed the Architecture Review Board ensuring all designs aligned with the future-state vision across Africa. At Sanlam, I navigated regulatory requirements during a complex de-merger. Governance isn't bureaucracy when it's well-designed — it's the framework that lets you move fast with confidence.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Risk Mitigation for the Banking Partner

**Immediate Actions (Days 1–30)**
- Meet the banking partner leadership to understand specific pain points
- Establish joint incident review process
- Define and commit to measurable SLAs (uptime, response time, resolution time)
- Implement dedicated monitoring for partner-facing integration points

**Medium-term (Days 30–90)**
- Automated health checks and alerting on integration endpoints
- Staging environment that mirrors partner integration for pre-deployment validation
- Monthly partner technical review meetings
- Penalty avoidance plan with clear milestones shared with partner

**Ongoing**
- Real-time status page for partner visibility
- Quarterly business reviews with technical deep-dives
- Joint disaster recovery testing

^
This is stakeholder management 101 for a critical relationship. At Discovery, I managed the Manulife partnership across North America — aligning roadmaps to partner-market expectations, managing incident escalation, and building trust through transparency. The banking partner doesn't need perfection on day one. They need to see a credible plan with measurable progress.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]

# 8. Engineering Culture
## Building a High-Performance Team

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Scaling from 10 to 25+ Engineers

**Team Topology Evolution (Team Topologies Framework)**

**Today: 10 people**
- 4 product teams + 2 platform teams + 1 QA = stretched thin, siloed

**Target: 20–25 people (12 months)**
- 3 Stream-Aligned Teams (payments, lending, KYC/onboarding) — own value delivery end-to-end
- 1 Platform Team — CI/CD, infrastructure, shared services, reducing cognitive load on delivery teams
- 1 Enabling Team (temporary) — upskill teams on cloud-native, DevOps practices, then dissolve

**Key Principles**
- "You build it, you run it" — full ownership reduces handoffs
- Cross-functional teams with embedded QA
- Minimise cognitive load through platform abstractions
- Chapters for discipline excellence (backend, frontend, DevOps) across squads

^
This draws directly from Team Topologies — the four fundamental team types — combined with what I built at ABSA. The critical insight is that platform teams exist to reduce cognitive load on stream-aligned teams, not just to centralise infrastructure. When I restructured teams at ABSA, we moved from functional silos to cross-functional product teams and halved cycle times.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Culture Levers: Purpose, Autonomy, Mastery

**Purpose — Connect engineers to business impact**
- Every sprint review includes the "so what" — how this feature moves the R500M needle
- Engineers participate in customer feedback sessions
- Quarterly all-hands with CEO connecting technology work to company mission

**Autonomy — Trust teams to make decisions**
- Stream-aligned teams own their backlog, architecture, and deployment
- Error budgets (Google SRE model) — teams choose how to spend their reliability budget
- 10% time for technical exploration and innovation

**Mastery — Create a path to excellence**
- Engineering guilds for cross-team learning
- Conference budget and learning days
- Internal tech talks and knowledge sharing
- Clear career ladder: IC and management tracks
- Blameless post-mortems — every failure is a learning opportunity

^
At ABSA, we articulated this as "Mastery is the pursuit of excellence" — driven by Purpose, Autonomy, and Mastery as intrinsic motivators. The 18% attrition at ABC tells me engineers don't see these elements in their current environment. People don't leave companies — they leave environments where they can't grow. Fix the environment and attrition drops.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Tackling 18% Attrition

**Root Causes (Typical at This Stage)**
- No clear career progression
- Heroic on-call culture leading to burnout
- Siloed work limiting learning
- Technical debt making daily work frustrating
- Lack of modern tooling and practices

**My Playbook**
- Implement structured on-call rotation with compensatory time (no more heroes)
- Pair programming and mob programming sessions weekly
- Dedicated tech debt sprint capacity (Two Product Principle — every sprint)
- Modern tooling: upgrade CI/CD, developer experience, local dev environments
- Transparent career framework within 90 days
- Regular skip-level 1:1s so I hear concerns early

**Target: 18% → <10% within 12 months**

^
At Discovery, I managed engineering teams delivering complex features for Manulife. The single biggest factor in retention wasn't compensation — it was whether engineers felt their work mattered and whether they were growing. Create those conditions and your best people stay.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 9. Key Metrics
## What I'd Track and Why

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Engineering Health Dashboard

**DORA Metrics (Delivery Performance)**
- Deployment Frequency → Are we shipping faster?
- Lead Time for Changes → How quickly can we respond to the market?
- Mean Time to Recovery → How resilient are we?
- Change Failure Rate → Are we shipping quality?

**Flow Metrics (Delivery Predictability)**
- Cycle Time → How long from start to customer delivery?
- Throughput → How many items completed per sprint?
- Work in Progress → Are we overloaded? (Little's Law)
- Flow Efficiency → Active time vs. wait time

**Business Metrics (Value Delivery)**
- On-time delivery percentage (62% → 85%+)
- Customer support ticket trend (down 40%)
- Platform uptime / SLA compliance
- Revenue enabled by technology (new products, new markets)

**People Metrics (Culture Health)**
- Engineering attrition (18% → <10%)
- Employee NPS / engagement score
- On-call burden per engineer
- Learning investment (training days per engineer per quarter)

^
At AXA, I built real-time dashboards with probabilistic forecasting that improved predictability by 15% and accelerated approvals by 20%. The key is not just measuring — it's making metrics visible and actionable. Every metric on this dashboard has a clear owner and a target. I'd review these weekly with the team and monthly with EXCO.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# 12-Month Metric Targets

| Category | Metric | Current | 6 months | 12 months |
|----------|--------|---------|----------|-----------|
| **Delivery** | On-time delivery | 62% | 75% | 85%+ |
| **Delivery** | Deploy frequency | 2–3 weeks | Weekly | 2x/week |
| **Quality** | Critical bugs/month | 18 | <8 | <3 |
| **Quality** | Test automation | 45% | 65% | 80% |
| **Resilience** | MTTR | 6–10 hrs | <2 hrs | <1 hr |
| **People** | Attrition | 18% | 14% | <10% |
| **Platform** | Cloud migration | 25% | 55% | 80% |
| **Compliance** | Code review | Inconsistent | 100% | 100% |

^
These targets are aggressive but achievable. At ABSA, we set comparable targets — 30% of teams cross-functional with DevOps practices within the first year, 50% with automated builds and code reviews within 6 months — and hit them. The key is making them visible, celebrating progress, and using retrospectives to course-correct.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]

# 10. Stakeholder Management
## CEO, Product, Risk, Ops, Partners

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Stakeholder Communication Framework

| Stakeholder | Their Priority | My Approach | Cadence |
|------------|---------------|-------------|---------|
| **CEO** | Faster time-to-market | Show deploy frequency + lead time improvements. Honest capacity planning. | Weekly 1:1 |
| **CPO** | Innovation & experimentation | 10% innovation time. Feature flags for safe experimentation. Product-tech roadmap alignment. | Weekly sync |
| **CRO** | Lower risk, stronger controls | Architecture Review Board. Automated compliance. Audit trail dashboards. | Bi-weekly |
| **COO** | Predictability & reliability | DORA metrics dashboard. SLA tracking. Incident trend reporting. | Weekly ops review |
| **Banking Partner** | No more outages | Dedicated monitoring. Joint incident review. Monthly technical reviews. | Monthly + ad-hoc |
| **Board/EXCO** | Confidence in technology | Monthly delivery report. Quarterly roadmap review. Transparent metrics. | Monthly report |

^
At Discovery, I managed stakeholders across John Hancock and Manulife — aligning roadmaps to partner-market expectations across time zones and cultures. The principle is the same: different stakeholders need different views of the same data. The CEO wants the business impact. The CRO wants the risk posture. The COO wants the operational metrics. One dashboard, multiple lenses.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Managing Competing Priorities

**The key insight: these are not contradictions — they're sequencing problems.**

**Speed AND Stability** — Small batch sizes with automated testing. You ship faster BECAUSE you have quality gates, not despite them. (DORA research proves this.)

**Innovation AND Control** — Feature flags + error budgets. Innovate within a defined risk envelope. If the error budget is consumed, freeze features and fix reliability.

**Growth AND Governance** — Cloud-native architecture with compliance built into the pipeline. Governance becomes automated, not manual overhead.

**The conversation I'd have with EXCO:**
"I can give you all four — but not all at once. Here's the sequence, here's why, and here's how we'll measure progress. Hold me accountable to these metrics."

^
This is the hardest part of the role — managing expectations honestly. At IQbusiness, I operated across the full architecture spectrum — business architecture at Bridgestone, enterprise at Eskom, application at Sanlam. Every engagement taught me that the most valuable thing a technology leader brings to EXCO is clarity about trade-offs, not promises about everything.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 11. Hard Trade-off Decisions
## The Choices That Define Us

---

[.background-color: #F1B52F]
[.header: #103554]
[.text: #103554]

# Trade-off 1: Speed vs. Stability

**The Tension:** CEO wants faster delivery. COO and banking partner need stability. With only 10 engineers, every hour spent on new features is an hour not spent on reliability.

**My Position:** Invest in stability FIRST because it unlocks speed.

**The Evidence:**
- At ABSA, I halved project cycle times by investing in DevOps practices first — TDD, CI/CD, code review. Speed came from quality, not from cutting corners.
- DORA research: elite performers ship 182x more frequently AND have 8x lower failure rates.

**The Decision Framework:**
- Months 1–3: 70% stability / 30% features
- Months 4–6: 50% stability / 50% features
- Months 7+: 30% stability / 70% features

As the platform stabilises, feature velocity naturally accelerates.

^
This is the conversation the CEO needs to hear. "If you want to go faster in 6 months, you need to invest in the road today." Every experienced engineering leader has had this conversation. The data is unambiguous: quality gates accelerate delivery over any meaningful time horizon.

---

[.background-color: #F1B52F]
[.header: #103554]
[.text: #103554]

# Trade-off 2: Build vs. Buy

**The Tension:** With 10 engineers, building everything custom is impossible. But buying introduces vendor lock-in and may not fit fintech regulatory requirements.

**My Position:** Buy the commodity, build the differentiator.

**Buy (Platform Components):**
- API Gateway (Kong, Apigee) — don't build routing and rate limiting
- Identity & Access Management (Auth0, Azure AD B2C) — proven at Old Mutual
- Monitoring & Observability (Datadog, Grafana) — commoditised and excellent
- CI/CD Platform (GitHub Actions, Azure DevOps) — focus engineers on product, not tooling

**Build (Core Differentiators):**
- Payment processing logic — this IS the product
- Lending decision engine — competitive advantage
- KYC workflow orchestration — regulatory differentiation
- Partner integration adapters — custom to each bank

^
At Old Mutual, I integrated Auth0-based CIAM for enterprise-grade security rather than building identity management from scratch. At Equal Experts, I advised John Lewis on which legacy systems to sunset and which to modernise. The principle is the same: preserve your engineering capacity for what makes you unique in the market.

---

[.background-color: #F1B52F]
[.header: #103554]
[.text: #103554]

# Trade-off 3: Technical Debt vs. African Expansion

**The Tension:** The board has approved expansion into two new countries. But the platform at 25% cloud migration, with rising defects and instability, isn't ready for multi-country deployment.

**My Position:** Parallel tracks with a hard gate.

**Track 1: Platform Readiness**
- Cloud migration to 50%+ before any country launch
- Multi-tenant architecture with data residency support
- POPIA data localisation compliance (2026 enforcement deadline)
- Partner integration testing in staging environment

**Track 2: Market Preparation**
- Country 1 regulatory analysis (run in parallel — no engineering dependency)
- Local partnership development
- Product localisation requirements gathering

**The Hard Gate:** No country launch until platform reliability metrics hit thresholds:
- MTTR < 2 hours
- Deploy frequency: weekly
- Critical bugs/month: < 5

^
This is the trade-off that requires the most courage to articulate to the board. At Barclays ABSA, I crafted the architecture vision for digital banking across Africa — a continent-scale ambition. But we sequenced it based on platform readiness, not market opportunity alone. Launching into new markets on an unstable platform is how you lose both the new market AND the existing one.

---

[.background-color: #103554]
[.header: #FFFFFF]

# 12. Why Me
## 20+ Years of Proof Points

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Directly Relevant Experience

**DevOps Transformation at Scale**
ABSA — Halved project cycle times, built DevOps culture from scratch, established engineering practices that became the standard across the organisation.

**Pan-African Architecture**
Barclays ABSA — Designed future-state digital banking architecture for the African continent. Created Architecture Review Board. Multi-year capability roadmap.

**Cloud-Native Migration**
John Lewis & Equal Experts — Led legacy-to-modern platform migration. Monolith-to-microservices. Google Cloud migration. Saved £1M/month on a declining product.

**Fintech & Insurance Delivery**
Discovery/Manulife — Engineering and product delivery for North America's largest insurer. Capex/Opex models. Partner-market alignment. Incident management at scale.

**ML/Data Modernisation**
AXA Insurance — CI/CD pipelines cutting deployment lead times 30%. Shadow deployments. Probabilistic forecasting improving predictability 15%.

**Architecture Governance**
Sanlam, Eskom, Accenture — Business, enterprise, and application architecture. Regulatory alignment. Operating model design.

^
Every challenge in the ABC Technologies case study maps directly to something I've delivered. DevOps transformation — ABSA. African expansion architecture — Barclays. Cloud migration — John Lewis. Partner management — Discovery/Manulife. Compliance and governance — Sanlam, Accenture. This isn't theory for me. It's pattern recognition built over two decades.

---

[.background-color: #FFFFFF]
[.header: #103554]
[.text: #333333]

# Measurable Impact Across Engagements

| Organisation | Challenge | Outcome |
|-------------|-----------|---------|
| **ABSA** | Slow delivery, no DevOps | Halved cycle times, 5% customer engagement increase |
| **Barclays ABSA** | Pan-African digital banking | Future-state architecture, Architecture Review Board |
| **John Lewis** | £1M/month losses, legacy platform | Cloud migration, cost reduction, microservices transformation |
| **Discovery** | Complex multi-market delivery | Capex/Opex models, incident management, portfolio alignment |
| **AXA** | ML deployment to production | 30% faster deployments, 25% fewer errors, 15% better predictability |
| **Sanlam** | De-merger architecture complexity | Future-state application architecture, regulatory alignment |
| **Accenture** | Delivery value chain gaps | Target-state architecture, IT strategy, governance frameworks |
| **Old Mutual** | Banking platform integration | End-to-end AWS integration with Auth0 CIAM |

^
These aren't just job titles — they're measurable outcomes. I bring this evidence base to ABC Technologies not as a consultant recommending theory, but as a practitioner who has stabilised, scaled, and accelerated engineering organisations across Africa, Europe, and North America.

---

[.background-color: #103554]
[.header: #FFFFFF]
[.text: #FFFFFF]

# Summary: My Commitment to ABC Technologies

**In 90 days:** Stabilised delivery, quality gates in place, partner confidence restored, clear roadmap to EXCO.

**In 12 months:** Weekly deployments, MTTR under 2 hours, cloud migration at 80%, team scaled to 20+, first country expansion launched.

**In 24 months:** Elite engineering performance, full cloud-native platform, two new markets live, real-time payments product generating revenue.

**The approach:** Evidence-based, metrics-driven, people-first. Every recommendation backed by what I've delivered before.

---

[.background-color: #1E73BE]
[.header: #FFFFFF]
[.text: #FFFFFF]

# Thank You

**Benjamin Hinson**
bhinson@plerk.co.za | 082 565 4665

*"We cannot sacrifice quality for velocity or vice-versa. We can and must have both."*

I welcome your questions.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Appendix: ABSA Six Conditions for Transformation

1. **Conway's Law** — Org structure is a product of history. Silos beget supervision, supervision begets process. Restructure for flow.
2. **Validate, don't anticipate** — Learning is the only competitive advantage. Seek validation, not prediction.
3. **Stop shipping your org chart** — Product alignment over functional alignment. Cross-functional teams.
4. **Automate everything you can** — Adopt low-friction technology paths. Discuss the rest.
5. **Meet people where they are** — Let go of organisational delusion. Have empathy for the people doing the work.
6. **Create events, support with community** — Use the ELSA model: Event, Language, Structure, Agency.

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Appendix: DORA 2024 Research Highlights

- Elite performers deploy **182x** more frequently than low performers
- Lead time for changes: **127x** faster for elite teams
- Recovery time: **2,293x** faster for elite performers
- Change failure rate: **8x** lower for elite teams
- High performance cluster shrank from 31% → 22% (2023–2024)
- Low performance cluster grew from 17% → 25% (2023–2024)

**Key insight:** The gap between elite and low performers is widening. Organisations that invest in DevOps maturity pull further ahead each year.

*Source: 2024 DORA State of DevOps Report, Google Cloud*

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Appendix: South African Fintech Landscape 2025–2026

**Market Growth**
- SA fintech projected USD 3.7–14.9 billion by 2033
- Card transaction volume: ZAR 2.9 trillion (2025), growing 10.4% annually
- SA fintech raised USD 335.9 million in 2025 (up 234% from 2024)

**Regulatory Environment**
- POPIA data localisation enforcement deadline: 2026
- COFI Bill: awaiting Chief State Law Adviser certification
- SARB payments ecosystem modernisation — first overhaul in ~3 decades

**Pan-African Opportunity**
- PAPSS (Pan-African Payment & Settlement System) under AfCFTA
- SADC and EAC interoperability pilots underway
- 92% of fintech startups use public cloud; 92% adopted API-first design

---

[.background-color: #F9F9F9]
[.header: #103554]
[.text: #333333]

# Appendix: Team Topologies — Four Team Types

**Stream-Aligned Teams**
Own value delivery end-to-end. Aligned to a product or service domain. The primary team type.

**Platform Teams**
Provide internal services and abstractions that reduce cognitive load on stream-aligned teams.

**Enabling Teams**
Temporarily embed with other teams to upskill on specific capabilities, then move on.

**Complicated Subsystem Teams**
Handle specialist, complex components that require deep domain expertise.

**Scaling Path for ABC Technologies:**
10 → 15: Stream-aligned + light platform responsibilities
15 → 25: Formalise platform team, split stream-aligned by domain
25 → 40+: Full Team Topologies model with enabling teams for cloud-native upskilling
