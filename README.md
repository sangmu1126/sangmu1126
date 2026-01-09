# 👋 Hi, I'm LEE SANGMU

### **Systems Architect & Performance Engineer** 🐧
*> "I don't just use the cloud; I engineer the underlying systems."*

<div align="center">
  <br />
  
  <a href="mailto:sangmu1126@gmail.com">
    <img src="https://img.shields.io/badge/Email-sangmu1126%40gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://sooming99.notion.site/Sangmu-Lee-13432d2f56c4808197f9c5e951edbca0?pvs=74">
    <img src="https://img.shields.io/badge/Portfolio-Notion-000000?style=flat-square&logo=notion&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://github.com/sangmu1126">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" />
  </a>

  <br />
  <br />

  Systems Engineer passionate about diving deep into **OS kernels (Cgroups)** and optimizing distributed systems.  
  Specialized in building **High-Performance Infrastructure** on AWS using **Terraform** and **Docker**.

</div>

---

## 🚀 Technical Arsenal

| Domain | Technolgies |
| :--- | :--- |
| **Core Systems** | ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) |
| **Cloud & IaC** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white) |
| **Backend** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) |
| **Data & Search** | ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![ElasticSearch](https://img.shields.io/badge/ElasticSearch-005571?style=flat-square&logo=elasticsearch&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |

---

## 🌟 Featured Projects

### 1️⃣ [Infra-FaaS: Custom Serverless Engine](https://github.com/sangmu1126/Infra-controller)
**Building a High-Performance FaaS Platform from Scratch (on EC2 & Docker)**
> *"Why accept the Cold Start latency of managed services when you can engineer it away?"*

Designed and implemented a proprietary Serverless Engine to overcome the limitations of AWS Lambda (Cold Start & Monitoring).
- **Core Engine**: Built a custom orchestrator replacing Kubelet, managing container lifecycles via direct Docker Socket control.
- **Zero Cold Start**: Engineered a **"Heavy Warm Pool"** architecture, reducing function wakeup time by **95% (sub-100ms)**.
- **Kernel-Level Tuning**: Developed a **Smart Auto-Tuner** leveraging **Linux Cgroup v2** metrics (memory.peak, cpu.stat) to optimize resource allocation automatically.
- **Event-Driven Scaling**: Implemented a **SQS Backlog-based** autoscaler using Terraform ASG policies to handle burst traffic reliable.

### 2️⃣ [NewJeanse: AI Energy Management](https://github.com/sangmu1126/NewJeanse)
**Large-scale Power Data Analysis & AI Model Serving**
> *Backend Lead & Data Engineer*

- **Pipeline Optimization**: Refactored Airflow ETL workflows, reducing daily data processing time by **60%**.
- **Real-time Serving**: Wrapped heavy ML models with **FastAPI** for low-latency inference, ensuring high availability for end-users.

### 3️⃣ [EveryTown: Location Search Engine](https://github.com/sangmu1126/EveryTown)
**Elasticsearch-based GEO Search Platform**
> *Backend Developer*

- **Search Performance**: Migrated complex RDB queries to **Elasticsearch**, boosting search speed from **2.0s to 0.2s (10x)** using inverted indexes.
- **DevOps**: Standardized the entire development lifecycle using **Docker Compose**, reducing onboarding time for new team members.

### 4️⃣ [Mingle: Global EdTech Platform](https://github.com/sangmu1126/MingleGDSC)
**Google Solution Challenge 2024 - Global Top 100**
> *Backend Architecture & Cloud Deployment*

- **Global Scalability**: Designed a scalable backend usage Firebase & Cloud Functions to support users worldwide.
- **Recognition**: Selected as a Top 100 project globally, recognized for technical execution and social impact.

---

<div align="center">
  <sub>Designed & Engineered by Sangmu Lee</sub>
</div>
