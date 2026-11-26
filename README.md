<div align="center">

<img src="https://avatars.githubusercontent.com/u/119033939?v=4" width="112" alt="Fufa Wakgari" />

# Fufa Wakgari

### Backend & Full-Stack Engineer · NestJS · PostgreSQL · TypeScript

Building production APIs, authorization boundaries, and relational data models for **fintech**, **B2B marketplaces**, and **multi-tenant SaaS**.

**Addis Ababa, Ethiopia (EAT / UTC+3) · Open to backend roles, contracts & remote teams**

[Portfolio](https://fufawakgari.vercel.app) &nbsp;·&nbsp;
[Engineering Notes](https://fufawakgari.vercel.app/insights) &nbsp;·&nbsp;
[Resume (PDF)](https://fufawakgari.vercel.app/Fufa_Wakgari_Resume.pdf) &nbsp;·&nbsp;
[LinkedIn](https://www.linkedin.com/in/fufa-wakgari-85b412228/) &nbsp;·&nbsp;
[Email](mailto:fufawakgari174@gmail.com)

<br />

<img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js" />

</div>

---

## Behind the APIs

I'm a Backend & Full-Stack Engineer (and Assistant Lecturer in Software Engineering at **Haramaya University**) focused on turning complex domain rules into reliable, testable services.

Most of my production NestJS work lives inside private employer repositories, so I document system architecture, trade-offs, and failure modes openly through **[case studies](https://fufawakgari.vercel.app/#projects)**, **[engineering notes](https://fufawakgari.vercel.app/insights)**, and **[public reference implementations](https://github.com/fufex3934/nestjs-fintech-marketplace-api)**.

---

## Public Code & Reference Architecture

| Repository | Focus | Highlights |
| --- | --- | --- |
| [**`nestjs-fintech-marketplace-api`**](https://github.com/fufex3934/nestjs-fintech-marketplace-api) | **NestJS + PostgreSQL + Prisma** reference backend | JWT refresh rotation + reuse detection, RBAC + IDOR scoping, `Idempotency-Key` transactions, tiered RFQ matching (max 8 vendors), Swagger `/docs`, Docker Compose, Jest + Supertest specs |
| [**`frontend` (Harar Gov CMS)**](https://github.com/fufex3934/frontend) | **MERN** production CMS (`hararicommunication.gov.et`) | Sole engineer; separated public read API from JWT-gated editorial workflows used by 5 non-technical staff (100+ published articles) |

---

## Production Systems & Selected Work

### [7Net B2B Marketplace ↗](https://7netmarket.com/) · [Case Study + Deep Dive →](https://fufawakgari.vercel.app/projects/7net-b2b-marketplace)
**Backend Developer (Remote) · `NestJS · PostgreSQL · Prisma · TypeScript`**
- Built catalog (`500+` SKUs), cart, and custom sourcing (RFQ quotation) APIs supporting `1,000+` buyers and `50+` verified industrial suppliers.
- Solved vendor notification spam via tiered category/verification matching capped at **8 vendors per RFQ** with **48h auto-expiry**, stabilizing quotes at **3–5 responses per request**.

### [Seed Finance Platform ↗](https://seed-finance-web.vercel.app/en) · [Case Study + Deep Dive →](https://fufawakgari.vercel.app/projects/seed-finance-platform)
**Backend Developer (Remote) · `NestJS · PostgreSQL · Prisma · JWT · RBAC`**
- Owned `AuthModule`, `UsersModule`, and `TransactionsModule` (`~20` production REST endpoints) backing multi-role financial workflows.
- Enforced JWT access/refresh lifecycle, `ValidationPipe` DTO whitelisting, route-level `RolesGuard`, and service-level IDOR scoping across admin, operator, and end-user roles.

### [RSMS – School Management System ↗](https://rsms.rammisbank.et:8080/) · [Case Study + Deep Dive →](https://fufawakgari.vercel.app/projects/rsms-school-management-system)
**Sole Full-Stack Developer · `Laravel · Inertia.js · MySQL` (Pilot — `400+` Student Records)**
- Built 6 core domains end-to-end (enrollment, grading, attendance, fees, 4-role RBAC) with **bank-integrated fee payment** and idempotent transaction reconciliation (`UNIQUE(bank_reference)` + `lockForUpdate()`).

### [Harar Government Communication CMS ↗](https://hararicommunication.gov.et/) · [Case Study →](https://fufawakgari.vercel.app/projects/harari-government-communication-platform)
**Sole Full-Stack Developer · `React · Node.js · Express · MongoDB` (Production `.gov.et`)**
- Delivered the official regional communication portal and admin publishing dashboard, enabling 5 staff editors to publish 100+ articles independently.

> *Proprietary employer codebases remain private. Full architecture diagrams, schema designs, and sanitized code samples are documented on each case study page.*

---

## Client Feedback

> *"Fufa was great to work with. He quickly understood the NestJS REST API issues, communicated clearly throughout the project, and delivered the fixes as expected. He was professional, responsive, and focused on getting the job done properly. I would be happy to work with him again on future backend development projects."*
>
> — **Upwork Client Review (`5.0 / 5.0`)** · *Fix NestJS REST API Bug* · Clear Communicator · Committed to Quality · Detail & Solution Oriented

---

## Engineering Focus & Approach

- **Authorization & Security First:** JWT + refresh token rotation, declarative RBAC guards, strict DTO validation, and service-level resource scoping so business rules never leak to the client.
- **Data & Payment Integrity:** Relational constraints, database transactions, `Idempotency-Key` replay safety, retry recovery, and clean reconciliation trails.
- **Performance & Real-Time:** Redis caching, indexed SQL queries, pagination envelopes, WebSockets, and event-driven workflows.
- **Verification & Maintainability:** Unit + HTTP contract tests (`Jest` / `Vitest` / `Supertest`), OpenAPI specs, Docker parity, and clear documentation for teammates.

## Technical Toolkit

| Focus | Technologies |
| --- | --- |
| **Backend & APIs** | Node.js, NestJS, Express, TypeScript, REST, OpenAPI / Swagger, WebSockets |
| **PHP Ecosystem** | PHP, Laravel, Inertia.js |
| **Databases & Caching** | PostgreSQL, Prisma, MySQL, MongoDB, Redis |
| **Security & Architecture** | JWT, RBAC, IDOR Scoping, Multi-Tenant Systems, Idempotent Webhooks |
| **Testing & DevOps** | Jest, Vitest, Supertest, Docker, GitHub Actions, Git, Postman |
| **Frontend Delivery** | Next.js, React, Tailwind CSS |

---

<div align="center">

### Have a Backend Engineering Role or API Challenge?

**[Send an email](mailto:fufawakgari174@gmail.com)** &nbsp;·&nbsp;
**[Explore case studies](https://fufawakgari.vercel.app)** &nbsp;·&nbsp;
**[Read engineering notes](https://fufawakgari.vercel.app/insights)** &nbsp;·&nbsp;
**[Connect on LinkedIn](https://www.linkedin.com/in/fufa-wakgari-85b412228/)**

</div>
