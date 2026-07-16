# AGENTS.md Template

> The lightest, most portable option. A single Markdown file that tells any AI coding agent how to work in your repo.
> Think of it as a "README for agents."
> Used by 60,000+ open-source projects. Stewarded by the Linux Foundation's Agentic AI Foundation.
> Supported by: Codex, Cursor, Copilot, Jules, Amp, Gemini CLI, Claude Code, and others.
> Best for: Any team wanting one tool-agnostic instructions file every agent reads.

---

```markdown
# AGENTS.md

## Project Overview

<!-- Brief description of what this project is and does -->

## Tech Stack

- Language: 
- Framework: 
- Database: 
- Package Manager: 
- Build Tool: 

## Commands

### Build
```
[your build command]
```

### Test
```
[your test command]
```

### Lint
```
[your lint command]
```

### Run (Development)
```
[your dev server command]
```

## Project Structure

```
src/
├── components/    # UI components
├── lib/           # Shared utilities
├── routes/        # Page routes
├── services/      # API/data layer
└── types/         # Type definitions
```

## Code Style

- [Style convention 1, e.g., "Use functional components with hooks"]
- [Style convention 2, e.g., "Prefer named exports over default exports"]
- [Style convention 3, e.g., "Use early returns to reduce nesting"]

### Naming Conventions

- Files: [e.g., kebab-case for files, PascalCase for components]
- Variables: [e.g., camelCase]
- Constants: [e.g., UPPER_SNAKE_CASE]
- Types/Interfaces: [e.g., PascalCase, prefix interfaces with I or not]

### Examples

```[language]
// Good
[example of preferred pattern]

// Avoid
[example of pattern to avoid]
```

## Testing Expectations

- [e.g., "All new features require unit tests"]
- [e.g., "Use describe/it blocks, not test()"]
- [e.g., "Mock external services, never hit real APIs in tests"]
- [e.g., "Minimum 80% coverage for new code"]

## Git Workflow

- Branch naming: [e.g., "feature/description", "fix/description"]
- Commit messages: [e.g., "Conventional Commits format"]
- PR requirements: [e.g., "All tests pass, at least 1 approval"]

## Boundaries

### DO NOT

- [e.g., "Do not modify the auth system without explicit instruction"]
- [e.g., "Do not add new dependencies without asking"]
- [e.g., "Do not change the database schema directly"]
- [e.g., "Do not remove existing tests"]

### ALWAYS

- [e.g., "Always run tests before committing"]
- [e.g., "Always handle errors explicitly, never swallow them"]
- [e.g., "Always use environment variables for secrets"]

## Common Pitfalls

- [e.g., "The ORM requires explicit .save() — changes don't auto-persist"]
- [e.g., "Auth middleware must come before route handlers"]
- [e.g., "CSS modules use camelCase, not kebab-case"]
```

---

## How To Use This Template

1. **Place at repo root** — `AGENTS.md` in the root directory. Agents look for it automatically.
2. **Keep it concise** — This is standing rules, not a feature spec. Pair with per-feature PRDs for specific work.
3. **No required fields** — Include only what's relevant to your project. Skip sections that don't apply.
4. **Update as patterns emerge** — When an agent repeatedly makes the same mistake, add a boundary or pitfall.
5. **Layer beneath PRDs** — AGENTS.md carries repo-level rules so your feature specs can focus on the feature.

---

## References

- [AGENTS.md Official Repository](https://github.com/agentsmd/agents.md)
- [GitHub: How to Write a Great agents.md](https://github.blog/ai-and-ml/github-copilot/how-to-write-a-great-agents-md-lessons-from-over-2500-repositories/)
- [SSOJet: 9 PRD and Spec Templates for AI Agents](https://ssojet.com/blog/prd-spec-templates-ai-agents)
- [Linux Foundation: Agentic AI Foundation](https://www.linuxfoundation.org/)
