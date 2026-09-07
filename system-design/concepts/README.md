# Concept Knowledge Tracker

For each topic, record status, confidence (0–5), last revision date, next revision date and evidence. All initial scores are unassessed, not claims about existing knowledge.

## Foundations

| Topic | Status | Score | Last revised | Next revision | Evidence / gap |
|---|---|---:|---|---|---|
| Functional vs non-functional requirements | ⬜ | 0 | - | - | |
| Latency, throughput, availability | ⬜ | 0 | - | - | |
| Capacity estimation, QPS, storage, bandwidth | ⬜ | 0 | - | - | |
| HTTP, HTTPS, TCP, DNS | ⬜ | 0 | - | - | |
| REST, gRPC, WebSockets | ⬜ | 0 | - | - | |
| Load balancing L4 vs L7 | ⬜ | 0 | - | - | |
| Stateless services and horizontal scaling | ⬜ | 0 | - | - | |
| CDN and object storage | ⬜ | 0 | - | - | |

## Database and caching

| Topic | Status | Score | Last revised | Next revision | Evidence / gap |
|---|---|---:|---|---|---|
| SQL vs NoSQL selection | ⬜ | 0 | - | - | |
| Indexes, B-tree, composite indexes | ⬜ | 0 | - | - | |
| Transactions, ACID, isolation levels | ⬜ | 0 | - | - | |
| Optimistic and pessimistic locking | ⬜ | 0 | - | - | |
| Replication and read replicas | ⬜ | 0 | - | - | |
| Partitioning vs sharding | ⬜ | 0 | - | - | |
| Consistent hashing | ⬜ | 0 | - | - | |
| CAP, consistency models, quorum | ⬜ | 0 | - | - | |
| Redis and cache-aside | ⬜ | 0 | - | - | |
| Cache invalidation, TTL, eviction | ⬜ | 0 | - | - | |
| Cache stampede, penetration, hot keys | ⬜ | 0 | - | - | |
| Distributed locking | ⬜ | 0 | - | - | |

## Distributed systems and reliability

| Topic | Status | Score | Last revised | Next revision | Evidence / gap |
|---|---|---:|---|---|---|
| Kafka partitions, consumer groups, ordering | ⬜ | 0 | - | - | |
| At-most-once, at-least-once, exactly-once semantics | ⬜ | 0 | - | - | |
| Idempotency and deduplication | ⬜ | 0 | - | - | |
| Retry, exponential backoff, jitter | ⬜ | 0 | - | - | |
| Dead-letter queues and poison messages | ⬜ | 0 | - | - | |
| Transactional outbox | ⬜ | 0 | - | - | |
| Saga choreography vs orchestration | ⬜ | 0 | - | - | |
| Timeouts, circuit breakers, bulkheads | ⬜ | 0 | - | - | |
| Rate limiting algorithms | ⬜ | 0 | - | - | |
| Backpressure and bounded queues | ⬜ | 0 | - | - | |
| Distributed tracing, metrics, logs | ⬜ | 0 | - | - | |
| SLI, SLO, error budgets | ⬜ | 0 | - | - | |
| Leader election and distributed coordination | ⬜ | 0 | - | - | |
| Eventual consistency and reconciliation | ⬜ | 0 | - | - | |

## Security, SaaS and Java backend

| Topic | Status | Score | Last revised | Next revision | Evidence / gap |
|---|---|---:|---|---|---|
| OAuth2, OIDC, JWT | ⬜ | 0 | - | - | |
| Authentication vs authorization | ⬜ | 0 | - | - | |
| Service-to-service authentication, mTLS | ⬜ | 0 | - | - | |
| Multi-tenancy isolation models | ⬜ | 0 | - | - | |
| Tenant-aware authentication and authorization | ⬜ | 0 | - | - | |
| Tenant-aware caching and background jobs | ⬜ | 0 | - | - | |
| Tenant onboarding, migration, backup and quotas | ⬜ | 0 | - | - | |
| Java thread pools and blocking I/O | ⬜ | 0 | - | - | |
| CompletableFuture and context propagation | ⬜ | 0 | - | - | |
| Spring transactions and connection pools | ⬜ | 0 | - | - | |
| Spring Security filter chain | ⬜ | 0 | - | - | |
| API versioning and backward compatibility | ⬜ | 0 | - | - | |

## Concept study template

Copy this for each concept:

```markdown
# Concept name
Status: ⬜ | Confidence: 0/5
Last revised: - | Next revision: -

## What is it?
## Why is it needed?
## How does it work internally?
## Simple example
## Trade-offs and limitations
## Real-project usage (only verified personal experience)
## Interview follow-up questions
## My 60-second explanation
## Gaps / next action
```

## Revision policy

Revise after 1 day, 3 days, 7 days, 14 days and 30 days where practical. A successful revision means explaining without notes, not rereading. Move the next revision earlier when a mock exposes a weakness.
