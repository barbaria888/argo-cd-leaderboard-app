# 🏆 Argo CD Leaderboard App

This repository demonstrates a **GitOps workflow using Argo CD and Helm** to deploy a sample **Leaderboard** microservice to Kubernetes.

It showcases how Argo CD applications are defined, configured per environment, and synced to a cluster using Helm value overrides.

---

## 📁 Repository Structure
📦 <b>argo-cd-leaderboard-app/</b><br>
├── <b>apps/</b><br>
│ ├── 🧪 <b>leaderboard-dev.yaml</b> — Argo CD Application for <i>Dev</i><br>
│ ├── 🔍 <b>leaderboard-qa.yaml</b> — Argo CD Application for <i>QA</i><br>
│ └── 🚀 <b>leaderboard-prod.yaml</b> — Argo CD Application for <i>Production</i><br>
│<br>
└── <b>charts/</b><br>
&nbsp;&nbsp;&nbsp;└── <b>leaderboard/</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 📄 <b>Chart.yaml</b> — Helm chart metadata<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧱 <b>templates/</b> — Kubernetes manifests (Deployment, Service, etc.)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ⚙️ <b>values.yaml</b> — Default Helm values<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧩 <b>values-dev.yaml</b> — Overrides for Dev<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── 🧩 <b>values-qa.yaml</b> — Overrides for QA<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── 🧩 <b>values-prod.yaml</b> — Overrides for Production<br>

