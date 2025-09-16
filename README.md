# Go Web App - DevOps Project 🚀

This project is a **Go-based web application** (simple HTML frontend) that I fully **DevOps-ified** to demonstrate industry-standard CI/CD workflows and Kubernetes deployment.

---

## ⚡ Project Overview
- **App**: Go web app serving static HTML.
- **Containerization**: Multi-stage Docker build for minimal and secure image.
- **Orchestration**: Kubernetes deployment with Nginx Ingress Controller.
- **Packaging**: Helm chart for easy installation and management.
- **CI/CD**:
  - **CI**: GitHub Actions – automated build, test, and push of Docker images.
  - **CD**: ArgoCD – GitOps-based continuous deployment to Kubernetes.
- **Ingress**: Nginx Ingress Controller exposing the app via a domain.
- **Version Control**: Git + GitHub for code and pipelines.

---

## 🛠️ Tech Stack
- **GoLang** – application backend  
- **Docker** – containerization  
- **Kubernetes** – orchestration  
- **Helm** – package management  
- **GitHub Actions** – CI pipeline  
- **ArgoCD** – GitOps & CD  
- **Nginx Ingress Controller** – external access  

---

## 🚀 Deployment Workflow

1. **Developer commits code** → GitHub repo.  
2. **GitHub Actions CI**:  
   - Build & test Go app.  
   - Build Docker image.  
   - Push image to Docker Hub.  
3. **ArgoCD CD**:  
   - Watches GitHub repo for changes in Helm chart/K8s manifests.  
   - Syncs latest version to Kubernetes cluster.  
4. **Kubernetes**:  
   - App runs in pods.  
   - Exposed via Nginx Ingress Controller.  
