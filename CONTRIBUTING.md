# Contributing Guidelines

This repository is part of the AI Lab platform. Our goal is to build **reusable AI capabilities**, not one-off solutions.

---

## C🧠 Core Principle

**1. Capability > Project**
    - Build reusable components (RAG, prompts, eval). If something will be used by 2+ projects, it belongs in `pw-ai-capabilities` - not buried inside an ap or client repo. Hence, avoid duplicating logic inside apps.

**2. Evaluation First**
    - Every AI output must be testable. Before you ship, define what "good" looks like. 

**3. Structured Prompts**
    - No harcoded prompts. Ever. Use templates and versioning in `pw-ai-capabilities/prompts`

**4. Separation of Layers**
    - `core` -> base utilities (depends on nothing)
    - `capabilities` -> reusable AI Logic (can use `core`)
    - `apps` -> use-case implementations (can use `capabilities`)

Before writing code, ask: which layer does this belong in?

| Layer | Repo | Contains |
|---|---|---|
| Foundation | `pw-ai-core` | base utilities, model abstraction, config, logging |
| Capabilities | `pw-ai-capabilities` | Reusable AI logic - RAG, prompts, evals, agents |
| Applications | `pw-ai-apps` | use-case implementations, internal products |
| Client work | `client-*` | Client-specific, isolated, private |

---

## 🛠 Development Workflow

1. **Create issue** - describe the problem, not the solution
2. **Discuss approach (if needed)** if it touches `pw-ai-core` or `pw-ai-capabilities` (these affect everyone)
3. **Implement** on branch: `feat/`, `fix/`, `chore`, `docs/`
4. **Add evaluation / tests** - no untested AI logic ships
5. **Submit PR** using the PR template - fill it out honestly

---

## ⚠️ What to Avoid
- Duplicating prompts across apps or client repos
- Skipping evaluation - define "good" before you build
- Hardcoding prompts, data sources, or model ames
- uilding tightly coupled solutins that can't be extracted later
- Letting client-specific logic bleed into `pw-ai-core` or `pw-ai-capabilities`
- Committing secrets, API keys, or client data - ever

## 📦 Where to Put Code

- Shared logic -> `pw-ai-capabilities`
- Base infra -> `pw-ai-core`
- Use-case specific -> `pw-ai-apps`

---

## 🔐 Secrets & Security
- Use `.env` locally - always in `.gitignore`
- Use Github org secrets for CI/CD
- If you accidently commit a secret: **rotate it immediately**, then clean the history 

---

## 📐 Code Style
- Python: `ruff` for linting, `black` for formatting
- Docstrings on all public functions and classes
- Keep functions small and single-purpose

---
## Versioning (`pw-ai-core` and `pw-ai-capabilities` only)

Semantic versioning: `vMAJOR.MINOR.PATCH`

| Change | Bump |
|---|---|
|Breaking API change | MAJOR |
| New feature, backward compatible | Minor |
| Bug fix | PATCH |

Tag release in GitHub. Update `CHANGELOG.md` with every release.

---

## 🚀 Goal

Every contribution should move us closer to:
> A reusable AI capability platform that scales across use-cases where one improvement benefits everything built on top of it.