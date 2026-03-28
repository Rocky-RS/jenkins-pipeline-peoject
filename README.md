# 🚀 DevOps CI/CD Pipeline Project (vProfile)

## 📌 Project Overview

This project demonstrates a **complete end-to-end CI/CD pipeline** using Jenkins, Docker, AWS ECR, and ECS.

It automates the process of **building, testing, analyzing, containerizing, and deploying applications** into a production environment.

---

## 🧱 Architecture

GitHub → Jenkins → SonarQube → Nexus → Docker → AWS ECR → AWS ECS

---

## ⚙️ Tools & Technologies

* AWS (EC2, ECR, ECS)
* Jenkins
* SonarQube
* Nexus Repository Manager
* Docker
* Maven
* Git & GitHub

---

## 🌿 Branch Strategy

* `develop` → CI Pipeline (Build, Test, Analysis)
* `main` → CD Pipeline (Production Deployment)

---

## 🔄 CI Pipeline Workflow (Develop Branch)

1. Developer pushes code to `develop` branch
2. GitHub webhook triggers Jenkins CI pipeline
3. Jenkins builds the application using Maven
4. Unit tests are executed
5. SonarQube performs code quality analysis
6. Quality Gate validation is checked
7. Artifact (.war) is uploaded to Nexus
8. Docker image is built from the application
9. Docker image is pushed to AWS ECR

---

## 🚀 CD Pipeline Workflow (Main Branch)

1. Code is merged from `develop` to `main`
2. Push to `main` triggers Jenkins CD pipeline
3. Jenkins pulls Docker image from ECR
4. ECS service is updated with new task definition
5. Application is deployed automatically to AWS ECS

---

## 📦 Artifact & Image Storage

### Nexus Repository

* vprofile-release
* vprofile-snapshot

### AWS ECR

* Stores Docker images for deployment

---

## ☁️ Deployment (AWS ECS)

* ECS Cluster for staging and production
* Task Definitions for container configuration
* Services for running containers
* Optional Load Balancer integration

---

## 🔐 Key Features

* End-to-End CI/CD automation
* Branch-based deployment strategy
* Code quality enforcement (SonarQube)
* Artifact management (Nexus)
* Containerization using Docker
* Cloud deployment using AWS ECS
* Scalable and production-ready pipeline

---

## 🧹 Cleanup & Cost Optimization

* ECS services and clusters removed after testing
* ECR repositories cleaned to avoid storage costs
* EC2 instances terminated
* Load balancers and target groups removed
* Task definitions deregistered

---

## 🚀 Future Improvements

* Kubernetes (EKS) deployment
* Blue-Green / Canary deployments
* Monitoring with Prometheus & Grafana
* CI/CD with GitHub Actions
* Infrastructure as Code (Terraform)

---

## 👨‍💻 Author

**Rahul Guleria**

