# ICANotes+ Feature Brief / PRD Template

> The feature-level specification layer that sits above stories — outcome, not implementation.
> Authored by the PM, aligned with engineering lead and product-and-engineering leadership before the broader team picks up work.
> Deliberately stops short of fine-grained user stories: stories derived from it carry intent and acceptance criteria, not exhaustive specification.
> Target length: 1-3 pages.
> Source: AWS Principal PM (shared internally for ICANotes+)

---

## The One Test That Matters

> A story is "ready for development" when it sits beneath an aligned feature brief and carries enough customer and business context for engineering to make implementation calls independently. Readiness is a test of framing quality, not specification completeness. The "how" belongs to engineering.

---

## Brief Metadata

| Field | Value |
|-------|-------|
| Owner (PM) | |
| Engineering counterpart | |
| Target quarter / release | |
| Status | Draft / Aligned with leadership / In development / Shipped |
| Related briefs or dependencies | |

---

## 1. Customer Problem

_Who has this problem, how it shows up in their workflow, and the evidence: support themes, churn signals, discovery interviews, migration blockers. Two or three paragraphs maximum._

_The most common failure mode is describing the requested feature instead of the problem. If this section names a solution, rewrite it. A reader should finish this section able to argue for the work without ever having seen the proposed feature._

---

## 2. Intended Outcome (the "what")

_What the customer can do when this ships that they cannot do today. Describe the outcome, not the implementation._

_Wrong: "Add a recurrence table and a series-management endpoint."_
_Right: "A scheduler sets up a repeating appointment series once and trusts it appears correctly on provider calendars all year."_

_If engineering cannot make implementation choices from this section plus the constraints below, the outcome is not yet stated at the right altitude._

---

## 3. Success Measures

_How the team will know it worked. Each measure needs a baseline (where one exists) and a date when it will first be read._

| Measure | Baseline | Target | First Read Date |
|---------|----------|--------|-----------------|
|         |          |        |                 |
|         |          |        |                 |
|         |          |        |                 |

_The failure mode is naming measures nobody instruments. If a measure cannot be read from existing telemetry or a named new instrument, move it to Open Questions with an owner._

---

## 4. Scope Boundaries and Non-Goals

_What is explicitly out of scope, and what is deferred to a later phase. Name the nearest tempting adjacencies and rule them in or out._

**In scope:**
- 
- 

**Non-goals (explicit):**
- 
- 

**Deferred to later phase:**
- 
- 

_An empty non-goals list usually means scope will be negotiated inside refinement — which is exactly the time this template exists to recover._

---

## 5. Known Constraints

_Technical, regulatory/compliance, data, platform, and timeline constraints engineering should design within. State constraints, not solutions._

| Type | Constraint |
|------|-----------|
| Technical | |
| Regulatory / Compliance | |
| Data | |
| Platform (Classic-parity, shared-service dependencies) | |
| Timeline | |

_"Series expansion must not multiply calls to the settings service" is a constraint. "Cache the settings service" is engineering's call._

---

## 6. Open Questions

_Questions that must be answered before development commits. A question without an owner and a date is a risk, not a question._

| Question | Owner | Needed By |
|----------|-------|-----------|
|          |       |           |
|          |       |           |
|          |       |           |

---

## 7. FAQs

_Questions engineering, leadership, or customer-facing teams will ask, pre-answered. Seed at authoring time with questions the PM expects in refinement. Then let it evolve: whenever a question is asked more than once, in any forum, its answer moves here._

_Over time this section becomes the brief's institutional memory — a thin FAQ on a contested feature is a signal the framing is not yet complete._

**Q:**  
**A:**  

**Q:**  
**A:**  

---

## 8. Alignment Record

_The brief is aligned at the leadership level before the team is brought in. That order is what prevents specification time-tax from reproducing one altitude higher._

| Date | Reviewed With | Outcome |
|------|---------------|---------|
|      | Engineering lead(s) | |
|      | Product & engineering leadership | |

---

## 9. Stories Derived From This Brief

_Linked after decomposition. Each story carries intent and acceptance criteria; implementation detail (the "how", edge-case enumeration, technical design) is owned by engineering within the boundaries above._

_Where practical, write acceptance criteria in structured when/then form — "when [condition], the system shall [behavior]" — so AI Code Reviewer ticket-compliance checks and agent tooling can verify implementation against intent directly._

| Jira ID | Title |
|---------|-------|
|         |       |
|         |       |
|         |       |

---

## Definition of "Ready for Development" Under This Model

- [ ] The story sits beneath a feature brief that is aligned with leadership.
- [ ] It carries clear intent plus enough customer and business context for engineering to make implementation calls independently.
- [ ] Readiness is judged on framing quality, not specification completeness.

---

## References

- Source: AWS Principal PM (shared for ICANotes+ product team)
- Philosophy aligns with: [Marty Cagan's Empowered Product Teams (SVPG)](https://www.svpg.com/empowered-product-teams/)
- Acceptance criteria format: [EARS — Easy Approach to Requirements Syntax](https://alistairmavin.com/ears/)
- [prodmgmt.world: Complete PRD Template Guide](https://www.prodmgmt.world/blog/prd-template-guide)
