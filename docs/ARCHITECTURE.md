# Target architecture — incremental design

## Logical flow

```mermaid
flowchart TD
  Channels[Web / newsletter / social / marketplaces] --> Edge[CDN WAF and API]
  Edge --> App[Public web and commerce API]
  App --> DB[(PostgreSQL / pgvector)]
  App --> Storage[(Object storage)]
  Operator[Human admin cockpit] --> Policy[Approval policy + budget controls]
  CEO[AI CEO: proposals, not unlimited authority] --> Policy
  Policy --> Queue[Durable workflows and job queue]
  Queue --> Research[Research agent]
  Queue --> Media[Original content factory]
  Queue --> Commerce[Commerce agent]
  Queue --> Growth[Channel/growth agent]
  Queue --> Finance[FinOps/analytics]
  Research --> Evidence[Source and provenance store]
  Media --> Review[Quality/factual and rights review]
  Review --> Publish[Approved platform connectors]
  Publish --> Channels
  Finance --> CEO
  ```

## Implementation baseline
- Next.js responsive commerce/content storefront; mobile comes after traction.
- FastAPI backend; PostgreSQL; object storage; asynchronous durable jobs and outbox.
- Hosted model APIs chosen by task and measured total cost; do not require a GPU for MVP.
- Containerized local development and reproducible deployment; Terraform for infrastructure. Kubernetes only after operational demand validates it.
- No secrets in Git. Isolated credentials by channel and environment; minimal scopes; secure key rotation.
- Telemetry: request IDs, cost tracing, business events, publishing delivery receipts, retries, idempotency, audit trail.
- Recovery: database backups and restore tests, storage lifecycle, failed job dead-letter handling.
- Payments use approved checkout provider; never store payment card data directly.
- A social/marketplace integration is enabled only after verifying API permission, platform rules, and explicit account linkage.

## Autonomous action policy
**Automatic**: reversible internal research, drafting, classification, unit-cost estimates, scheduler of preapproved low-risk posts.

**Human approval required**: initial public activation, sensitive factual claims, new paid subscription/products with legal commitments, account creation, payouts/refunds exceptions, paid advertising budgets, pricing beyond allowed bands, deletion and irreversible changes.

**Prohibited**: fabricated testimony or evidence, undisclosed synthetic persons, impersonation, illicit goods, manipulative fear-based selling, platform anti-bot circumvention.

## Security and acceptance gates
Document threat model, data lifecycle, GDPR notices, consent, user deletion, abuse reports, age/sensitive-content rules, supply chain scanning, budget cutoff and operations runbooks prior to public launch.
