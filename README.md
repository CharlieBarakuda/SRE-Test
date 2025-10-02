# webapp-k8s
Kubernetes manifests for a highly-available web app (nginx demo): Namespace, Service, Ingress, PDB, Deployment, HPA.

## Apply order
```bash
kubectl apply -f k8s/namespace.yaml
kubectl apply -f k8s/service.yaml
kubectl apply -f k8s/ingress.yaml
kubectl apply -f k8s/deployment.yaml
