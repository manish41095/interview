# High-Level Design Practice

Complete one system in 45–60 minutes. A design is complete only after a timed explanation, trade-off discussion and recorded feedback. Initial progress is unassessed.

| # | Problem | Priority | Status | Score /10 | Last attempt | Next action |
|---|---|---|---|---:|---|---|
| 1 | URL shortener | High | ⬜ | - | - | Requirements, key generation, redirects, caching |
| 2 | Rate limiter | High | ⬜ | - | - | Token bucket, Redis atomicity, distributed limits |
| 3 | Notification system | High | ⬜ | - | - | Queues, retries, preferences, DLQ |
| 4 | Multi-tenant supply-chain SaaS | Very High | ⬜ | - | - | Tenant isolation, onboarding, inventory, orders |
| 5 | Food delivery | High | ⬜ | - | - | Order lifecycle, dispatch, consistency |
| 6 | Ride sharing | High | ⬜ | - | - | Geo search, matching, real-time location |
| 7 | Movie ticket booking | High | ⬜ | - | - | Seat locking, payment, expiration |
| 8 | E-commerce order and inventory | High | ⬜ | - | - | Reservation, idempotency, Saga |
| 9 | Payment system | High | ⬜ | - | - | Ledger, idempotency, reconciliation |
| 10 | Chat / messaging | Medium | ⬜ | - | - | WebSockets, ordering, offline delivery |
| 11 | News feed | Medium | ⬜ | - | - | Fanout, ranking, hot users |
| 12 | File storage / media service | High | ⬜ | - | - | Uploads, metadata, storage, cleanup |
| 13 | Distributed job scheduler | High | ⬜ | - | - | Leases, retries, duplicate execution |
| 14 | Stock exchange / order matching | High | ⬜ | - | - | Ordering, matching, durability, latency |
| 15 | Distributed cache | Medium | ⬜ | - | - | Partitioning, eviction, replication |
| 16 | Search autocomplete | Medium | ⬜ | - | - | Trie, indexing, ranking, cache |
| 17 | Metrics / logging platform | Medium | ⬜ | - | - | Ingestion, aggregation, retention |
| 18 | API gateway | Medium | ⬜ | - | - | Routing, auth, quotas, resilience |

## 60-minute interview structure

| Time | Activity |
|---|---|
| 0–5 min | Clarify functional requirements and scope |
| 5–10 min | Non-functional requirements, traffic and storage estimates |
| 10–15 min | APIs and data model |
| 15–25 min | Draw architecture and explain main request flow |
| 25–40 min | Deep dive into the hardest components |
| 40–50 min | Scale, consistency, failures, security, observability |
| 50–60 min | Trade-offs, alternatives and follow-up questions |

## Design answer template

```markdown
# System name
Date: | Duration: | Mock score: /10

## 1. Clarifying questions
## 2. Functional requirements and out of scope
## 3. Non-functional requirements and assumptions
## 4. Estimation (QPS, peak, storage, bandwidth)
## 5. APIs and contracts
## 6. Data model and indexes
## 7. High-level architecture diagram
## 8. Critical request / event flows
## 9. Deep dive: hardest component
## 10. Scaling and partitioning
## 11. Consistency, concurrency and idempotency
## 12. Failure handling, retries and recovery
## 13. Security and observability
## 14. Trade-offs and alternatives
## 15. 60-second summary
## 16. Interviewer follow-ups and missed points
## 17. Next revision / re-attempt date
```

## First priority: Multi-tenant supply-chain SaaS

Practice the architecture for tenant onboarding, users/roles, products, warehouses, inventory, purchase orders and order fulfillment. Compare shared-schema, schema-per-tenant and database-per-tenant approaches. Define how the authenticated tenant is resolved and authorized, how all queries and caches maintain isolation, and how background jobs preserve tenant context. Discuss migrations, quotas, noisy neighbors, audit trails, backup/restore and tenant-specific configuration.

Start with a modular monolith or a small number of services unless scale and team boundaries justify more. Explain the trade-offs rather than assuming microservices are always necessary.

### Interview challenge

A customer belongs to tenant A but sends tenant B's ID in a request. Explain every defense layer and how you would test for data leakage. Then explain tenant isolation for a Kafka consumer, Redis key and scheduled job. Never trust an unvalidated client-supplied tenant ID.

## Real-project evidence

Use actual experience as a bridge to design principles. Candidate examples to verify and document include a media ingestion/retrieval pipeline, bounded FTP worker pools, PostgreSQL time partitioning, cache → filesystem → database retrieval, inventory recovery and cleanup coordination. Record what you personally owned, measurable scale if known, the problem, decision, trade-off and result. Do not publish proprietary code, customer data or internal infrastructure details.
