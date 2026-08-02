<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1f2937&height=180&section=header&text=Arjun%20Patidar&fontSize=52&fontColor=e6edf3&fontAlignY=40&desc=Backend%20Full%20Stack%20Engineer&descAlignY=62&descSize=18&descColor=8b949e&animation=fadeIn" width="100%"/>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/arjun-patidar-6556b2226)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arjunjagotra2001@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/arjun808)
[![Profile Views](https://komarev.com/ghpvc/?username=arjun808&style=for-the-badge&color=0d1117&label=PROFILE+VIEWS)](https://github.com/arjun808)

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Backend+Engineer+%7C+Distributed+Systems;Event-Driven+Architecture+%7C+Kafka+%7C+SQS;AWS+Serverless+%7C+NestJS+%7C+MongoDB;Building+for+Scale%2C+Resilience%2C+and+Clarity" alt="Typing SVG" />

</div>

---

## 🧑‍💻 About Me

I'm a **backend-first full stack engineer** with **3+ years** of experience designing and shipping production-grade, distributed systems. I specialize in **event-driven architecture**, **serverless infrastructure**, and **high-throughput data pipelines** — while retaining enough frontend depth to ship features end-to-end without handoffs.

I care deeply about **system correctness under failure** — idempotency, at-least-once delivery guarantees, race condition safety, and dead-letter queue handling are not afterthoughts in my systems; they're first-class design constraints.

```text
⚙️  Architecture   →   Event-driven · Distributed · Serverless · Domain-Driven
📐  Philosophy     →   Design for failure first. Optimize for scale second.
🔭  Currently      →   Owning backend systems & core business logic at duochat
🌍  Open To        →   Backend / Full Stack roles in product-driven teams
```

---

## 🏗️ Backend Engineering — Deep Dives

### ⚡ Event-Driven & Messaging Systems
- Architected **multi-consumer Kafka pipelines** with topic partitioning for parallelism, consumer group isolation, and lag monitoring
- Implemented **at-least-once delivery** with idempotency keys to prevent duplicate processing across retries
- Designed **SQS FIFO queues** for strict ordering with deduplication IDs and visibility timeouts tuned per job complexity
- Built **SNS fan-out patterns** for decoupled, multi-subscriber event broadcasting across service domains
- Applied **dead-letter queue (DLQ) routing** with CloudWatch alarms and automated replay strategies for failed events
- Implemented **transactional outbox pattern** to guarantee consistency between DB writes and event emissions

### ☁️ Serverless & AWS Infrastructure
- Built **Lambda-based async workflows** triggered via SQS, SNS, and API Gateway with cold-start mitigation via provisioned concurrency
- Designed **fully decoupled serverless pipelines** for lead scoring, webhook ingestion, and scheduled report generation
- Used **API Gateway + Lambda authorizers** for custom JWT/token-based auth enforced at the edge
- Implemented **S3 event-driven processing** — file upload → SQS → Lambda → DB ingestion pipelines
- Configured **CloudWatch dashboards & metric filters** for real-time alerting on Lambda errors, DLQ depth, and P95 latency
- Managed infrastructure patterns across **EC2, VPC, IAM roles/policies**, and **Secrets Manager**

### 🗄️ MongoDB — Production Patterns
- Designed **compound and partial indexes** supporting high-cardinality filter queries with sub-10ms response times
- Built **multi-stage aggregation pipelines** (`$lookup`, `$unwind`, `$group`, `$facet`) powering live analytics dashboards
- Applied **bucket pattern** for time-series chat data to reduce document count and improve range query efficiency
- Implemented **read preference tuning** (secondary reads for analytics) to offload the primary and reduce hot-spot writes
- Used **MongoDB change streams** as lightweight event triggers for cache invalidation and downstream service sync
- Performed **systematic query profiling** via `explain()` and slow query logs — achieving meaningful P95 latency reductions in production

### 🔌 Real-Time Infrastructure — WebSockets at Scale
- Designed *WebSocket gateway* in NestJS with room-based namespacing for multi-tenant chat isolation
- Built **Kafka-backed fan-out** — socket events emitted from a Kafka consumer, not the originating service, enabling horizontal scaling
- Implemented **presence tracking** with Redis TTL keys and heartbeat intervals for accurate agent online/offline state
- Handled **socket reconnection logic** with event buffering and replay windows to prevent message loss on disconnect
- Designed **backpressure-aware consumers** to throttle ingestion when downstream services are degraded

### 🏛️ NestJS Architecture & Clean Code
- Structured large NestJS codebases using **modular DDD** — domain-bounded modules, use-case interactors, and repository interfaces
- Applied **CQRS pattern** with command/query separation for write-heavy domains (chat assignment, analytics writes)
- Used **custom interceptors** for request logging, response serialization, and distributed tracing header propagation
- Implemented **custom exception filters** for structured error responses and Sentry/CloudWatch error forwarding
- Wrote **unit + integration tests** with Jest and Supertest — service logic fully isolated via mock repositories
- Enforced **contract-first API design** with Swagger decorators and class-validator DTOs with complete type safety

### 🔒 Resilience & Production Reliability
- Implemented **exponential backoff + jitter** on SQS/Kafka retry handlers to prevent thundering herd on cascading failure
- Designed **circuit breaker wrappers** (via `opossum`) around third-party calls (Stripe, external APIs) with half-open probes
- Applied **optimistic locking** on MongoDB documents for concurrent update conflicts (e.g., agent assignment races)
- Built **idempotency middleware** for webhooks and payment events — deduplication via Redis with configurable TTL windows
- Structured services for **graceful shutdown** — drain in-flight messages before SIGTERM completes in ECS/Kubernetes environments
- Maintained **saga-style distributed transactions** across services with compensating rollback actions on partial failure

---

## 🏢 Current Work — duochat

> Real-time communication & customer engagement platform. I own core backend systems and business logic powering live chat at scale.

| What I Built | Outcome |
|---|---|
| **Event-driven chat infrastructure** — Kafka consumers across assignment, notification & analytics domains | All domain concerns fully decoupled; horizontally scalable |
| **Chat assignment engine** — rule-based routing with race condition safety & SLA tracking | Zero double-assignments in production |
| **Serverless automation** — Lambda for lead scoring, webhook ingestion & scheduled reports | Eliminated all cron-based bottlenecks |
| **MongoDB analytics pipelines** — live dashboards with compound indexes & multi-stage aggregations | Significant P95 latency reduction on key queries |
| **NestJS monolith decomposition** — modular DDD refactor with clean domain boundaries | Reduced coupling; faster deploys and improved testability |
| **WebSocket presence system** — Redis-backed heartbeat + Kafka fan-out for real-time state | Accurate agent availability tracking at scale |

---

## 🛠️ Tech Stack

<div align="center">

### Backend & Runtime
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![REST API](https://img.shields.io/badge/REST-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

### Messaging & Event Systems
![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Amazon SQS](https://img.shields.io/badge/AWS%20SQS-FF9900?style=for-the-badge&logo=amazonsqs&logoColor=white)
![Amazon SNS](https://img.shields.io/badge/AWS%20SNS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)

### AWS & Cloud Infrastructure
![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)
![Amazon EC2](https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![API Gateway](https://img.shields.io/badge/API%20Gateway-FF4F8B?style=for-the-badge&logo=amazonaws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

### Databases & Caching
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)

### Payments & Tooling
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🎯 What I'm Excited to Work On

```
✅  High-throughput event pipelines    →   Kafka, SQS, SNS, outbox pattern, fan-out
✅  AWS serverless architectures       →   Lambda, API Gateway, S3 triggers, provisioned concurrency
✅  MongoDB schema design at scale     →   Aggregations, indexing strategy, change streams
✅  Resilient system design            →   DLQ, circuit breakers, idempotency, sagas, backpressure
✅  Clean, modular NestJS codebases    →   CQRS, DDD, dependency injection, clean boundaries
✅  Real-time systems                  →   WebSockets, presence tracking, Kafka-backed fan-out
```

---

## 📫 Let's Connect

<div align="center">

| Platform | Link |
|---|---|
| 💼 LinkedIn | [arjun-patidar-6556b2226](https://www.linkedin.com/in/arjun-patidar-6556b2226) |
| 📧 Email | [arjunjagotra2001@gmail.com](mailto:arjunjagotra2001@gmail.com) |
| 🐙 GitHub | [github.com/arjun808](https://github.com/arjun808) |

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1f2937,50:161b22,100:0d1117&height=100&section=footer" width="100%"/>

*Open to backend-heavy or full-stack roles. I bring architectural clarity, production discipline, and end-to-end ownership.*

</div>
