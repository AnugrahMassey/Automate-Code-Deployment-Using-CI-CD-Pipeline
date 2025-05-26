# DevOps Task 1: CI/CD Pipeline Automation

## **Objective**: Automate deployment of a Node.js app using GitHub Actions and Docker.

---

## 🛠️ Tech Stack
- **CI/CD**: GitHub Actions
- **Runtime**: Node.js
- **Containerization**: Docker
- **Registry**: Docker Hub

---

## 📂 Project Structure

├── .github/workflows/main.yml     # CI/CD config                                                                                   
├── Dockerfile                     # Docker setup                                                                                   
├── index.js                       # Node.js app                                                                                   
├── package.json                   # Dependencies                                                                                   
└── README.md                      # This file                                                                                   


---

## ⚙️ CI/CD Pipeline
**Trigger**: Push to `main` branch  
**Stages**:
1. **Build & Test**
   - Node.js setup
   - Dependency installation
   - Test execution (`npm test`)
2. **Docker Deployment**
   - Build Docker image
   - Push to Docker Hub with tags:
     - `latest`
     - Git commit SHA

---

## 🚀 Quick Start
1. Clone repo:
   ```bash
   https://github.com/AnugrahMassey/Automate-Code-Deployment-Using-CI-CD-Pipeline.git
Run locally:

```bash
npm install && npm start
```
## Access http://localhost:3000
Docker build:
```bash
docker build -t nodejs-demo-app . && docker run -p 3000:3000 nodejs-demo-app
```

## 🔑 Configuration
GitHub Secrets:

DOCKERHUB_USERNAME: Docker Hub username

DOCKERHUB_TOKEN: Docker Hub access token

Files:

-index.js: Simple Express server

-Dockerfile: Multi-stage build configuration

---

## 🤝 Contributing
Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request
---
