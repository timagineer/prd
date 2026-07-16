# PRD Templates — Summary & Guide

A curated collection of product requirements document templates, from lean one-pagers to AI-agent specs. Each is a copyable Markdown file with usage instructions and source references.

---

## Templates at a Glance

| # | Template | Origin | Best For | Length |
|---|----------|--------|----------|--------|
| 01 | [Lenny Rachitsky 1-Pager](01-lenny-rachitsky-1-pager.md) | Lenny's Newsletter / Notion | Most projects, quick alignment, startups | 1 page |
| 02 | [Basecamp Shape Up Pitch](02-basecamp-shape-up-pitch.md) | Basecamp (Ryan Singer) | Builder-autonomy culture, fixed time budgets | 1-2 pages |
| 03 | [Intercom Intermission](03-intercom-intermission.md) | Intercom (Paul Adams) | JTBD teams, B2B SaaS, design partnerships | Strict 1 page (A4) |
| 04 | [Kevin Yien Staged PRD](04-kevin-yien-staged-prd.md) | Square / Mutiny | Growth-stage, cross-functional sign-off gates | 3-5 pages |
| 05 | [Amazon Working Backwards](05-amazon-working-backwards.md) | Amazon (Colin Bryar) | Major new products, strategic bets | 3-6 pages |
| 06 | [Planio Lean PRD](06-planio-lean-prd.md) | Planio / Marty Cagan | Agile teams wanting lightweight structure | 1-2 pages |
| 07 | [Figma Coda PRD](07-figma-coda-prd.md) | Figma (Yuhki Yamashita) | Design-forward orgs, living project hubs | 3-5 pages (interactive) |
| 08 | [AI-Agent Phased PRD](08-ai-agent-phased-prd.md) | GitHub Spec Kit / Haberlah | Spec-driven AI coding (Cursor, Claude, Copilot) | Varies by phases |
| 09 | [AGENTS.md](09-agents-md.md) | Linux Foundation / agentsmd | Repo-level standing rules for any AI agent | 1-2 pages |
| 10 | [ICANotes+ Feature Brief](10-icanotes-feature-brief.md) | AWS Principal PM | Outcome-over-implementation, story decomposition | 1-3 pages |

---

## Patterns Across High-Performing Teams

### 1. Problem Before Solution — Always

Every template in this collection separates problem understanding from solution design. The ones that enforce it hardest (Intercom: "Do not add the solution here"; ICANotes+: "If this section names a solution, rewrite it") produce the clearest specs.

The most common PRD failure mode is describing the requested feature instead of the problem it solves.

### 2. Explicit Non-Goals Are Non-Negotiable

Templates 02, 03, 04, 05, 06, 08, and 10 all include a dedicated non-goals or "no-gos" section. The reasoning is consistent: if you don't explicitly exclude tempting adjacencies, they'll be negotiated during refinement or silently built by an eager engineer (or AI agent).

An empty non-goals list is a red flag, not a sign of focus.

### 3. Constraints Over Dates

The best templates frame timelines as constraints, not deadlines:
- Shape Up's "appetite" (a time budget that shapes the solution)
- Planio's constraint-based timeline (work backward from real limits)
- ICANotes+'s known constraints (state the constraint, not the solution)

This aligns teams on tradeoffs rather than creating false precision.

### 4. The "How" Belongs to Engineering

A clean separation of altitude appears in:
- ICANotes+ Feature Brief: "The 'how' belongs to engineering"
- Shape Up: Solution stays at fat-marker level, builders fill in details
- Kevin Yien: "Draw the perimeter so the team can focus on how to fill it in"

Over-specification removes team ownership and slows delivery.

### 5. Living Documents, Not Static Artifacts

Modern PRDs are project hubs that evolve:
- Figma embeds live designs that auto-update
- Kevin Yien includes a change log
- ICANotes+ FAQ section grows as questions accumulate ("a thin FAQ on a contested feature is a signal the framing is not yet complete")

A PRD that nobody revisits after writing is a PRD that didn't need to exist.

### 6. Acceptance Criteria Must Be Verifiable

The AI-agent era made this non-optional. Traditional criteria like "should be fast" or "easy to use" are useless for both humans and machines. The pattern:
- ICANotes+: "when [condition], the system shall [behavior]"
- AI Phased PRD: checkbox acceptance criteria per phase
- GitHub Spec Kit: FR-numbered requirements with Given-When-Then format

If you can't test it, it's not a requirement — it's a wish.

### 7. Alignment Happens Before Building

Every mature template includes explicit alignment gates:
- Kevin Yien: Stakeholder sign-off between Problem and Solution phases
- ICANotes+: Leadership alignment before the team is brought in
- Amazon: PR/FAQ goes through rounds of rejection (cheap validation)

Building something nobody agreed to is the most expensive mistake a team can make.

---

## Trends Shaping PRDs in 2025-2026

### The AI-Agent Shift

PRDs now serve dual audiences: humans (for alignment and decisions) and AI agents (for implementation). This means:
- Sequential, dependency-ordered phases replace monolithic documents
- "DO NOT CHANGE" protection patterns prevent AI from refactoring stable code
- Machine-verifiable acceptance criteria replace human-interpretable guidelines
- ~150-200 instructions per phase is the practical ceiling for frontier LLMs

### Spec as Source of Truth

GitHub's engineering team declared: "We're moving from 'code is the source of truth' to 'intent is the source of truth.'" The specification now determines what gets built. Tools like GitHub Spec Kit, Kiro Specs, and Task Master formalize this into Specify → Plan → Tasks → Implement workflows.

### Research Before Specification

Platform capabilities change faster than LLM training data. Best practice now mandates a research phase before writing specs — verifying framework versions, API compatibility, and platform constraints before committing requirements to paper. Claude Code, JetBrains Junie, and Replit all enforce this explicitly.

### The PM as Specification Architect

Andrew Ng observed that managers are proposing twice as many PMs as engineers for the first time. The PM role is shifting from "alignment document author" to "specification architect" — structuring intent precisely enough that AI agents implement it reliably, while preserving the strategic judgment and user empathy that define the role.

---

## How to Choose

**Start here:** Lenny's 1-Pager (01) works for most features. It's the universal starting point.

**Then graduate based on context:**
- Need builder autonomy + time constraints → Shape Up (02)
- Need JTBD clarity, no solution yet → Intercom (03)
- Need cross-functional sign-off gates → Kevin Yien (04)
- Major new product bet → Amazon PR/FAQ (05)
- Need a living project hub → Figma Coda (07)
- Building with AI agents → Phased PRD (08) + AGENTS.md (09)
- Feature → story decomposition flow → ICANotes+ Brief (10)

**Layer them:** AGENTS.md (09) provides repo-level standing rules. A feature-level template (01-08, 10) provides per-project specs. They complement, not compete.

---

## Sources

- [prodmgmt.world: The Complete PRD Template Guide](https://www.prodmgmt.world/blog/prd-template-guide)
- [Planio: How to Write a Lean PRD](https://plan.io/blog/one-pager-prd-product-requirements-document/)
- [Basecamp: Shape Up (Free Book)](https://basecamp.com/shapeup)
- [Atlassian: Lenny's Product Requirements Template](https://www.atlassian.com/software/confluence/templates/lennys-product-requirements)
- [Haberlah: How to Write PRDs for AI Coding Agents (2026)](https://medium.com/@haberlah/how-to-write-prds-for-ai-coding-agents-d60d72efb797)
- [SSOJet: 9 PRD and Spec Templates for AI Agents (2026)](https://ssojet.com/blog/prd-spec-templates-ai-agents)
- [GitHub: Spec-Driven Development with AI](https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/)
- [AGENTS.md Official Repository](https://github.com/agentsmd/agents.md)
