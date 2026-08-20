# 🏄‍♂️ Sachin Bashetti

**`Evolving DevOps Engineer | Networking Roots → Cloud & DevOps`**

I'm DevOps-focused engineer with a strong networking foundation, building hands-on experience around **CI/CD automation, containerization, Kubernetes, GitOps, observability, infrastructure as code, and cloud-native platforms**.

I focus on understanding systems end-to-end — from source code and container images to Kubernetes workloads, networking, deployment automation, monitoring, and troubleshooting.

Rather than collecting tools, I prefer building and operating projects that demonstrate **how different DevOps components work together in a real engineering workflow**.

---

## 🔧 Skills & Tools

### 🧩 DevOps & Cloud

- **CI/CD:** GitHub Actions, Jenkins
- **Containers:** Docker, Docker Compose, Multi-Stage Builds, Image Optimization
- **Orchestration:** Kubernetes
  - Deployments
  - Services
  - Ingress
  - ConfigMaps
  - Secrets
  - Persistent Volumes
  - Namespaces
  - Health Probes
  - Resource Requests & Limits
  - HPA
- **Packaging:** Helm
- **GitOps:** Argo CD, Git as Source of Truth
- **Infrastructure as Code:** Terraform
- **Cloud:** AWS fundamentals, EKS roadmap
- **Monitoring:** Prometheus, Grafana

### 🖥️ Systems & Networking

- Linux Administration & Troubleshooting
- Networking Fundamentals
- DNS, Ports & Services
- Bash Scripting & Automation
- Process & Service Management
- Infrastructure Troubleshooting
- Root Cause Analysis

---

# 🚀 Featured Project

## ☁️ CloudCart Platform

**Production-Style Cloud-Native Microservices Platform**

CloudCart is a production-inspired cloud-native platform built to demonstrate an end-to-end **DevOps engineering workflow**.

The project covers the complete journey from application containerization to Kubernetes orchestration, CI/CD automation, GitOps deployment, observability, and infrastructure automation.

### 🏗️ Current Architecture

```text
                         Developer
                             │
                         Git Push
                             │
                             ▼
                     GitHub Repository
                             │
                             ▼
                    GitHub Actions (CI)
                             │
                    ┌────────┴────────┐
                    │                 │
              Build Images        Run Tests
                    │                 │
                    ▼                 │
                Docker Hub            │
                    │                 │
                    └────────┬────────┘
                             ▼
                     Helm Values Update
                             │
                             ▼
                          Argo CD
                         (GitOps)
                             │
                             ▼
                    Kubernetes Cluster
                             │
                  ┌──────────┴──────────┐
                  │                     │
             NGINX Ingress          PostgreSQL
                  │
                  ▼
             React Frontend
                  │
          ┌───────┼────────┐
          │       │        │
          ▼       ▼        ▼
        Auth   Product   Payment
       Service  Service   Service
````

### 🧩 Application Components

* **React Frontend**
* **FastAPI Auth Service**
* **FastAPI Product Service**
* **FastAPI Payment Service**
* **PostgreSQL**

The architecture intentionally focuses on three backend services:

* **Auth Service** — authentication and user-related functionality
* **Product Service** — product/catalog management and APIs
* **Payment Service** — payment-related functionality

---

## 🛠️ CloudCart Technology Stack

### Application

* React
* FastAPI
* PostgreSQL

### Containerization

* Docker
* Docker Compose
* Docker Hub
* Multi-stage builds
* Image optimization

### Orchestration

* Kubernetes
* Minikube
* Helm
* NGINX Ingress Controller

### CI/CD & GitOps

* GitHub Actions
* Argo CD
* GitOps
* Git as Source of Truth
* Git commit SHA image tagging

### Observability

* Prometheus
* Grafana
* Application metrics
* Kubernetes metrics
* Alerting configuration

### Infrastructure

* Terraform
* AWS
* Amazon EKS

---

# ✅ What I've Implemented in CloudCart

### 🐳 Containerization

* Containerized frontend and backend services
* Multi-stage frontend Docker build
* Optimized backend container images
* Docker Compose development environment
* Service-specific Dockerfiles

### ☸️ Kubernetes

Implemented Kubernetes resources including:

* Deployments
* Services
* ConfigMaps
* Secrets
* Persistent Volume Claims
* Namespaces
* Health probes
* Resource requests and limits
* NGINX Ingress
* Horizontal Pod Autoscaler

### ⛵ Helm

Built a Helm chart providing:

* Parameterized Kubernetes resources
* Environment-specific values
* Configurable image tags
* Configurable replicas
* Configurable ingress
* Configurable HPA

### 🔄 GitHub Actions

Implemented CI automation for:

* Docker image builds
* Docker Hub image pushes
* Git commit SHA-based image tagging
* Helm image tag updates
* Automated Git commits

### 🔁 GitOps with Argo CD

Implemented GitOps-based Kubernetes deployment using:

```text
GitHub
   │
   ▼
GitHub Actions
   │
   ▼
Docker Image
   │
   ▼
Helm Values Update
   │
   ▼
Git Repository
   │
   ▼
Argo CD
   │
   ▼
Kubernetes
```

Git is treated as the source of truth for the desired application state.

### 🧪 Automated Testing

Implemented Product Service API testing using:

* pytest
* FastAPI TestClient
* PostgreSQL test database

Current tests cover:

* Product creation
* Product listing
* Product retrieval
* Brand filtering
* Featured filtering
* Product update
* Product deletion
* Not-found handling
* Invalid payload validation

---

# 🎬 Next Major Feature — CloudCart Showcase Mode

After the platform verification phase, CloudCart will include a dedicated **Showcase Mode**.

Showcase Mode is not intended to create another marketplace experience.

Its purpose is to demonstrate the engineering work behind CloudCart.

The frontend will be able to switch into a presentation-oriented mode using a keyboard shortcut.

The planned showcase will explain and visualize:

* CloudCart architecture
* Microservices
* Docker containers
* Kubernetes workloads
* Helm deployment
* GitHub Actions CI pipeline
* Argo CD
* GitOps workflow
* NGINX Ingress
* Prometheus
* Grafana
* HPA
* Deployment flow
* Infrastructure architecture
* DevOps engineering decisions

The goal is to make the project itself **demonstrate the DevOps work that built it**.

---

# 📈 Roadmap

### Phase 1 — Platform Verification

* [x] Microservices architecture
* [x] Docker
* [x] Docker Compose
* [x] Product Service API tests
* [ ] Validate Kubernetes manifests
* [ ] Validate Helm deployment
* [ ] Validate Argo CD synchronization
* [ ] Validate NGINX Ingress
* [ ] Validate Prometheus
* [ ] Validate Grafana
* [ ] Validate HPA
* [ ] Complete end-to-end deployment testing

### Phase 2 — Showcase Mode

* [ ] Frontend keyboard shortcut
* [ ] Architecture visualization
* [ ] DevOps workflow visualization
* [ ] Kubernetes / Helm / GitOps explanation
* [ ] Monitoring overview
* [ ] Infrastructure overview
* [ ] Deployment pipeline visualization

### Phase 3 — Infrastructure

* [ ] Terraform
* [ ] AWS VPC
* [ ] Amazon EKS
* [ ] Remote Terraform State
* [ ] Production-style AWS infrastructure

### Phase 4 — Security

* [ ] Trivy image scanning
* [ ] Kubernetes RBAC
* [ ] Network Policies
* [ ] Improved Secret Management
* [ ] Container security hardening

### Phase 5 — Advanced Observability

* [ ] Alertmanager
* [ ] Loki
* [ ] OpenTelemetry
* [ ] Distributed Tracing
* [ ] Application Performance Monitoring

---

# 📖 Currently Learning

* Advanced Kubernetes operations
* Kubernetes troubleshooting
* AWS container infrastructure
* Terraform and infrastructure as code
* Prometheus and Grafana
* CI/CD architecture
* GitOps workflows
* Linux and Bash automation
* Production-style incident analysis and root cause analysis

---

# 🌱 How I Work

* Build first, then refine
* Prefer understanding over memorization
* Focus on root causes rather than commands
* Automate repetitive workflows
* Keep Git as the source of truth
* Introduce technologies only when they provide meaningful value
* Build incrementally instead of trying to create everything at once
* Document systems so they can be explained and reproduced

---

# 🎯 Current Goal

My goal is to transition into a **DevOps Engineering role** by demonstrating practical experience with:

* Kubernetes
* Docker
* CI/CD
* GitOps
* Helm
* Infrastructure as Code
* AWS
* Observability
* Linux
* Automation
* Production-style troubleshooting

CloudCart is my primary hands-on project for bringing these concepts together into one complete engineering workflow.

Long-term, I want to work on **cloud-native platforms, infrastructure automation, and reliable production systems**.

---

## 📌 Project Philosophy

> **Don't just deploy an application. Understand and automate everything around it.**

CloudCart is continuously evolving as a practical DevOps engineering project, with each phase focused on adding meaningful engineering capability rather than simply adding more technologies.
