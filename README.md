# Hi, I'm Aaron George

I build AI agents that run inside real operations, where a wrong message reaches a customer and a leaked number is a real problem. My focus is the part that is easy to skip: making an agent's safety rules **enforceable in code** and its claims **verifiable**.

## Start here

| Repo | What it shows |
|------|---------------|
| [**agent-ops-contract**](https://github.com/aarongeorge97/agent-ops-contract) | Four tested primitives (policy lint, per-message send gate, preview-only deploy guard, evidence-required handoffs) plus a drop-in `CLAUDE.md` contract and agent templates. Python, stdlib only, 26 tests. |
| [**cc**](https://github.com/aarongeorge97/cc) | A Claude Code-native 20-agent pipeline with manager agents that fail low-quality work and send it back. Includes a side-by-side against a single-prompt baseline. |

## What I care about

- **Rules that live where the action happens**, not in a prompt or a folder name.
- **Approval per action**, never a standing license.
- **Honest gaps over plausible placeholders.**
- **Done means evidenced:** every handoff carries a number.
