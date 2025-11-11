# 🏆 Argo CD Leaderboard App

This repository demonstrates a **GitOps workflow using Argo CD and Helm** to deploy a sample **Leaderboard** microservice to Kubernetes.

It showcases how Argo CD applications are defined, configured per environment, and synced to a cluster using Helm value overrides.

---

## 📁 Repository Structure
📦 argo-cd-leaderboard-app/
├── apps/
│   ├── 🧪 leaderboard-dev.yaml     # Argo CD App for Dev
│   ├── 🔍 leaderboard-qa.yaml      # Argo CD App for QA
│   └── 🚀 leaderboard-prod.yaml    # Argo CD App for Prod
│
└── charts/
    └── leaderboard/
        ├── 📄 Chart.yaml           # Helm chart metadata
        ├── 🧱 templates/           # K8s manifests
        ├── ⚙️ values.yaml          # Default values
        ├── 🧩 values-dev.yaml      # Dev overrides
        ├── 🧩 values-qa.yaml       # QA overrides
        └── 🧩 values-prod.yaml     # Prod overrides
