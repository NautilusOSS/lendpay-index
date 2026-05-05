# lendpay-index

Canonical index for **LendPay** across multiple Git repositories after [ETHGlobal Open Agents 2026](https://ethglobal.com/).

## What this is

LendPay started during **ETHGlobal Open Agents 2026**. The hackathon produced several focused repositories (apps, demos, integrations) rather than a single monolith.

This repository is the **source of truth for navigation**: where each repo lives, what it does, who owns it, how mature it is, and how the set evolves over time. It aggregates links, status, and architectural context so contributors do not have to infer structure from scattered READMEs alone.

## What this is not

This is **not** the LendPay application monorepo. It does not ship product code, run services, or replace any individual repo’s documentation. Use the linked repositories for implementation and runtime detail.

## Contents

| Path | Role |
|------|------|
| [repos.md](repos.md) | Human-readable repo table |
| [data/repos.json](data/repos.json) | Machine-readable repo metadata |
| [timeline.md](timeline.md) | Pointer to canonical project timeline |
| [docs/repo-status.md](docs/repo-status.md) | Status vocabulary |
| [docs/architecture-map.md](docs/architecture-map.md) | Repos mapped to product layers |
| [docs/maintenance-notes.md](docs/maintenance-notes.md) | How to keep the index current |

## Primary upstream context

- Hackathon coordination / umbrella context: [temptemp3/ETHGlobal2026OpenAgent](https://github.com/temptemp3/ETHGlobal2026OpenAgent)
- Canonical timeline: [NautilusOSS/lendpay-timeline](https://github.com/NautilusOSS/lendpay-timeline)
