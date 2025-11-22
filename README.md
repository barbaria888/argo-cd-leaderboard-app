# <h2> <img src="https://argo-cd.readthedocs.io/en/stable/assets/argo.png" alt="Argo CD" width="28"/> Argo CD Leaderboard App</h2> Argo CD Leaderboard App

This repository demonstrates a **GitOps workflow using Argo CD and Helm** to deploy a sample **Leaderboard** microservice to Kubernetes.

It showcases how Argo CD applications are defined, configured per environment, and synced to a cluster using Helm value overrides.
<br>HOW did I deploy it over ArgoUI see blog-> 
<a href="https://kubernetes-project.hashnode.dev/deploying-a-multi-environment-application-with-argo-cdand-helm-a-complete-gitopsguide"><?xml version="1.0" encoding="UTF-8"?>
<svg width="256px" height="256px" viewBox="0 0 256 256" xmlns="http://www.w3.org/2000/svg">
  <g fill-rule="evenodd">
    <path d="M17.5913461,85.5328619 C-5.86378203,108.98799 -5.86378203,147.01185 17.5913461,170.464766 L85.5337714,238.409404 C108.9889,261.862319 147.01276,261.862319 170.465675,238.409404 L238.410313,170.464766 C261.863229,147.009638 261.863229,108.985777 238.410313,85.5328619 L170.465675,17.5904365 C147.010547,-5.86247884 108.986687,-5.86247884 85.5337714,17.5904365 L17.5913461,85.5328619 Z M157.724673,157.725976 C174.143262,141.307386 174.143262,114.690241 157.724673,98.2738645 C141.308296,81.8552748 114.691151,81.8552748 98.274774,98.2738645 C81.8561843,114.692454 81.8561843,141.307386 98.274774,157.725976 C114.693364,174.142353 141.308296,174.142353 157.726886,157.725976 L157.724673,157.725976 Z" fill="#2962FF"/>
  </g>
</svg>

</a>
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

