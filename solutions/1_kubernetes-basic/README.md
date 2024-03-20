```
kubectl cluster-info
kubectl create namespace dani
kubectl config set-context --current --namespace=dani
kubectl get deployments -n dani
kubectl apply -f deployment.yaml -n dani
kubectl logs -f -n dani deployment/dani-demo-app
kubectl exec -it -n dani deployment/dani-demo-app -- bash
kubectl apply -f service-clusterip.yaml -n dani
```
