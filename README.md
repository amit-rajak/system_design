# System Design

## What is System Design?

System design is the process of defining the architecture, components, modules, interfaces, and data flow of a software system so it can meet functional and non-functional requirements at scale.

It answers questions like:

- How should the system be structured?
- How do services communicate?
- Where is data stored, cached, and replicated?
- How do we handle growth, failures, and latency?

### Why it matters

Good system design helps you build systems that are:

- **Scalable** — handle more users and data without a full rewrite
- **Reliable** — keep working when parts fail
- **Performant** — stay fast under load
- **Maintainable** — easy to change and operate over time

### Typical building blocks

| Concern | Common approaches |
| --- | --- |
| Traffic | Load balancers, reverse proxies, CDNs |
| Compute | App servers, microservices, serverless |
| Data | SQL/NoSQL databases, sharding, replication |
| Speed | Caching (Redis, Memcached), CDN |
| Async work | Message queues, event streams |
| Discovery | DNS, service registry, API gateway |

### High-level process

1. **Clarify requirements** — functional goals and constraints (QPS, latency, consistency)
2. **Estimate scale** — users, storage, bandwidth, growth
3. **Sketch the API** — core endpoints and data models
4. **Draw the architecture** — clients → edge → services → data stores
5. **Deep dive** — bottlenecks, caching, consistency, failure modes
6. **Iterate** — trade-offs between simplicity, cost, and performance

System design is less about a single “correct” answer and more about making clear trade-offs for the problem at hand.
