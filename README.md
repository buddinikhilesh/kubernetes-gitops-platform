# kubernetes-gitops-platform

GitOps delivery platform using ArgoCD, Helm, and Kubernetes.
Implements blue-green and canary deployment strategies for production microservices.

## What this solves
- Fully automated GitOps delivery via ArgoCD
- Zero-downtime blue-green and canary deployments
- Self-healing Kubernetes workloads
- Multi-environment promotion (dev → staging → production)

## Structure

| Folder | What is inside |
|---|---|
| `argocd/` | ArgoCD application manifests |
| `charts/` | Helm charts for microservices |
| `deployments/blue-green/` | Blue-green deployment configs |
| `deployments/canary/` | Canary rollout configs |

## Prerequisites
- Kubernetes cluster running
- ArgoCD installed
- Helm >= 3.0

## Usage
```bash
git clone https://github.com/YOUR_USERNAME/kubernetes-gitops-platform
kubectl apply -f argocd/application.yaml
```

## Related resume projects
- Project LaunchPad — self-service CI/CD platform at Southwest Airlines
- Project CloudCore — Kubernetes containerisation of 500+ workloads
