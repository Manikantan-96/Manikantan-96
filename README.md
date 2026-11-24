## Deevanooru Manikantan

**Java Backend & Full-Stack Engineer** · Bengaluru, India  
Building secure REST APIs, concurrency-safe workflows, and distributed Spring Boot systems.

[![Portfolio](https://img.shields.io/badge/Portfolio-manikantan--portfolio.netlify.app-0F172A?style=flat-square&logo=vercel&logoColor=white)](https://manikantan-portfolio.netlify.app/)
[![Live App](https://img.shields.io/badge/Live_Demo-ExpenseFlow_SaaS-059669?style=flat-square&logo=netlify&logoColor=white)](https://expense-frontend.netlify.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/manikantan-deevanooru)
[![Email](https://img.shields.io/badge/Email-manikantandeevanooru%40gmail.com-DC2626?style=flat-square&logo=gmail&logoColor=white)](mailto:manikantandeevanooru@gmail.com)

---

### Quick Guide for Visitors

- **Recruiters & Hiring Managers:** Click **[ExpenseFlow Live Demo](https://expense-frontend.netlify.app)** and use the built-in **1-Click Persona Switcher** (`Employee` → `Manager` → `Finance Admin`) to test the full multi-stage approval app in 30 seconds — no signup required. Or browse architecture walkthroughs on my **[Portfolio](https://manikantan-portfolio.netlify.app/)**.
- **Engineers & Technical Leads:** Inspect the pinned repositories below for concurrency-safe JPQL locking, JPA `@Version` optimistic locking, rotating `HttpOnly` refresh cookies, Saga compensation state machines, Resilience4j patterns, and automated RestAssured / Mockito test suites.

---

### Selected Projects

| Project | What It Solves (Business View) | Key Backend Implementation | Links |
|---|---|---|---|
| **ExpenseFlow** | Automates workplace expense approvals from receipt upload through manager sign-off and finance payout without duplicate payments or cross-team data leaks. | Java 17 · Spring Boot 4.1 · Spring Security (`@PreAuthorize` + IDOR ownership checks) · Rotating SHA-256 `HttpOnly` refresh tokens · Atomic JPQL `@Modifying` lock (`409` on race) + `@Version` · 18 test suites (JUnit 5, Mockito, RestAssured) · Multi-stage Docker | [Code](https://github.com/Manikantan-96/Expense-Claim-Approval-System) · [Live App](https://expense-frontend.netlify.app) |
| **Sentinel** | Coordinates multi-step e-commerce orders (payment, stock reservation, email alerts) across separate services so partial failures automatically refund customers and restore stock. | 7 Spring Boot 4 / Spring Cloud services (Eureka, Config Server, WebFlux Gateway, OpenFeign) · Persistent `PAYMENT → INVENTORY → NOTIFICATION` Saga state machine · Resilience4j Circuit Breaker/Bulkhead/Retry · Redis rate limiting & caching · 4 MySQL DBs · Docker Compose | [Code](https://github.com/Manikantan-96/Sentinel-Distributed-Saga-Orchestrator-Microservices) · [Config](https://github.com/Manikantan-96/Config-server-for-sentinel) |
| **Food Delivery DB** | Models restaurant menus, orders, riders, and payments in MySQL for fast backend reporting and safe order stock updates. | Normalized schema (`ER_diagram.png`) · Stored procedures & transactions · Triggers · Composite indexes · Analytical views & SQL queries | [Code](https://github.com/Manikantan-96/Food-Delivery-Database) |

---

### Technical Stack

- **Backend:** Java 17 · Spring Boot 4 · Spring Web MVC · Spring Security · Spring Data JPA / Hibernate · Spring Cloud (Gateway, Eureka, Config, OpenFeign) · Resilience4j · REST APIs
- **Databases & Caching:** MySQL 8 · Redis 7 · H2
- **Security & API Contracts:** JWT (JJWT) · BCrypt · SHA-256 Refresh Token Rotation · Bean Validation · OpenAPI / Swagger UI
- **Testing:** JUnit 5 · Mockito · RestAssured · AssertJ · `@SpringBootTest` / `@DataJpaTest`
- **Frontend & Infrastructure:** React 19 · Axios · Tailwind CSS v4 · Vite · Docker · Docker Compose · Maven · Git
