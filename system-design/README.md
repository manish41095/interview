# System Design Interview Tracker — Manish

A practical tracker for Java Backend / Senior / Tech Lead interview preparation.

## Goal

Track progress across concepts, HLD, LLD, mock interviews, revision, and real-project examples.

Use this loop for every topic:

**Learn → Explain → Apply → Mock → Fix gaps → Re-solve**

## Status legend

- ⬜ Not started
- 🟨 Learning
- 🟦 Can explain
- 🟩 Can apply in design
- ✅ Interview ready

## Confidence scale

| Score | Meaning |
|---|---|
| 0 | Not studied |
| 1 | Recognize the topic |
| 2 | Can explain basics |
| 3 | Can explain internals + trade-offs |
| 4 | Can apply independently in a system design |
| 5 | Can defend decisions under senior/lead follow-up questions |

## Current priority areas

| Area | Status | Confidence /5 | Priority | Last revised | Next action |
|---|---:|---:|---:|---|---|
| Core scalability patterns | ⬜ | 0 | High | - | Learn load balancing, horizontal scaling, statelessness |
| Database scaling | ⬜ | 0 | High | - | Indexing, replication, partitioning, sharding |
| Caching | ⬜ | 0 | High | - | Cache-aside, invalidation, stampede, Redis |
| Kafka / messaging | ⬜ | 0 | High | - | Ordering, partitions, retries, DLQ, idempotency |
| Distributed transactions | ⬜ | 0 | High | - | Saga, outbox, compensation |
| Rate limiting | ⬜ | 0 | Medium | - | Token bucket, sliding window, distributed limiter |
| Multi-tenancy | 🟨 | 1 | **Very High** | - | Design tenant isolation end-to-end |
| Security | 🟨 | 2 | High | - | OAuth2/JWT, service-to-service auth, tenant authorization |
| Observability | ⬜ | 0 | Medium | - | Logs, metrics, tracing, SLI/SLO |
| Reliability | ⬜ | 0 | High | - | Retry, timeout, circuit breaker, bulkhead |

> Update confidence only after explaining the topic without notes or using it in a mock interview.

## Interview readiness dashboard

| Track | Target | Current |
|---|---:|---:|
| Core system-design concepts | 35+ topics | 0 |
| HLD problems completed | 15 | 0 |
| LLD problems completed | 12 | 0 |
| Timed mocks completed | 10 | 0 |
| Designs re-attempted after feedback | 5 | 0 |
| Topics at confidence 4+ | 25 | 0 |

## Recommended 45–60 minute HLD flow

1. Clarify functional requirements
2. Clarify non-functional requirements and scale
3. Back-of-the-envelope estimation
4. APIs
5. Data model
6. High-level architecture
7. Deep dive into 1–2 difficult components
8. Scaling, reliability and security
9. Trade-offs and alternatives
10. Summarize the final design

## Repository structure

```text
system-design/
├── README.md
├── concepts/
│   └── README.md
├── hld/
│   └── README.md
├── lld/
│   └── README.md
├── practice/
│   └── README.md
└── templates/
    └── mock-interview.md
```

## Rules for this tracker

1. Do not mark a topic complete because you read it once.
2. Add at least one real-project example for important concepts.
3. Every HLD must contain explicit trade-offs.
4. Every mock must record where points were lost.
5. Re-attempt weak designs after 7–14 days.
6. For gaps such as multi-tenancy, be transparent about production experience and build strong conceptual + design depth.

## Weekly routine

- Mon–Thu: concepts + one design section each day
- Fri: complete one full HLD or LLD
- Sat: 45–60 minute mock interview
- Sun: revise weak areas and update scores

## Target profile

This tracker is optimized for experienced Java backend interviews involving:

- Java / concurrency
- Spring Boot
- Microservices
- Spring Security / JWT / OAuth2
- Kafka / asynchronous processing
- SQL / PostgreSQL / database scaling
- Redis / caching
- Distributed systems
- HLD / LLD
- Senior Engineer / Tech Lead architecture discussions
