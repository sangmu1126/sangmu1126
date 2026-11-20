# Sangmu Lee

**Backend & Cloud Infrastructure Engineer** · Seoul, South Korea

I build backend systems and cloud infrastructure with a focus on **reliability, performance, and resource efficiency**. I enjoy tracing problems to their root causes, validating changes through measurements, and documenting engineering decisions.

[**Portfolio**](https://sooming99.notion.site/Sangmu-Lee-13432d2f56c4808197f9c5e951edbca0?pvs=74) · [**Email**](mailto:sangmu1126@gmail.com) · [**GitHub**](https://github.com/sangmu1126)

## Technical Skills

| Area | Technologies |
| --- | --- |
| **Cloud & Infrastructure** | AWS, Kubernetes, Docker, Terraform, Helm, Packer, Linux |
| **Backend** | Python, Java, Node.js, FastAPI, Express.js, Spring Boot |
| **DevOps & Observability** | GitHub Actions, Prometheus, Grafana, k6 |
| **Databases & Messaging** | PostgreSQL, MySQL, MongoDB, Redis, Amazon SQS |
| **Frontend & Mobile** | HTML5, CSS3, JavaScript, TypeScript, React, Next.js, Flutter, Android |

## Featured Projects

### [FaaS Platform](https://github.com/sangmu1126/FaaS-Platform) · Custom Serverless Execution Platform

**AWS · EC2 · SQS · Docker · Redis · Terraform · Linux Cgroup v2**

Independently redesigned a hackathon project into an AWS-based platform for running user-uploaded functions inside Docker containers.

- Separated request handling from function execution with **Controller → SQS → Worker**, using Redis Pub/Sub for synchronous responses.
- Built reusable container warm pools and safeguards for process cleanup, execution-slot management, and user-code isolation.
- Provisioned the infrastructure with Terraform and Packer, and configured SQS backlog-based Worker Auto Scaling.
- **Validation:** Completed **181/181 synchronous function invocations** at 3 offered RPS over 60 seconds on one `t3.micro` Worker. Separately measured **445.57 accepted requests/s** on the Controller's private HTTP path; this is request admission, not function completion throughput.

[Documentation](https://github.com/sangmu1126/FaaS-Platform) · [Demo video](https://youtu.be/TyCFOvRkNCc)

### [PipeLens](https://github.com/sangmu1126/PipeLens) · Evidence-Based CI Failure Diagnosis

**FastAPI · PostgreSQL · Redis · GitHub App · OpenAI · Prometheus**

Developed a GitHub App that correlates failed GitHub Actions logs with code changes and workflow configuration to suggest verifiable diagnoses.

- Combined rule-based analysis with optional LLM diagnosis; checked evidence citations and file-level suggestions before publishing results.
- Implemented webhook verification, untrusted-fork isolation, sensitive-data redaction, and idempotent GitHub reporting.
- Designed failure recovery using Redis worker leases, heartbeats, **fencing tokens**, and database/queue reconciliation.
- **Validation:** Completed **3,605 jobs in a one-hour, four-worker synthetic soak test** on a single Docker host, with zero lost jobs or duplicate completions.

[Documentation](https://github.com/sangmu1126/PipeLens)

### [KubeFit](https://github.com/sangmu1126/Kubefit) · Kubernetes Resource Optimization

**Kubernetes · Prometheus · AWS EKS · Helm · k6 · Python · GitOps**

Built a tool to analyze Kubernetes workloads, recommend CPU and memory resource settings, validate changes, and open GitHub Draft PRs for human review.

- Correlated Deployment and Pod identities with metrics; derived recommendations from **CPU P95** and **memory P99** with safety margins.
- Compared baseline and candidate settings under fixed load and added CPU-throttling evidence to prevent misleading performance-only PASS decisions.
- Preserved human approval rather than automatically merging or deploying changes.
- **Validation:** Completed a **60-minute EKS pilot (100,503 requests; zero HTTP errors)** for metric collection and read-only recommendation. Actual AWS cost savings were **not** demonstrated.

[Documentation](https://github.com/sangmu1126/Kubefit) · [Demo video](https://youtu.be/HQRzH8ce2a4)

## Other Projects

| Project | Highlights |
| --- | --- |
| [EveryTown](https://github.com/sangmu1126/EveryTown) | Spring Boot and Elasticsearch location-based search platform. Reduced query latency from approximately **2 s to 200 ms** in historical local measurements. |
| [Mingle](https://github.com/sangmu1126/MingleGDSC) | Flutter and Firebase educational application; selected for the **Google Solution Challenge 2024 Global Top 100**. |
| [ElectricKo! / NewJeanse](https://github.com/sangmu1126/NewJeanse) | Led a five-member AI energy management project; worked on predictive modeling and backend APIs. |

## Experience & Activities

| Period | Activity |
| --- | --- |
| **Oct – Nov 2026** | **SoftBank Hackathon 2026** — Developed an AI-assisted AWS infrastructure provisioning and optimization platform in the preliminary round; contributed to security and observability for an AWS-to-on-premises migration platform in the final round. |
| **Aug 2026** | **Open Source Developer Contest 2026** — Submitted KubeFit, a Kubernetes resource optimization tool validated on AWS EKS. |
| **Jun – Jul 2026** | **AX 인재전쟁 2026** — Built an investment-assistance plugin for a KakaoPay Securities challenge. |
| **Nov – Dec 2025** | **SoftBank Hackathon 2025 in Korea** — Developed a web-app deployment platform in the preliminary round and an AWS serverless function execution platform in the final round. |
| **Sep 2025 – Apr 2026** | **Soldesk** — Completed an AWS-based Cloud DevOps training program. |
| **Mar – Nov 2024** | **K-Software Empowerment Bootcamp (KEB), Cohort 3** — Completed a university–industry software development training program. |
| **Aug 2023 – Aug 2024** | **Google Developer Student Clubs (GDSC)** — Participated in a university developer community. |
| **Sep 2021 – Aug 2025** | **Kaiwa, university Japanese language & culture club** — Served as Vice President in the first semester of 2022 and President in the second semester. |
| **Sep 2020 – Aug 2023** | **IGRUS** — Participated in a university IT, software development, and security club. |

## Honors & Awards

- **Dec 2025** — **Preliminary Round Excellence Award**, SoftBank Hackathon 2025 in Korea (advanced to the finals).
- **Apr 2024** — **Global Top 100**, Google Solution Challenge 2024 (Mingle).

## Education & Qualifications

- **Inha University** — B.S., Computer Science and Engineering (Mar 2020 – Aug 2025)
- **TOPCIT Level 3** — May 2024
- **TOEIC 755** — Jun 2025

---

*Measure carefully. Design for failure. Document what the evidence supports.*
