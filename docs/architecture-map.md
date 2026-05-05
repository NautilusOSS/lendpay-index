# Architecture map: repos to product layers

This maps **known named repos** to logical layers. One repo can span multiple layers; layers can be empty until a repo is linked.

| Layer | Role | Repos (current index) |
|-------|------|------------------------|
| **Web app** | Browser UI, client state, public or authenticated UX | `lendpay-app` (URL TBD) |
| **Backend / API** | HTTP/RPC services, persistence, auth, business rules | `lendpay-backend` (URL TBD) |
| **KeeperHub workflow** | Automation, keepers, scheduled or event-driven jobs consuming LendPay APIs or chain state | TBD — link repo when named |
| **Gateway webhook** | Inbound webhooks, signing, routing to core services | `lendpay-gateway-algorand-dorkfi` (URL TBD) |
| **Protocol integration** | Chain- or protocol-specific adapters (e.g. Algorand, DorkFi) | `lendpay-gateway-algorand-dorkfi` (may overlap with gateway) |
| **Timeline / documentation** | Dated history, decisions, releases | `lendpay-timeline` |
| **Hackathon coordination** | Umbrella repo, judging artifacts, multi-repo pointers | `ETHGlobal2026OpenAgent` (status **reference**; hackathon concluded, inactive) |

**Demos and spikes:** `openagent-demo1` is classified as an **archived** pre–UI-integration spike (status in [repos.md](../repos.md)); it may be revived for future experimentation. Historically it sat under hackathon coordination or **web app** depending on implementation—treat as dormant unless reopened.

**Reference:** [repos.md](../repos.md), [data/repos.json](../data/repos.json).
