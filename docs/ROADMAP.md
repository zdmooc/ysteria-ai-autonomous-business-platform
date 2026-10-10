# Delivery roadmap — first commercial activity

Status convention: PLANNED / IN PROGRESS / EVIDENCED / BLOCKED. Mark EVIDENCED only with verifiable commits, tests and operational proof.

| Gate | Objective | Acceptance criteria | Initial state |
|---|---|---|---|
| M0 | Business/architecture/budget baseline | Documented scope, risk register, financial caps, decision rights | EVIDENCED: documentation only |
| M1 | Reproducible engineering platform | Local compose, basic site/API/DB, tests and CI green | PLANNED |
| M2 | Agent governance | Workflows, policies, explicit approvals, execution journal, mock budgets | PLANNED |
| M3 | Content factory | Source-aware research, original article/video pipeline, localization, QA and safe scheduled drafts | PLANNED |
| M4 | Commerce | Catalogue, subscriptions/digital delivery, checkout tests, invoicing/tax/privacy review | PLANNED |
| M5 | Channel integrations | Authorized account OAuth/APIs, retry/deduping, audit, KDP workflow where supported | PLANNED |
| M6 | Controlled go-live | Secured live infrastructure, restore drill, measured sale, analytics, support and cost alerting | PLANNED |

## MVP experiments
- Initial verticals: symbolic readings and researched cultural mysteries, clearly separated from factual reporting.
- Initial offer hypotheses: EUR 9.99/month membership, EUR 6.99 downloadable guide, EUR 4.99 symbolic report; test value and pricing before claiming product-market fit.
- Languages: French and English first; add further languages based on measured opportunity.
- Distribution: editorial website and a small number of officially integrated channels, not all networks at once.

## Dependencies and boundaries
Reference patterns from separate GitOps/cloud/platform repositories when useful; no hard dependency on D099, OpenShift CRC or a personal workstation running 24/7.

## Next implementation slice
M1: scaffold frontend/backend, docker compose, database migration, GitHub Actions tests and a cost-safe local development guide.
