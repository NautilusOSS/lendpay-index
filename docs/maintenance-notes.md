# Maintaining lendpay-index

Internal rules so the index stays trustworthy.

## Additions

- **Register every new LendPay-related repository** here as soon as it exists or is planned: update [repos.md](../repos.md) and [data/repos.json](../data/repos.json) together so humans and automation stay aligned.
- Prefer one row per GitHub (or equivalent) repo; split monorepos into one logical entry with notes if you do not split remotes.

## Lifecycle

- **Update `status` and `phase`** when a repo’s role changes (e.g. demo → production fork, or active → maintenance-only).
- **Do not delete rows or JSON objects** for repos that are retired. Mark them `archived` or `deprecated`, add a short note and optional successor URL in `notes` or `related_links`.
- **Preserve hackathon repos** as `reference` or `archived` as appropriate so history and reproducibility remain discoverable.

## Links

- **Link outward:** demos, blog posts, significant PRs, and releases via `related_links` in JSON and/or the Notes column in `repos.md`.
- **Timeline:** substantive dated narrative belongs in [lendpay-timeline](https://github.com/NautilusOSS/lendpay-timeline); this repo points there and records repo-level metadata.

## Hygiene

- Keep tone factual and concise; avoid marketing copy.
- When unsure, use `unknown` / `TBD` and a note rather than guessing URLs or owners.
