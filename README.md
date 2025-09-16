DevOps Go Web App 🚀

A simple Go-based web application, fully DevOps-ified and production-ready with containerization, orchestration, CI/CD, and monitoring.

⚙️ Tech Stack

Go – simple HTML-based web app

Docker – multi-stage builds for lightweight, secure images

Kubernetes – app deployed and managed inside a cluster

Helm – packaging & deploying manifests

Nginx Ingress Controller – routing traffic inside the cluster

GitHub Actions – CI pipeline for building & pushing images

ArgoCD – GitOps-based CD pipeline for automated K8s deployments

AWS EKS – production-grade cluster setup and deployment

Minikube – local testing and cluster simulation

🚀 Features

Multi-stage Docker build for optimized image size

Helm charts for modular and reusable deployments

Ingress configured for clean routing

GitHub Actions CI pipeline integrated with DockerHub

ArgoCD for automated GitOps deployments

Works both locally (Minikube) and on cloud (EKS)

📦 Deployment

Local (Minikube):

minikube start
helm install go-web-app ./helm
minikube service list


AWS EKS:

eksctl create cluster --name go-web-cluster --region ap-south-1
helm install go-web-app ./helm
kubectl get svc


Access the app via the LoadBalancer or Ingress endpoint.