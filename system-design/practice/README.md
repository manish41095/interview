# Mock Interview and Revision Tracker

Use one timed mock each week. Do not mark a mock complete until feedback and next actions are recorded.

| Mock | Date | Problem | Duration | Requirements /10 | Architecture /10 | Problem-solving /10 | Scale / trade-offs /10 | Communication /10 | Overall /10 | Re-attempt |
|---|---|---|---|---:|---:|---:|---:|---:|---:|---|
| 01 | - | Multi-tenant SaaS | - | - | - | - | - | - | - | - |
| 02 | - | URL shortener | - | - | - | - | - | - | - | - |
| 03 | - | Food delivery | - | - | - | - | - | - | - | - |
| 04 | - | Ride sharing | - | - | - | - | - | - | - | - |
| 05 | - | Movie ticket booking | - | - | - | - | - | - | - | - |
| 06 | - | Notification system | - | - | - | - | - | - | - | - |
| 07 | - | Stock exchange | - | - | - | - | - | - | - | - |
| 08 | - | Payment system | - | - | - | - | - | - | - | - | - |
| 09 | - | Distributed scheduler | - | - | - | - | - | - | - | - | - |
| 10 | - | Media storage service | - | - | - | - | - | - | - | - | - |

Overall = average of the five category scores. Scores are self-assessments until independently reviewed.

## Scoring rubric

**Requirements:** 0–3 misses core use cases; 4–6 reasonable scope but missing constraints; 7–8 clear scope and NFRs; 9–10 proactively resolves ambiguity and prioritizes.

**Architecture:** 0–3 incomplete; 4–6 workable but weak flows or data model; 7–8 coherent design with justified components; 9–10 clear evolution and boundaries.

**Problem-solving:** 0–3 names technologies without solving the hard problem; 4–6 partial solution; 7–8 correct core algorithm and edge cases; 9–10 handles difficult follow-ups independently.

**Scale / trade-offs:** 0–3 unsupported claims; 4–6 basic scaling; 7–8 sensible estimates, consistency and failures; 9–10 explicit alternatives, bottlenecks and recovery.

**Communication:** 0–3 difficult to follow; 4–6 understandable but unstructured; 7–8 clear time management and diagrams; 9–10 concise, collaborative and confident under questions.

## Weekly review

Record: topics learned, designs completed, mocks attempted, score trend, top three weaknesses, actions completed and next week's priorities. A low score is useful evidence for deciding what to practice next.

## Revision queue

| Topic / design | Why revision is needed | Last attempt | Next revision | Action | Done |
|---|---|---|---|---|---|
| Multi-tenancy | No direct production ownership; build design depth | - | - | Compare isolation models and design tenant-aware request flow | ⬜ |
| Distributed transactions | Baseline assessment needed | - | - | Explain outbox + Saga with failure scenarios | ⬜ |
| Database scaling | Baseline assessment needed | - | - | Explain partitioning vs sharding and migration strategy | ⬜ |

## Daily practice journal

```markdown
# YYYY-MM-DD
Time spent:
Topic / problem:
What I learned:
What I explained without notes:
What I implemented / designed:
Questions I could not answer:
Confidence before → after:
Next revision date:
Tomorrow's next action:
```

## Interview question bank

Keep questions you actually struggled with. Record your first answer, corrected answer, concise explanation and one follow-up. Examples: How do you prevent duplicate orders? What happens when a Kafka consumer crashes after a DB commit? How do you stop tenant A reading tenant B's data? How do you migrate a large table without downtime? How do you handle a slow downstream service exhausting a thread pool?
