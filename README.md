# 🚀 DevOps Project: Automated CI/CD Pipeline for a 2-Tier Flask Application on AWS

## 👨‍💻 Author

**Jatin Shant**
DevOps Engineer | AWS | Docker | Jenkins | Kubernetes | CI/CD Enthusiast

---

## 📌 Project Overview

This project demonstrates a complete **DevOps CI/CD pipeline** implementation for a **2-tier Flask + MySQL application** deployed on **AWS EC2** using:

* Jenkins
* Docker
* Docker Compose
* GitHub Webhooks
* AWS EC2

The pipeline automatically builds and deploys the application whenever code is pushed to GitHub, enabling fully automated deployments.

---

# 🏗️ Architecture

```text
Developer → GitHub → Jenkins → Docker Build → Docker Compose Deployment → Flask + MySQL Application
```

---

# ⚙️ Tech Stack

| Technology      | Purpose                    |
| --------------- | -------------------------- |
| AWS EC2         | Cloud Infrastructure       |
| Jenkins         | CI/CD Automation           |
| Docker          | Containerization           |
| Docker Compose  | Multi-container Deployment |
| GitHub          | Version Control            |
| GitHub Webhooks | Automatic Pipeline Trigger |
| Flask           | Backend Application        |
| MySQL           | Database                   |
| Ubuntu 22.04    | Operating System           |

---

# ☁️ AWS EC2 Setup

* Ubuntu 22.04 LTS
* t2.micro Instance
* Security Groups:

  * Port 22 → SSH
  * Port 8080 → Jenkins
  * Port 3000 → Flask Application

---

# 🔧 Installed Components

* OpenJDK 17/21
* Jenkins
* Docker Engine
* Docker Compose
* Git
* Swap Memory Configuration

---

# 🐳 Dockerized Application

The application contains:

## Flask Application Container

* Python Flask backend
* Exposed on port 5000

## MySQL Container

* MySQL 8 Database
* Persistent Docker Volume

---

# 🔄 CI/CD Pipeline Workflow

## Jenkins Pipeline Stages

### 1️⃣ Clone Repository

Jenkins pulls the latest code from GitHub.

### 2️⃣ Build Docker Image

Docker Compose builds application containers.

### 3️⃣ Deploy Application

Containers are recreated automatically using Docker Compose.

### 4️⃣ Automated Trigger

GitHub Webhooks automatically trigger Jenkins after every push.

---

# 📂 Important Files

## Dockerfile

Used to containerize the Flask application.

## docker-compose.yml

Defines multi-container setup for:

* Flask App
* MySQL Database

## Jenkinsfile

Pipeline-as-code configuration for CI/CD automation.

---

# 🚀 Deployment Process

```bash
git push origin main
        ↓
GitHub Webhook Trigger
        ↓
Jenkins Pipeline Execution
        ↓
Docker Image Build
        ↓
Container Deployment
        ↓
Application Live on AWS
```

---

# 📊 Infrastructure Diagram

(Add your architecture image here)

---

# 🌟 Key Learnings

* Setting up Jenkins CI/CD pipelines
* Docker containerization
* Multi-container orchestration using Docker Compose
* AWS EC2 infrastructure management
* GitHub Webhook integration
* Pipeline automation using Jenkinsfile
* DevOps deployment workflow implementation

---

# 📌 Features

✅ Automated CI/CD Pipeline
✅ Dockerized Application
✅ Multi-tier Architecture
✅ GitHub Webhook Integration
✅ AWS Cloud Deployment
✅ Jenkins Automation
✅ Infrastructure as Code Approach

---

# 🔗 Access URLs

## Jenkins Dashboard

```text
http://<EC2-PUBLIC-IP>:8080
```

## Flask Application

```text
http://<EC2-PUBLIC-IP>:3000
```

---

# 📚 Future Improvements

* Kubernetes Deployment
* Terraform Automation
* Monitoring with Prometheus & Grafana
* Nginx Reverse Proxy
* SSL Configuration using Let's Encrypt
* GitHub Actions Integration

---

# 🧑‍💻 About Me

Hi, I'm **Jatin Shant**, a DevOps Engineer passionate about:

* Cloud Infrastructure
* CI/CD Automation
* Docker & Kubernetes
* AWS & Linux
* Infrastructure Automation

---

# 📌 Tags

`DevOps` `AWS` `Docker` `Jenkins` `CI/CD` `Flask` `MySQL` `GitHub` `Automation` `Docker Compose` `Cloud Computing`
