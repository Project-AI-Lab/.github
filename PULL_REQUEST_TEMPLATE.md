## Summary
What does this PR do?

<!-- 1-2 sentences. What problem does it solve or what does it add? -->

## Type of Change
- [ ] Feature
- [ ] bug Fix
- [ ] Refactor (no behavior change)
- [ ] Documentation
- [ ] Capability Improvement (RAG / Prompt / Eval / Agent)
- [ ] Breaking change


## Layer
- [ ] `pw-ai-core` — foundation, impacts everything. Review carefully.
- [ ] `pw-ai-capabilities` — reusable logic. Check for breaking changes + bump version.
- [ ] `pw-ai-apps` — application layer
- [ ] `client-*` — client project
- [ ] `internal-*` — ops / tooling

## Related Issue / Context
<!-- Link issue or describe context -->

## What Changed
<!-- Steps to validate this change: -->
1.
2.

---

## 🤖 AI-Specific Considerations (if applicable)
*Skip sections that don't apply.*

### Prompt Changes
- [ ] Prompt updated
- [ ] Versioned / tracked in `pw-ai-capabilities/prompts`
- [ ] No hardcoded prompts introduced

### Retrieval (RAG)
- [ ] chunking / embedding logic changed
- [ ] Data source updated
- [ ] Retrieval logic changed

### Evaluation
- [ ] Test cases added/updated
- [ ] Output quality verified
- [ ] Eval rubric updated if sucess criteria changed

### model / Provider
- [ ] uses model sbstraction from `pw-ai-core` (no direct API calls in capabilities or apps)
- [ ] no provider-specific logic outside `pw-ai-core`

---

## ⚠️ Risks / Edge Cases
- 

## Checklist
- [ ] Follows layer rules - core / capabilities / apps separation is clean
- [ ] No secrets, API keys, or client data included
- [ ] Tests / evals added or updated
- [ ] Documentation updated if behavior changed
- [ ] Code reviewed
- [ ] if `pw-ai-core` or `pw-ai-capabilities` - version bumped and downstream impact checked.