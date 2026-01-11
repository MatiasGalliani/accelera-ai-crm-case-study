# Accelera CRM: Enterprise AI-Powered Lead & Document Management System

> Production-grade CRM processing 5,000+ monthly leads with OpenAI-driven automation, achieving 80% operational cost reduction and 300% ROI in the Italian financial services sector.

![Stack](https://img.shields.io/badge/Stack-React%20%7C%20Node.js%20%7C%20PostgreSQL-blue)
![AI](https://img.shields.io/badge/AI-GPT--4%20Vision%20%7C%20RAG-green)
![Cloud](https://img.shields.io/badge/Cloud-GCP%20%7C%20Docker-orange)

---

## 🎯 Executive Summary

**Business Context:**
Creditplan Italia, a credit mediation firm, faced critical operational bottlenecks. Manual data entry from physical documents took 40+ hours weekly, with a 15-20% error rate and response times of up to 5 days.

**The Solution:**
I architected and deployed a full-stack AI-powered CRM from scratch. This system automates the entire lead-to-loan workflow through intelligent document processing, smart lead distribution, and conversational AI assistance.

**Quantified Business Impact:**
* **80% reduction** in operational overhead (from 40h to 8h weekly).
* **316% ROI** achieved within the first year.
* **90% accuracy** in automated document validation (Italian ID, CUD, Payslips).
* **94% faster** lead response time (from days to <2 hours).
* **65% reduction** in support tickets via RAG chatbot.

---

## 🏗️ Technical Architecture

The system is built on a robust, scalable architecture designed for high-availability and security:

* **Frontend:** React 18 (Vite), Tailwind CSS, shadcn/ui, and React Query for server state.
* **Backend:** Node.js (Express.js) with a layered service architecture and 50+ RESTful endpoints.
* **Database:** PostgreSQL with Sequelize ORM, utilizing JSONB for flexible document metadata.
* **AI Layer:** GPT-4o for reasoning, GPT-4 Vision for OCR, and RAG for intelligent search.
* **Infrastructure:** Google Cloud Storage (GCS) with Signed URLs, Dockerized microservices, and Railway deployment.

---

## 🛠️ Key Technical Innovations

### 1. AI-Powered Document Validation
I implemented a pipeline that extracts and validates data from 12+ types of Italian financial documents. By using document-specific prompt engineering and GPT-4 Vision, the system achieves 90% accuracy, far surpassing human baseline error rates.

### 2. Intelligent Round Robin Distribution
To manage 5,000+ monthly leads, I engineered a persistent Round Robin algorithm in PostgreSQL. This ensures fair, real-time distribution among 20+ agents based on source permissions, with atomic transactions to prevent race conditions.

### 3. RAG-Based Assistant ("Eugenio")
A conversational AI that enables agents to query the document database using natural language. It uses a dual-model strategy (gpt-4o-mini for intent analysis and GPT-4 for response) to minimize latency (<1.2s) and reduce API costs by 60%.

---

## 🔐 Security & Compliance
* **Encryption:** AES-256 at rest and TLS 1.3 in transit.
* **Signed URLs:** Documents are never public; access is granted via GCS Signed URLs with 60-minute expiration.
* **GDPR:** Fully compliant with data minimization, right to erasure, and audit logging.

---

## 📈 Scalability & Future
The system currently maintains **99.9% uptime** and is designed to scale 10x (50,000 leads/month) with current infrastructure through horizontal scaling and connection pooling (PgBouncer).

---

## 💼 Business Value
This project demonstrates how AI-driven automation directly impacts the bottom line, turning a cost center into a high-efficiency revenue engine. It represents 12 months of production-grade engineering and product ownership.

**Full Case Study:** [Download the Technical PDF](./Accelera_CRM_Enterprise_AI_Case_Study.pdf)

---

### 📞 Contact
**Matías Galliani**
* **Email:** matiasgalliani00@gmail.com
* **LinkedIn:** [linkedin.com/in/matias-galliani](https://linkedin.com/in/matias-galliani)
* **Location:** Argentina (Remote) | **Languages:** English (C1), Italian (B2), Spanish (Native)
