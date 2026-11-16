<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1f2937&height=190&section=header&text=Arjun%20Patidar&fontSize=52&fontColor=e6edf3&fontAlignY=38&desc=Backend%20%7C%20AI%20%7C%20Full%20Stack%20Engineer&descAlignY=62&descSize=18&descColor=8b949e&animation=fadeIn" width="100%"/>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/arjun-patidar-6556b2226)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arjunjagotra2001@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/arjun808)
[![Profile Views](https://komarev.com/ghpvc/?username=arjun808&style=for-the-badge&color=0d1117&label=PROFILE+VIEWS)](https://github.com/arjun808)

</div>

---

## 👋 About Me

I'm a **backend-focused full stack engineer** working at the intersection of **backend systems, distributed architecture, and AI engineering**. I build production-oriented applications, scalable APIs, event-driven workflows, and LLM-powered features.

My experience includes building multi-tenant platforms, real-time communication systems, background processing pipelines, and AI-powered sales experiences. I've worked with **Node.js, NestJS, TypeScript, MongoDB, Redis, Kafka, AWS, OpenAI APIs, and Pinecone**.

I enjoy solving problems that sit between application engineering and AI: connecting LLMs to reliable business workflows, grounding responses in relevant data with RAG, and enabling models to interact with application capabilities through function calling.

```text
⚙️  Focus           → Backend Engineering · AI Engineering · Distributed Systems
🧠  AI               → LLMs · RAG · Embeddings · Vector Search · Tool Calling · AI Agents
🏗️  Backend          → Node.js · NestJS · Kafka · Redis · MongoDB · AWS
🌱  Building toward  → Reliable, scalable and useful AI-powered products
🌍  Open to          → Backend · AI Engineer · Full Stack opportunities
```

---

## 🧠 AI Engineering

I work on integrating LLM capabilities into real application workflows, with a focus on retrieval, tool execution, and reliable backend orchestration.

### Retrieval-Augmented Generation (RAG)
- Implemented RAG-based knowledge retrieval using **Pinecone** as a vector database.
- Worked with document/query embeddings and semantic similarity search to retrieve context relevant to a user's query.
- Connected retrieved context with LLM prompts to support grounded, context-aware responses.
- Worked with the retrieval flow: query embedding → vector search → relevant chunk retrieval → context construction → LLM response.
- Focus on retrieval relevance, context quality, and keeping application data connected to generated answers.

### LLM Integration & AI Agents
- Built AI-powered sales-agent capabilities using **OpenAI APIs and function calling**.
- Connected LLM-driven decisions to application functions so the agent can interact with business workflows and structured application data.
- Worked on tool/function schemas, passing arguments, executing backend operations, and returning tool results to the model.
- Designed backend flows that coordinate model requests, tool execution, and follow-up model responses.
- Explored agentic workflows where an LLM can choose an appropriate tool based on the user's intent and available context.

### AI Application Engineering
- Integrated AI capabilities into an existing multi-tenant product rather than treating AI as a standalone chatbot.
- Worked across API design, backend orchestration, data retrieval, and application integration.
- Focus on practical AI concerns: prompt and context construction, retrieval quality, tool execution, error handling, and predictable application behavior.

### AI Engineering Toolkit

![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-5A45FF?style=for-the-badge)
![LLM](https://img.shields.io/badge/LLM_Applications-2563EB?style=for-the-badge)
![Vector Search](https://img.shields.io/badge/Vector_Search-0F766E?style=for-the-badge)
![AI Agents](https://img.shields.io/badge/AI_Agents-7C3AED?style=for-the-badge)

---

## 🏗️ Backend Engineering

### ⚡ Event-Driven Architecture & Messaging
- Worked with **Kafka consumer groups, partitions, and event-driven processing** to decouple application workflows.
- Designed asynchronous processing flows using **Amazon SQS and SNS**.
- Applied idempotency strategies to make retryable event processing safer.
- Used dead-letter queues (DLQs), retry handling, and visibility timeouts to improve message-processing reliability.
- Explored the **transactional outbox pattern** for coordinating database updates with event publication.

### ☁️ AWS & Serverless
- Built asynchronous workflows using **AWS Lambda, SQS, SNS, and API Gateway**.
- Worked with webhook ingestion and background processing patterns.
- Used **S3** for object storage and event-driven processing workflows.
- Worked with CloudWatch logs and monitoring to investigate production issues.
- Familiar with IAM, EC2, VPC, and Secrets Manager fundamentals.

### 🗄️ Database Engineering & Performance
- Designed MongoDB indexes and aggregation pipelines for application-specific query patterns.
- Used `explain()` to investigate query execution and identify inefficient database operations.
- Improved a chat retrieval API from approximately **5–6 seconds to 200–300 ms** through indexing, query optimization, aggregation, and reducing unnecessary database round trips.
- Worked with `$lookup`, `$unwind`, `$group`, `$facet`, and Mongoose `.lean()`.
- Used Redis for caching, TTL-based data, presence tracking, and background workflow support.
- Familiar with relational database concepts, PostgreSQL, SQL, transactions, and data modeling.

### 🔌 Real-Time Systems
- Built real-time application features using **WebSockets and NestJS**.
- Worked with Redis-backed presence and online/offline state.
- Designed event flows for chat, assignment, and notification use cases.
- Considered reconnection, duplicate events, concurrency, and horizontal scaling in real-time workflows.

### 🏛️ NestJS & Application Architecture
- Build modular backend applications using NestJS, TypeScript, dependency injection, and clear module boundaries.
- Apply separation of concerns across controllers, services, repositories, and domain logic.
- Work with DTO validation, Swagger/OpenAPI documentation, interceptors, and exception handling.
- Write unit and integration tests using Jest and Supertest.
- Familiar with CQRS, DDD, and clean architecture concepts.

### 🔒 Reliability & Distributed Systems
- Design retry-safe operations using idempotency and deduplication.
- Understand at-least-once delivery and the implications of duplicate message processing.
- Work with optimistic concurrency control and race-condition prevention.
- Use timeouts, retry strategies, and failure handling when integrating external services.
- Understand trade-offs around consistency, availability, ordering, and eventual consistency in distributed systems.

---

## 🏢 Product Experience — Duochat

**Duochat** is an omnichannel CRM and customer-engagement platform that brings customer conversations and AI-powered workflows together.

As a founding engineer, I worked across backend architecture, core product features, and AI-powered capabilities.

| Area | Work |
|---|---|
| **Multi-tenant architecture** | Built backend capabilities for a platform serving multiple businesses with tenant-aware data and workflows. |
| **AI sales agent** | Worked on an AI-powered sales agent using OpenAI function calling to connect model decisions with application capabilities. |
| **RAG implementation** | Integrated Pinecone-based vector retrieval to provide relevant context to LLM-powered experiences. |
| **Chat infrastructure** | Worked on unified conversation and messaging workflows across customer communication channels. |
| **Database performance** | Optimized MongoDB queries and reduced a chat retrieval API from approximately 5–6 seconds to 200–300 ms. |
| **Background processing** | Used Redis and asynchronous job workflows for scheduled and background operations. |
| **Billing and integrations** | Worked on billing-related functionality and third-party integrations, including payment and commerce workflows. |

---

## 🛠️ Tech Stack

### Backend & Languages
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

### AI & LLM Engineering
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-5A45FF?style=for-the-badge)
![Embeddings](https://img.shields.io/badge/Embeddings-2563EB?style=for-the-badge)
![Vector Databases](https://img.shields.io/badge/Vector_Databases-0F766E?style=for-the-badge)
![Function Calling](https://img.shields.io/badge/Function_Calling-7C3AED?style=for-the-badge)
![AI Agents](https://img.shields.io/badge/AI_Agents-9333EA?style=for-the-badge)

### Messaging & Event Systems
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Amazon SQS](https://img.shields.io/badge/Amazon_SQS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Amazon SNS](https://img.shields.io/badge/Amazon_SNS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)

### Cloud & DevOps
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)
![Amazon EC2](https://img.shields.io/badge/Amazon_EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![API Gateway](https://img.shields.io/badge/API_Gateway-FF4F8B?style=for-the-badge&logo=amazonaws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

### Databases
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

### Testing & Developer Tools
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 🎯 What I'm Focused On

- **AI Engineering:** Building practical LLM-powered features, RAG systems, and tool-using AI agents.
- **Agentic Workflows:** Connecting LLMs with APIs, business logic, and asynchronous backend operations.
- **Backend Architecture:** Designing modular services and maintainable Node.js/NestJS applications.
- **Distributed Systems:** Understanding messaging guarantees, consistency, retries, and fault tolerance.
- **Data & Performance:** Improving database access patterns, caching, and query performance.
- **Cloud Infrastructure:** Building reliable event-driven and serverless systems on AWS.

---

## 📫 Let's Connect

<div align="center">

| Platform | Link |
|---|---|
| 💼 LinkedIn | [Arjun Patidar](https://www.linkedin.com/in/arjun-patidar-6556b2226) |
| 📧 Email | [arjunjagotra2001@gmail.com](mailto:arjunjagotra2001@gmail.com) |
| 🐙 GitHub | [github.com/arjun808](https://github.com/arjun808) |

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1f2937,50:161b22,100:0d1117&height=100&section=footer" width="100%"/>

*Building reliable backend systems and useful AI-powered products.*

</div>
