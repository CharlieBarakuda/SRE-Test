# webapp-k8s
Kubernetes manifests for a highly-available web app (nginx demo): Namespace, Service, Ingress, PDB, Deployment, HPA.

## Apply order
```bash
kubectl apply -f namespace.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml
kubectl apply -f deployment.yaml

# To open http://localhost:8080
kubectl -n webapp-prod port-forward deploy/app 8080:80

