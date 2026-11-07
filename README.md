# Hi, I'm Aaron George

I build AI agents that run inside real operations, where a wrong message reaches a customer and a leaked number is a real problem. My focus is the part that is easy to skip: making an agent's safety rules **enforceable in code** and its claims **verifiable**.

## Start here

| Repo | What it shows |
|------|---------------|
| [**agent-ops-contract**](https://github.com/aarongeorge97/agent-ops-contract) | Four tested primitives (policy lint, per-message send gate, preview-only deploy guard, evidence-required handoffs) plus a drop-in `CLAUDE.md` contract and agent templates. Python, stdlib only, 26 tests. |
| [**fleet-ops-platform**](https://github.com/aarongeorge97/fleet-ops-platform) | A multi-tenant delivery platform: Postgres schema with PostGIS, pgvector and row-level security (12 migrations), an Express API and WebSocket events. Migrated and booted end to end on Postgres 17; four bugs found and fixed while preparing it (see its README). Synthetic data. |
| [**shop-booking-engine**](https://github.com/aarongeorge97/shop-booking-engine) | A dependency-free booking engine for a single shop: timezone-correct availability, no double-booking, idempotent no-show fees, a walk-in queue, consent-aware messaging. 31 tests, plus a check that injected bugs get caught. |
| [**route-globe**](https://github.com/aarongeorge97/route-globe) ([live](https://aarongeorge97.github.io/route-globe/)) | An interactive 3D globe of a delivery network on a plain canvas: no libraries, no map tokens, no network. Tested projection and routing geometry. |
| [**cc**](https://github.com/aarongeorge97/cc) | A Claude Code-native 20-agent pipeline with manager agents that fail low-quality work and send it back. Includes a side-by-side against a single-prompt baseline. |
| [**agent-mission-control**](https://github.com/aarongeorge97/agent-mission-control) | A Next.js 14 + TypeScript dashboard for watching a fleet of AI agents: status, token cost, activity feed, pipeline, tasks. Builds clean (14 routes); synthetic data. |
| [**claude-skill-principal-audit**](https://github.com/aarongeorge97/claude-skill-principal-audit) | A Claude Code skill for four-phase audits where every finding needs a `file:line` citation, with an A–F grade and M0–M3 roadmap. |

## Private work (details withheld)

This runs in production at a food-logistics company. The code and data are confidential, so there are no repos. What I can say:

- **Operations platform driven by Claude Code agents.** One registry, one template and one builder generate per-counterparty internal modules from live routing data. A human-owned contract (`CLAUDE.md`) sets what agents may and may not do, and every job ends in a structured handoff.
- **Guarded publishing.** Internal pages are linted for personal data, secrets and financial figures, then deployed only to access-controlled previews. A smoke-test suite gates every demo.
- **Steward agents.** Specialist Claude Code subagents refresh data, check the one metric each counterparty cares about, and draft (never send) updates.
- **Local admin control room** with authenticated endpoints, and a 3D-globe operating picture of the delivery network.
- **Marketing site and SEO work** shipped to production.

`agent-ops-contract` above is the reusable core of the safety model, rewritten from scratch with no company data.

## What I care about

- **Rules that live where the action happens**, not in a prompt or a folder name.
- **Approval per action**, never a standing license.
- **Honest gaps over plausible placeholders.**
- **Done means evidenced:** every handoff carries a number.
