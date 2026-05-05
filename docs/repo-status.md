# Repository status vocabulary

Statuses describe **lifecycle and how the team should treat the repo**, not code quality. A repo can be `archived` but still run in production until migrated; the status records intent and maintenance expectation.

| Status | Meaning |
|--------|---------|
| **active** | Under active development or operational maintenance; PRs and issues expected; default for shipping components. |
| **reference** | Kept for historical accuracy, specs, or reproducibility (e.g. hackathon snapshot); not the place for new feature work unless explicitly revived. |
| **archived** | Read-only or frozen; no planned feature work; may still be cloned or deployed for legacy paths until sunset. |
| **experimental** | Exploratory or spike; APIs and scope may change abruptly; not a stability contract for dependents. |
| **planned** | Repository intended but not yet created, or scaffold exists without committed owners; update when it becomes real. |
| **deprecated** | Successor exists or the approach is abandoned; avoid new integrations; document migration in notes or `related_links`. |

**Machine-readable index:** [data/repos.json](../data/repos.json) uses a constrained set (`active`, `archived`, `reference`, `planned`, `unknown`). Map **experimental** and **deprecated** in prose here; when promoting to JSON, use `active`/`archived`/`reference`/`planned`/`unknown` and encode nuance in `notes` until the schema is extended.
