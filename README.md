# 🚀 DevOps CI Pipeline Project (vProfile)1####

## 📌 Project Overview

This project demonstrates a complete CI pipeline using Jenkins, SonarQube, and Nexus on AWS EC2 instances.

The pipeline automates code build, testing, code quality analysis, and artifact storage.

---

## 🧱 Architecture

GitHub → Jenkins → SonarQube → Nexus

---

## ⚙️ Tools & Technologies

* AWS EC2
* Jenkins
* SonarQube
* Nexus Repository Manager
* Maven
* GitHub

---

## 🔄 Pipeline Workflow

1. Developer pushes code to GitHub
2. GitHub webhook triggers Jenkins pipeline
3. Jenkins builds the application using Maven
4. Unit tests are executed
5. Code quality is analyzed using SonarQube
6. Quality Gate validation is performed
7. Build artifact (.war) is uploaded to Nexus

---

## 📦 Artifact Storage

Artifacts are stored in Nexus repository:

* vprofile-release
* vprofile-snapshot

---

## 🔐 Key Features

* Automated CI pipeline
* Code quality enforcement
* Artifact versioning
* Integration with AWS infrastructure

---

## 🚀 Future Improvements

* Add CD pipeline (Deployment using Tomcat / Docker)
* Integrate Kubernetes
* Add monitoring (Prometheus & Grafana)

---

## 👨‍💻 Author

Rahul Guleria

