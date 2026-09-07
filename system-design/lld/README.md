# Low-Level Design Practice

For a 45–60 minute round, explain requirements, entities, responsibilities, relationships, patterns, code, tests and trade-offs. Prefer simple, working designs over unnecessary patterns.

| # | Problem | Priority | Status | Score /10 | Last attempt | Next action |
|---|---|---|---|---:|---|---|
| 1 | Vending machine | High | ⬜ | - | - | State, inventory, payment, change |
| 2 | Parking lot | High | ⬜ | - | - | Allocation, pricing, extensibility |
| 3 | Elevator system | High | ⬜ | - | - | Scheduling, state, concurrency |
| 4 | Movie ticket booking | High | ⬜ | - | - | Seat holds, concurrency, payment |
| 5 | Food delivery | High | ⬜ | - | - | Order lifecycle, strategy, notifications |
| 6 | Ride sharing | High | ⬜ | - | - | Matching, trip state, fare strategy |
| 7 | Stock exchange | High | ⬜ | - | - | Order book, matching, FIFO, cancellation |
| 8 | Splitwise | Medium | ⬜ | - | - | Expenses, balances, settlement |
| 9 | ATM | Medium | ⬜ | - | - | State, cash dispensing, failures |
| 10 | Library management | Medium | ⬜ | - | - | Catalog, reservations, lending |
| 11 | Chess | Medium | ⬜ | - | - | Rules, pieces, move validation |
| 12 | Logging framework | High | ⬜ | - | - | Levels, appenders, thread safety |
| 13 | In-memory cache | High | ⬜ | - | - | LRU, TTL, concurrency |
| 14 | Rate limiter | High | ⬜ | - | - | Token bucket, injectable clock, tests |
| 15 | Task scheduler | High | ⬜ | - | - | Scheduling, cancellation, thread pools |
| 16 | Multi-tenant configuration service | High | ⬜ | - | - | Tenant scope, overrides, cache isolation |

## Design patterns to master

| Pattern | Typical usage | Status | Confidence /5 |
|---|---|---|---:|
| Strategy | Pricing, matching, allocation algorithms | ⬜ | 0 |
| State | Vending machine, orders, trips | ⬜ | 0 |
| Factory / Abstract Factory | Object creation families | ⬜ | 0 |
| Observer | Event notifications | ⬜ | 0 |
| Decorator | Logging, metrics, optional behavior | ⬜ | 0 |
| Adapter | External payment / provider integration | ⬜ | 0 |
| Command | Requests, undo, job execution | ⬜ | 0 |
| Chain of Responsibility | Validation and filter chains | ⬜ | 0 |
| Template Method | Shared algorithm with variable steps | ⬜ | 0 |
| Builder | Complex immutable objects | ⬜ | 0 |
| Repository | Persistence abstraction | ⬜ | 0 |
| Dependency Injection | Replaceable dependencies and testability | ⬜ | 0 |

## 60-minute LLD framework

1. Clarify requirements, edge cases and scope.
2. Identify entities, value objects, services and interfaces.
3. Define responsibilities and relationships; draw a class diagram.
4. Explain main flows and state transitions.
5. Select patterns only where they solve a real problem.
6. Implement the core behavior in Java.
7. Add unit tests, validation and concurrency handling where relevant.
8. Discuss extensibility, limitations and trade-offs.

## Design template

```markdown
# Problem
Date: | Duration: | Score: /10

## Requirements / out of scope
## Use cases and edge cases
## Entities and responsibilities
## Class diagram
## Interfaces and design patterns
## Main flow / sequence diagram
## Java implementation
## Tests and concurrency
## SOLID and extensibility
## Trade-offs
## Follow-up questions
## Improvements for next attempt
```

## Coding checklist

Use meaningful names, constructor injection, encapsulation and small interfaces. Avoid making every class a singleton or using inheritance where composition is simpler. Demonstrate important business rules with tests. For concurrent booking or inventory problems, explain atomicity and the actual persistence boundary rather than assuming synchronized Java methods solve distributed concurrency.
