# 🧠 gitlabby  
*CI/CD playground built for learning, testing, and leveling up DevOps workflows.*

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

# ✅ gitlabby Pipeline & Quality Checks

[![Pipeline Status](https://img.shields.io/badge/pipeline-passed-brightgreen?style=for-the-badge&logo=gitlab)](http://localhost/root/gitlabby/-/pipelines)
[![Quality Gate](https://img.shields.io/badge/quality--gate-passed-brightgreen?style=for-the-badge&logo=sonarqube)](http://localhost:9000/dashboard?id=gitlabby)







A secure CI/CD lab project integrating GitLab, Docker, and SonarQube.


---

## 🖇️ Architecture Flow

```mermaid
flowchart TD
    subgraph DevEnv[Local Dev Environment]
        A[Developer 🧑‍💻] -->|Push Code| B[GitLab 🦊]
    end

    subgraph GitLabCI[GitLab CI/CD Pipeline]
        B -->|Triggers| C[GitLab Runner 🏃‍♂️]
        C -->|Runs Jobs| D[Docker 🐳]
        D -->|Executes sonar-scanner| E[SonarQube 🔍]
    end

    subgraph Sonar[SonarQube Server]
        E -->|Saves Results| F[(Quality Gate ✅ / ❌)]
    end

    F -->|Feedback| B
