# platform-config

Shared cluster add-ons for the k3d GitOps portfolio platform. Argo CD watches
this repo through an App-of-Apps rooted at `bootstrap/root-app.yaml`.

- `bootstrap/` — root Application (App-of-Apps)
- `apps/` — Argo CD Application manifests (namespaces, cloudflared, monitoring, status-page, warden)
- `manifests/` — raw k8s manifests (cloudflared, namespaces)
- `monitoring/` — pinned chart values

See the plan: [devops-portfolio-gitops-vps-plan.md](https://github.com/benzac708/bzdotfiles/blob/main/docs/plans/devops-portfolio-gitops-vps-plan.md)