# Project AI Systems

We build *reusable AI capabilities** and deliver intelligent systems for clients.

> Build capabilities, not one-off tools.

---

## 🎯 What We Focus On

- Model Abstraction
- LLM Cost tracking and usage
- Retrieval (RAG)
- Prompt orchestration 
- Evaluation frameworks
- Agent workflows

---

## 🧱 Architecture 
Every system we build follows the same three-layer structure:

| Layer | Repo | Putpose |
|---|---|---|
| Foundation | `pw-ai-core` | Model abstraction, config, logging, utilities |
| Capabilities | `pw-ai-capabilities` | RAG, prompt, evals, agents |
| Applications | `pw-ai-apps` | Internal products build on capabilities |

Client projects are delivered in isolated `client-*` repos - consuming capabilities, never reinventing them.

---

## 🧠 Our Philosophy
One improvement to `pw-ai-capabilities` benefits every app and every client simultaneously.

That's the compounding effect we're building toward.

---

## Standards

- **Language:** Python (primary)
- **Models:** Claude (primary), with provider abstraction via `pw-ai-core`
- **Branching:** `main` is always deployable. All work via PRs.
- **Versioning:** Semantic version (`v1.2.3`) for `pw-ai-core` and `pw-ai-capabilities` releases.

## 📁 Repo naming Conventions

| Prefix | Example | Used for |
|---|---|---|
| `pw-ai-core` | `pw-ai-core` | Foundation layer |
| `pw-ai-capabilities` | `pw-ai-capabilities` | Reusable capability layer |
| `pw-ai-apps` | `pwai-apps` | Internal products |
| `client-` | `gpj-acme-chatbot` | Clent-specific projects |
| `internal-` | `internal-playbooks` | Ops, templates, research |

---

## 🤝 Contributing
See [`CONTRIBUTIN.md`](../CONTRIBUTING.md) for guidelines.