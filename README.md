# Matome Mbowene

Software Engineer based in Johannesburg, South Africa.

I build backend systems, AI systems, data pipelines, distributed software, and cloud automation. My flagship open-source project is **Fairflow**: a production-oriented commerce platform built with TypeScript, Rust, React, Hono, Supabase/PostgreSQL, Paystack, Cloudflare R2, OpenAPI, ADRs, Docker, and CI.

**Focus:** Backend Engineering · AI Systems · Data Engineering · Distributed Systems · Cloud Engineering · Automation

**BSc Computer Science & Computer Engineering, University of Cape Town**

[Portfolio](https://matomembowene.co.za) · [Email](mailto:matomepontso@gmail.com) · [GitHub](https://github.com/MatomeMb) · [LinkedIn](https://linkedin.com/in/matomembowene)

## About

I work on systems where correctness matters at the boundary: APIs that validate before they mutate state, data pipelines that reject bad records before storage, and AI workflows that expose evidence instead of hiding uncertainty.

My recent work spans Python, Java, TypeScript, SQL, and Rust across backend services, applied AI, cloud infrastructure, and data-intensive applications. I prefer explicit trust boundaries, maintainable schemas, reproducible environments, and documentation that makes a system easier to operate, review, and extend.

Fairflow is the centre of that work: a public codebase that combines application architecture, API design, security controls, documentation, testing, and developer tooling in one repository.

## Experience

| Role | Period | Engineering outcome |
| --- | --- | --- |
| **Fairflow — Software Engineer / CTO** | **2025 — Present** | Building validation-first backend services in Python and TypeScript; shipped OCR document automation, grounded retrieval workflows, and a production-oriented open-source platform with public architecture, API, security, and operations documentation. |
| **Science Learning Centre, University of Cape Town — Systems Developer** | **Feb 2025 — Nov 2025** | Built **MyAdvisor**, a scheduling system with relational constraints and allocation scoring; measured a **35% improvement in tutor-allocation efficiency** and automated validated administrative imports. |
| **Google Cloud Career Launchpad — Cloud Engineering Track** | **2024** | Completed hands-on work across compute, storage, VPC networking, IAM, and managed data services. |
| **Dell Young Leaders — Leadership Development Programme** | **2022 — 2025** | Completed structured professional development alongside the engineering degree. |
| **EY Uncovered — Technology Consulting Insight Programme** | **2023** | Gained exposure to requirement gathering, delivery discipline, and governance around enterprise systems. |
| **University of Cape Town — BSc Computer Science & Computer Engineering** | **2020 — 2025** | Built across algorithms, operating systems, embedded systems, networking, machine learning, and distributed systems. |

## Fairflow

**Fairflow** is my flagship open-source engineering project.

It is a monorepo commerce platform with a React merchant/admin portal, a Hono API, a Rust core for portable product artifacts, Supabase/PostgreSQL for data and auth, Cloudflare R2 for storage, Paystack for payments, and a browser extension for product resolution.

### What the codebase includes

- **Architecture:** `auth-portal`, `shadow-index`, `matter-core`, `matter-ffi`, and `lens-extension` in one repository.
- **Authentication:** merchant JWT flows, Supabase staff auth, Google OAuth, and an admin proxy to keep privileged secrets server-side.
- **Payments and KYC:** Paystack checkout and webhook handling, plus Sumsub integration for merchant verification.
- **Storage:** PostgreSQL via Supabase, Cloudflare R2 in production, and local JSON storage for low-friction development.
- **Rust core:** `matter-core` compiles and validates portable `.thing` artifacts.
- **API:** OpenAPI-backed HTTP surface for auth, catalog, checkout, webhooks, analytics, compile, and resolve flows.
- **Documentation:** architecture notes, API reference, authentication guide, deployment docs, security docs, roadmap, and ADRs.
- **Testing:** Vitest for unit and integration coverage, Playwright for end-to-end coverage, and smoke verification workflows.
- **CI/CD:** GitHub Actions for linting, type-checking, tests, builds, and post-deploy smoke validation.
- **Docker:** Dockerfiles per package and a local `docker-compose.yml` stack.
- **Security:** security policy, PBKDF2 password hashing, webhook signature verification, rate limiting, and documented secret-handling practices.
- **Developer experience:** env templates, local-first setup, contribution docs, CODEOWNERS, PR templates, Dependabot, and conventional commit guidance.

### Fairflow links

| Resource | Link |
| --- | --- |
| Repository | [MatomeMb/FairFlow](https://github.com/MatomeMb/FairFlow) |
| Website | [fairflow.co.za](https://fairflow.co.za) · [fairflow-nine.vercel.app](https://fairflow-nine.vercel.app) |
| Case study | [Portfolio case study](https://matomembowene.co.za/#/project/fairflow) |
| Documentation | [Repository docs](https://github.com/MatomeMb/FairFlow/tree/main/docs) |
| OpenAPI | [`packages/shadow-index/openapi.yaml`](https://github.com/MatomeMb/FairFlow/blob/main/packages/shadow-index/openapi.yaml) |
| ADRs | [`docs/adr`](https://github.com/MatomeMb/FairFlow/tree/main/docs/adr) |
| Security | [`SECURITY.md`](https://github.com/MatomeMb/FairFlow/blob/main/SECURITY.md) |
| Contributing | [`CONTRIBUTING.md`](https://github.com/MatomeMb/FairFlow/blob/main/CONTRIBUTING.md) |

## Featured Projects

| Project | Problem | Solution | Technologies | GitHub / case study | Impact |
| --- | --- | --- | --- | --- | --- |
| **Fairflow** | Merchant operations, checkout, KYC, payouts, and product artifacts are usually fragmented across tools. | Built a public monorepo platform with a React portal, Hono API, Rust core, Supabase/PostgreSQL, R2 storage, and production documentation. | TypeScript, React, Hono, Node.js, Supabase, PostgreSQL, Paystack, Sumsub, Rust, Docker | [GitHub](https://github.com/MatomeMb/FairFlow) · [Case study](https://matomembowene.co.za/#/project/fairflow) | Production-oriented OSS covering architecture, auth, payments, docs, testing, CI, and DX in one codebase. |
| **OCR Document Automation** | OCR errors on financial documents can produce plausible but incorrect ledger values. | Built a staged pipeline with OpenCV preprocessing, coordinate segmentation, extraction, and four-layer validation before storage. | Python, OpenCV, Tesseract, Pandas, PostgreSQL | Private · [Case study](https://matomembowene.co.za/#/project/ocr-document-automation) | Eliminated silent OCR character-swap errors before they could reach downstream ledgers. |
| **RAG Knowledge Assistant** | Retrieval systems fail when weak evidence reaches generation and the model fills in the gap. | Built a grounded assistant with deterministic indexing, FAISS retrieval, conservative similarity gating, and explicit refusal paths. | Python, FAISS, Sentence Transformers, Streamlit, LLM APIs | [GitHub](https://github.com/MatomeMb/personal-codex-agent) · [Case study](https://matomembowene.co.za/#/project/rag-assistant) | Answers with citations when evidence is present and refuses when the corpus does not support the question. |
| **MyAdvisor** | Tutor allocation at the Science Learning Centre depended on manual coordination and was prone to collisions. | Built a scheduling system with relational invariants, role-based workflows, automated imports, and an allocation scoring routine. | Java, Spring Boot, PostgreSQL, SQL | Private · [Case study](https://matomembowene.co.za/#/project/myadvisor) | Measured **35% improvement** in tutor-allocation efficiency. |
| **FashionMNIST Neural Network** | Coursework results needed to be reproducible and honestly evaluated, not just visually impressive. | Built a reproducible training and evaluation pipeline with structured metrics and controlled experimentation. | Python, PyTorch, NumPy, Matplotlib | [GitHub](https://github.com/MatomeMb/FashionMNIST-Classifier) · [Case study](https://matomembowene.co.za/#/project/fashionmnist-classifier) | Achieved **89.33%** test accuracy with a reproducible evaluation pipeline. |
| **Peer-to-Peer Network** | File transfer without a central server introduces peer churn, integrity, and concurrency problems. | Built a socket-based peer protocol with chunk hashing, resumable transfer logic, and integrity checks. | Java, TCP sockets, threads, SHA-256 | Private · [Case study](https://matomembowene.co.za/#/project/p2p-network) | Delivered verifiable file transfer under partial failure and peer churn. |
| **STM32 Embedded Systems** | Bare-metal systems must operate within hard timing and memory constraints. | Built interrupt-driven firmware with register-level configuration, fixed memory usage, and bounded ISR work. | C, STM32, UART, timers, GPIO | Private · [Case study](https://matomembowene.co.za/#/project/stm32-embedded) | Produced deterministic firmware that remained inspectable and debuggable at the hardware boundary. |

## Open Source

I maintain open-source code the same way I would maintain an internal production repository.

- **Fairflow** is public because the engineering artefacts matter: architecture decisions, OpenAPI contracts, deployment notes, security guidance, and contributor workflows are part of the project, not afterthoughts.
- **Code quality** is enforced through linting, type-checking, tests, PR templates, and conventional commit rules.
- **Documentation standards** are explicit: API changes should update the OpenAPI spec, design changes should be reflected in docs or ADRs, and operational concerns belong in runbooks or deployment guides.
- **Contribution process** is documented in the repository through `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, GitHub templates, and CI expectations.
- **Engineering philosophy:** open source should be runnable, reviewable, and safe to extend. I prefer production-oriented OSS over decorative repositories.

## Engineering Principles

- **Maintainability:** keep route handlers thin, model invariants clearly, and make the next change easier than the last.
- **Observability:** structured logs, auditable workflows, and visible failure modes beat silent success assumptions.
- **Testing:** test contracts, edge cases, and failure paths, not just happy-path UI behavior.
- **Security:** separate trust boundaries, keep secrets off the client, verify signatures, and document incident-safe defaults.
- **Developer experience:** low-friction local setup, reproducible environments, and clear contribution guidance matter.
- **Documentation:** architecture, API, deployment, and operational context should live with the code.
- **Reliability:** reject bad input early, make invalid states hard to represent, and design for partial failure.

## Tech Stack

- **Languages:** Python, Java, TypeScript, SQL, C/C++, Rust, Bash
- **Backend:** Hono, Spring Boot, Node.js, FastAPI, REST API design, webhooks
- **Frontend:** React, Vite, Tailwind CSS, Thymeleaf, Streamlit
- **AI:** PyTorch, FAISS, Sentence Transformers, OpenCV, Tesseract, RAG pipelines, LLM APIs
- **Cloud:** Google Cloud, Supabase, Cloudflare R2, Vercel
- **Infrastructure:** Docker, Docker Compose, Linux, Nginx
- **Data:** ETL pipelines, schema design, validation-first ingestion, vector indexing, OCR workflows
- **DevOps:** GitHub Actions, CI/CD, dependency management, smoke testing
- **Databases:** PostgreSQL, MySQL
- **Developer Tools:** Git, Postman, Jira, VS Code

![Core stack](https://skillicons.dev/icons?i=python,java,ts,nodejs,react,spring,postgres,mysql,docker,gcp,rust,linux,githubactions&perline=13)

## Technical Writing

| Topic | Link |
| --- | --- |
| Building Fairflow | [Fairflow case study](https://matomembowene.co.za/#/project/fairflow) |
| REST API Design | [Engineering notes](https://matomembowene.co.za/#/writing) — includes *REST API design with Spring Boot: contracts before controllers* |
| RAG Systems | [RAG case study](https://matomembowene.co.za/#/project/rag-assistant) · [Engineering notes](https://matomembowene.co.za/#/writing) |
| OCR Pipelines | [OCR case study](https://matomembowene.co.za/#/project/ocr-document-automation) · [Engineering notes](https://matomembowene.co.za/#/writing) |
| Distributed Systems | [P2P case study](https://matomembowene.co.za/#/project/p2p-network) · [Engineering notes](https://matomembowene.co.za/#/writing) |
| SQL Optimisation | [Engineering notes](https://matomembowene.co.za/#/writing) — includes *Optimising SQL queries* |
| Spring Boot Architecture | [MyAdvisor case study](https://matomembowene.co.za/#/project/myadvisor) · [Engineering notes](https://matomembowene.co.za/#/writing) |
| Docker | [Engineering notes](https://matomembowene.co.za/#/writing) — includes *Docker in production* |

## GitHub

### Selected repositories

- [**FairFlow**](https://github.com/MatomeMb/FairFlow) — flagship open-source commerce platform.
- [**personal-codex-agent**](https://github.com/MatomeMb/personal-codex-agent) — grounded RAG assistant built on FAISS and sentence embeddings.
- [**FashionMNIST-Classifier**](https://github.com/MatomeMb/FashionMNIST-Classifier) — reproducible machine learning coursework pipeline.
- [**Connected-Components-Image-Processor**](https://github.com/MatomeMb/Connected-Components-Image-Processor) — C++ image-processing work focused on connected-component analysis.

![GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=MatomeMb&theme=github-compact&hide_border=true&bg_color=0d1117&color=9ca3af&line=2563eb&point=ffffff)

![Contribution Snake](https://raw.githubusercontent.com/MatomeMb/MatomeMb/output/github-contribution-grid-snake.svg)

![Profile Views](https://komarev.com/ghpvc/?username=MatomeMb&style=flat-square&color=2563eb)

## Contact

- **Email:** [matomepontso@gmail.com](mailto:matomepontso@gmail.com)
- **Portfolio:** [matomembowene.co.za](https://matomembowene.co.za)
- **LinkedIn:** [linkedin.com/in/matomembowene](https://linkedin.com/in/matomembowene)
- **GitHub:** [github.com/MatomeMb](https://github.com/MatomeMb)
