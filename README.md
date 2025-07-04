<h3>DEMO:</h3>
<p><a href='https://crypto-coins-tracker.vercel.app/'>crypto-coins-tracker</a></p>
# crypto-tracker-v2

**Crypto Tracker** is a React-based web application that displays real-time cryptocurrency prices using the [CoinGecko API](https://www.coingecko.com/en/api). The app is fully containerized and deployed to Azure Kubernetes Service (AKS) following GitOps practices via ArgoCD.

## 🚀 Features

- Live cryptocurrency price updates
- Responsive React UI
- CoinGecko API integration
- Docker containerization
- CI/CD with GitHub Actions
- GitOps deployment via ArgoCD
- Hosted on AKS (Azure Kubernetes Service)

## 🛠️ Tech Stack

- **Frontend**: React.js  
- **API**: CoinGecko  
- **Containerization**: Docker  
- **CI/CD**: GitHub Actions  
- **Image Registry**: Azure Container Registry (ACR)  
- **Orchestration**: Azure Kubernetes Service (AKS)  
- **Deployment**: ArgoCD  

## 🌐 Live Demo

[🔗 View Live App](crypto-coins-tracker.vercel.app) 

## ⚙️ Environment Variables

If needed, create a `.env` file in the root directory and set the following (optional):


# 📦 Getting Started (Local Setup)

## Clone the repo
git clone https://github.com/<your-username>/crypto-tracker.git
cd crypto-tracker

## Install dependencies
npm install

## Run the development server
npm start

# 🐳 Docker Build & Run
## Build the Docker image
docker build -t crypto-tracker .

## Run the container
docker run -p 3000:3000 crypto-tracker

# ☸️ Kubernetes Deployment
Ensure you have kubectl configured and a running cluster (e.g., AKS).
# Apply all Kubernetes manifests
kubectl apply -f k8s/

# 🔁 CI/CD Workflow
GitHub Actions runs on push:

Builds Docker image

Pushes to Azure Container Registry (ACR)

ArgoCD watches the Git repo

Changes are auto-deployed to AKS via GitOps

