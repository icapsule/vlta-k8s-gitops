# 🐙 VLTA Kubernetes GitOps Repository

This is the Single Source of Truth (SSOT) GitOps repository monitored by ArgoCD.

## Topology
- `manifests/00-namespace.yaml`: Namespace definition (`vlta-dev`)
- `manifests/10-deployment.yaml`: Production-hardened Python FastAPI deployment (2 replicas, Anti-Affinity, Probes, preStop)
- `manifests/20-service.yaml`: LoadBalancer Service
- `manifests/30-ingress.yaml`: Ingress HTTP routing
