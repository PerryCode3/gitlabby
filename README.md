# 🧠 gitlabby  
*A cozy CI/CD playground built for learning, testing, and leveling up DevOps workflows.*

---

## 🚀 Overview  
**gitlabby** is a local GitLab + Docker + SonarQube sandbox designed for hands-on DevOps practice.  
It’s where pipelines, scanners, and containers all come to hang out.

This project demonstrates:
- GitLab CI/CD automation
- Docker-based GitLab Runner
- Static code analysis with SonarQube
- Quality Gate enforcement for clean, secure builds

---

## 🧩 Pipeline Stages
| Stage | Description |
|-------|--------------|
| 🧱 **Build** | Prepare or compile source code (or container images). |
| 🧪 **Test** | Run validation or unit tests before deployment. |
| 🔍 **Analyze** | Scan code quality and security with SonarQube. |
| 🚢 **Deploy** | (Coming soon!) Deploy to containerized or cloud environments. |

---

## 📊 Quality & Metrics

[![Quality Gate](http://host.docker.internal:9000/api/project_badges/measure?project=gitlabby&metric=alert_status)](http://host.docker.internal:9000/dashboard?id=gitlabby)
[![Bugs](http://host.docker.internal:9000/api/project_badges/measure?project=gitlabby&metric=bugs)](http://host.docker.internal:9000/dashboard?id=gitlabby)
[![Vulnerabilities](http://host.docker.internal:9000/api/project_badges/measure?project=gitlabby&metric=vulnerabilities)](http://host.docker.internal:9000/dashboard?id=gitlabby)
[![Code Smells](http://host.docker.internal:9000/api/project_badges/measure?project=gitlabby&metric=code_smells)](http://host.docker.internal:9000/dashboard?id=gitlabby)

> **SonarQube Quality Gate:** Passing ✅ — Your code is clean, green, and mean.

---

## ⚙️ Getting Started

### 🐋 1. Run GitLab locally
```bash
docker-compose up -d gitlab
