# 🏆 Argo CD Leaderboard App

This repository demonstrates a **GitOps workflow using Argo CD and Helm** to deploy a sample **Leaderboard** microservice to Kubernetes.

It showcases how Argo CD applications are defined, configured per environment, and synced to a cluster using Helm value overrides.

---

## 📁 Repository Structure

├── apps/
│ ├── leaderboard-dev.yaml # Argo CD Application manifest for dev environment
│ ├── leaderboard-qa.yaml # Argo CD Application manifest for QA environment
│ └── (more environments can be added here)
│
└── charts/
└── leaderboard/
├── Chart.yaml # Helm chart metadata
├── templates/ # Kubernetes manifests (Deployment, Service, etc.)
├── values.yaml # Default Helm values
├── values-dev.yaml # Overrides for dev
├── values-qa.yaml # Overrides for QA
└── values-prod.yaml # Overrides for production
