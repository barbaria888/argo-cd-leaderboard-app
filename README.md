# 🏆 Argo CD Leaderboard App

This repository demonstrates a **GitOps workflow using Argo CD and Helm** to deploy a sample **Leaderboard** microservice to Kubernetes.

It showcases how Argo CD applications are defined, configured per environment, and synced to a cluster using Helm value overrides.

---

## 📁 Repository Structure
📦 argo-cd-leaderboard-app/<br>
├── apps/<br>
│ ├── 🧪 leaderboard-dev.yaml &nbsp;&nbsp;# Argo CD App for Dev<br>
│ ├── 🔍 leaderboard-qa.yaml &nbsp;&nbsp;# Argo CD App for QA<br>
│ └── 🚀 leaderboard-prod.yaml &nbsp;&nbsp;# Argo CD App for Prod<br>
│<br>
└── charts/<br>
&nbsp;&nbsp;&nbsp;└── leaderboard/<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 📄 Chart.yaml &nbsp;&nbsp;# Helm chart metadata<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧱 templates/ &nbsp;&nbsp;# K8s manifests<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ⚙️ values.yaml &nbsp;&nbsp;# Default values<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧩 values-dev.yaml &nbsp;&nbsp;# Dev overrides<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧩 values-qa.yaml &nbsp;&nbsp;# QA overrides<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── 🧩 values-prod.yaml &nbsp;&nbsp;# Prod overrides<br>
