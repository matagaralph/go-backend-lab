# Go Backend Lab

A hands-on laboratory for exploring backend engineering with Go, covering APIs, databases, concurrency, caching, distributed systems, performance, testing, and system design.

## Overview

This repository is dedicated to understanding backend engineering concepts through practical implementation, experimentation, testing, and performance analysis.

Rather than relying exclusively on frameworks and abstractions, the objective is to understand **how backend systems work internally, why engineering patterns exist, and how systems behave under failure and load**.

Each experiment focuses on a specific concept, progressing from fundamental backend development to advanced distributed systems and production engineering.

## Learning Areas

### 1. HTTP & API Engineering

- HTTP fundamentals and protocol behavior
- REST API design
- Routing, middleware, and request validation
- Context propagation and cancellation
- API versioning and pagination
- Idempotency
- Webhooks and signature verification
- Graceful shutdown

### 2. Testing & Code Quality

- Unit and integration testing
- Table-driven tests
- HTTP handler testing
- Dependency injection
- Test doubles and mocking
- Fuzz testing
- Benchmarking and profiling
- Race detection

### 3. Database Engineering

- PostgreSQL and SQL fundamentals
- Database modeling and indexing
- Transactions and ACID properties
- Transaction isolation levels
- Optimistic and pessimistic locking
- Connection pooling
- N+1 queries and query optimization
- Database migrations
- Replication and partitioning

### 4. Concurrency & Parallelism

- Goroutines and channels
- Mutexes and atomic operations
- Race conditions and deadlocks
- Worker pools
- Synchronization
- Context cancellation
- Goroutine and memory leaks
- Backpressure

### 5. Caching

- In-memory caching
- Redis
- Cache-aside and write-through strategies
- Cache invalidation
- TTL and eviction policies
- Cache stampedes
- Distributed caching

### 6. Resilience & Fault Tolerance

- Timeouts and retries
- Exponential backoff and jitter
- Circuit breakers
- Rate limiting
- Request deduplication
- Bulkheads
- Graceful degradation
- Failure recovery

### 7. Messaging & Event-Driven Systems

- Message queues
- Publish/subscribe
- Background workers
- Dead-letter queues
- Message delivery guarantees
- Event-driven architecture
- Transactional outbox pattern
- Eventual consistency

### 8. Networking & Security

- TCP, UDP, DNS, and TLS
- Reverse proxies
- Load balancing
- API gateways
- WebSockets and gRPC
- Authentication and authorization
- OAuth 2.0, JWT, and sessions
- Secrets management
- API security

### 9. Distributed Systems

- Horizontal and vertical scaling
- CAP theorem and consistency models
- Replication and sharding
- Distributed transactions
- Sagas
- Consensus and leader election
- CQRS and event sourcing
- Service discovery

### 10. Observability & Production Engineering

- Structured logging
- Metrics and monitoring
- Distributed tracing
- OpenTelemetry
- Health checks
- Performance profiling
- Load testing
- Docker and CI/CD
- Deployment and rollback strategies

### 11. System Design

- Requirements analysis
- Capacity estimation
- Architecture tradeoffs
- Scalability and reliability
- High-level and low-level design
- Failure analysis
- Architecture Decision Records

## Repository Structure

```text
go-backend-lab/
├── 01-http/
├── 02-testing/
├── 03-databases/
├── 04-concurrency/
├── 05-caching/
├── 06-resilience/
├── 07-messaging/
├── 08-networking/
├── 09-security/
├── 10-distributed-systems/
├── 11-observability/
├── 12-deployment/
├── projects/
└── README.md
```

Each directory contains focused experiments and practical implementations. Directories and experiments are added progressively.

Independent experiments may use separate Go modules to keep dependencies isolated.

## Experiment Methodology

Every experiment follows six principles:

1. **Understand:** Study the concept and the problem it solves.
2. **Implement:** Build a minimal working implementation using Go.
3. **Test:** Verify correctness, including edge cases and failure scenarios.
4. **Measure:** Benchmark performance when relevant.
5. **Break:** Simulate failures, concurrency issues, or unexpected behavior.
6. **Document:** Record observations, limitations, and engineering tradeoffs.

## Testing & Benchmarking

Testing is a core part of every experiment.

The repository emphasizes:

- Unit testing
- Integration testing
- Concurrency testing
- Benchmarking
- Failure simulation
- Performance profiling

Common Go commands:

```bash
# Run tests
go test ./...

# Run race detection
go test -race ./...

# Run benchmarks
go test -bench=. ./...

# Run tests with coverage
go test -cover ./...
```

Run these commands from the relevant Go module directory.

## Technology Stack

**Primary Language:** Go

**Core Technologies:**
- Go Standard Library
- PostgreSQL
- Redis
- Docker
- Linux

**Additional Technologies (introduced when needed):**
- RabbitMQ / Kafka
- Prometheus
- OpenTelemetry
- gRPC
- Kubernetes

Technologies are introduced to solve specific engineering problems rather than simply increase the number of tools used.

## Engineering Principles

- Understand fundamentals before introducing abstractions.
- Prefer simplicity over unnecessary complexity.
- Test behavior rather than implementation details.
- Measure performance before optimizing.
- Design for failure, not only successful execution.
- Understand consistency, reliability, and scalability tradeoffs.
- Treat observability and security as engineering requirements.
- Document decisions and lessons learned.

## Resources

- [Go Documentation](https://go.dev/doc/)
- [Learn Go with Tests](https://quii.gitbook.io/learn-go-with-tests)
- [Go Blog](https://go.dev/blog/)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)
- [Redis Documentation](https://redis.io/docs/latest/)
- [OpenTelemetry Documentation](https://opentelemetry.io/docs/)
- [Backend Developer Roadmap](https://roadmap.sh/backend)
- [System Design Notes](https://github.com/liquidslr/system-design-notes)

## Philosophy

**Understand the concept. Build the implementation. Test its behavior. Measure its performance. Explore its failures.**

The objective is to develop the engineering judgment needed to build reliable, maintainable, and scalable backend systems,not simply to learn frameworks or memorize architectural patterns.
