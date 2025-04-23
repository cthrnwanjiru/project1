# 🌐 Cloud-Native Flask App on AWS EKS

A minimal Flask app containerized with Docker, deployed to AWS EKS using Terraform and Kubernetes manifests.

## 🛠️ Stack
- Flask (Python)
- Docker
- Kubernetes (on AWS EKS)
- Terraform (for infrastructure)
- Linux shell scripting

## 📦 Features
- AWS infrastructure provisioning with Terraform
- Kubernetes deployment with `kubectl`
- Docker container for Flask app
- Shell script for automation

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/your-username/cloud-native-flask-app.git
cd cloud-native-flask-app

# Deploy infrastructure
cd terraform/
terraform init
terraform apply

# Build and push Docker image
docker build -t your-dockerhub-username/flask-app .
docker push your-dockerhub-username/flask-app

# Deploy to Kubernetes
kubectl apply -f k8s/

# Get the load balancer URL
kubectl get svc
