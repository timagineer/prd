# AI-Agent Phased PRD

> Optimized for AI coding agents. Sequential, dependency-ordered, testable phases.
> Traditional PRDs optimize for human comprehension. This format optimizes for machine execution while remaining human-reviewable.
> Best for: Spec-driven development with AI agents (Claude Code, Cursor, Copilot, Codex, Kiro).

---

## Project Context

### Project Name

<!-- Clear, descriptive -->

### Description

<!-- 2-3 sentences establishing what this is -->

### Core Features

1. 
2. 
3. 

### Technical Stack

- Frontend: 
- Backend: 
- Database: 
- Storage: 
- Auth: 

### Architecture Patterns

- State management: 
- API structure: 
- Component organization: 

---

## Phase 0: Planning (Confirm Understanding)

> Present this phase first. Ask the agent to confirm understanding BEFORE any code is written.

**Objective:** Establish shared understanding of the full project scope.

**Agent instruction:** _"Please confirm you understand this architecture. Do not build yet."_

---

## Phase 1: [Foundation]

**Objective:** _One sentence describing what this phase accomplishes._

**Requirements:**
1. 
2. 
3. 

**Technical Details:**
- Database: 
- API: 
- Components: 

**DO NOT CHANGE:**
- (nothing yet — this is phase 1)

**Acceptance Criteria:**
- [ ] 
- [ ] 
- [ ] All functionality is verifiable / testable

**Checkpoint:** "[Phase 1 name]"

---

## Phase 2: [Core Feature A]

**Objective:** _One sentence._

**Requirements:**
1. 
2. 
3. 

**Technical Details:**
- Database: 
- API: 
- Components: 

**DO NOT CHANGE:**
- Database schema from Phase 1
- 

**Acceptance Criteria:**
- [ ] 
- [ ] 
- [ ] All Phase 1 functionality still works

**Checkpoint:** "[Phase 2 name]"

---

## Phase 3: [Core Feature B]

**Objective:** _One sentence._

**Requirements:**
1. 
2. 
3. 

**Technical Details:**
- Database: 
- API: 
- Components: 

**DO NOT CHANGE:**
- Database schema
- API endpoint signatures from Phases 1-2
- 

**Acceptance Criteria:**
- [ ] 
- [ ] 
- [ ] All previous functionality still works

**Checkpoint:** "[Phase 3 name]"

---

## Phase N: [UI Polish & Error Handling]

**Objective:** _One sentence._

**Requirements:**
1. 
2. 
3. 

**DO NOT CHANGE:**
- Database schema
- API endpoint signatures
- Authentication flow
- Core business logic from all previous phases

**Acceptance Criteria:**
- [ ] 
- [ ] 
- [ ] All previous functionality still works
- [ ] No regressions

**Checkpoint:** "[Final phase name]"

---

## Non-Goals (Global)

_State these positively. AI agents cannot infer from omission._

- DO NOT implement: 
- DO NOT implement: 
- DO NOT implement: 

---

## Adaptation Patterns

_When changes are needed mid-project:_

| Change Type | Action |
|-------------|--------|
| Layout/data model change | Restructure NOW — affects all downstream phases |
| Isolated new feature | Add as additional phase at the end |
| Visual polish | Scoped phase with DO NOT CHANGE section covering all logic |

---

## Key Principles

1. **Research before specifying** — Verify platform capabilities, framework versions, API compatibility before writing requirements.
2. **Sequential phases** — Each phase builds on the last. No forward references.
3. **Testable checkpoints** — Every phase ends with working, verifiable functionality.
4. **No dead ends** — Every phase leaves the codebase in a runnable state.
5. **Explicit protection** — DO NOT CHANGE sections grow with each phase.
6. **~150-200 instructions max** — Frontier LLMs degrade beyond this. Keep phases bounded.
7. **5-15 minutes of agent work per phase** — Larger phases are too hard to debug. Smaller phases create overhead.

---

## References

- [Haberlah: How to Write PRDs for AI Coding Agents (2026)](https://medium.com/@haberlah/how-to-write-prds-for-ai-coding-agents-d60d72efb797)
- [GitHub Spec Kit](https://github.com/github/spec-kit)
- [GitHub: Spec-Driven Development with AI](https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/)
- [SSOJet: 9 PRD and Spec Templates for AI Agents](https://ssojet.com/blog/prd-spec-templates-ai-agents)
- [Claude Code: Explore-Plan-Code-Commit Workflow](https://docs.anthropic.com/en/docs/claude-code)
- [Replit: Introducing Plan Mode](https://blog.replit.com/introducing-plan-mode-a-safer-way-to-vibe-code)
