# Mysteria AI — Autonomous Digital Business Platform

> Repository name: `ysteria-ai-autonomous-business-platform` (historical slug). Product and working brand: **Mysteria AI**.

## Vision
Build a multilingual, AI-native digital company that identifies viable opportunities in esotericism, mysteries, unexplained phenomena and cultural storytelling, creates original products and media, operates approved distribution channels, sells digital goods and subscriptions, and optimizes based on **net margin**, subject to human-defined authority boundaries.

The platform is a **business operating system**, not only a mobile application. Websites, mobile apps, marketplaces, newsletters and social media channels are independently selectable go-to-market channels.

## Principles
- **Human-controlled capital:** no spending, account opening, irreversible publication, contracts or platform policy bypass outside explicit authorization.
- **Truthfulness:** label entertainment, symbolic readings, fiction, hypotheses and documented facts. Never invent evidence or testimonials or exploit fear.
- **Multi-agent with audit trails:** decision proposals, evidence, approval, execution, measurement, rollback.
- **FinOps first:** provider quotas, hard budgets, unit economics, observability and emergency kill switch.
- **Platform portability:** container-first; Terraform; defer Kubernetes and owned GPUs until economically warranted.
- **Compliance:** GDPR, consumer protection, payments, AI/media disclosures, intellectual property and each channel's API/marketplace terms.

## MVP
1. Multilingual responsive website (initially French and English; expand from verified demand).
2. AI research, editorial planning and original articles/video production with review gates.
3. Content scheduling to approved channels via supported APIs.
4. Digital product catalogue, payment checkout and customer support workflow.
5. AI CEO *proposes* opportunities, launches controlled experiments, and measures conversion/margins.
6. Amazon/KDP as a **separate approval-dependent integration**, not a presumed autonomous publishing API.

## High-level modules
- `apps/web`: public website, editorial content and commerce.
- `apps/admin`: operations cockpit, budgets, approvals and audit.
- `services/api`: API, identity integration, tenancy, catalogues and orders.
- `agents/`: research, editor, production, marketing, commerce, finance, compliance, AI CEO.
- `integrations/`: social publishing, payment providers and marketplaces.
- `infra/`: IaC, deployment, secrets strategy, logging and backup.
- `docs/`: strategy, roadmap, economics, architecture and governance.

## Delivery gates
- **M0** Cadrage and documented baseline.
- **M1** Reproducible local stack and CI.
- **M2** Agent orchestration and budget/approval/audit controls.
- **M3** Content production, quality and scheduled publication.
- **M4** Web storefront and payment test-to-live flow.
- **M5** Marketplace integrations subject to provider permissions.
- **M6** Operational launch and first measured unit economics.

## Current state
**Cadrage / NOT DEPLOYED.** No cloud resources, paid accounts, posts, transactions or live storefront have been created by this repository.

See [financial baseline](docs/BUDGET-BASELINE.md), [architecture](docs/ARCHITECTURE.md) and [roadmap](docs/ROADMAP.md).
