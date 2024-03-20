```
kubectl apply -f service-loadbalancer.yaml -n dani
kubectl describe service -n dani dani-demo-app-ext
curl 98.67.251.200

watch kubectl top pod -n dani
kubectl apply -f deployment.yaml -n dani

kubectl apply -f configmap.yaml -n dani
kubectl apply -f secret.yaml -n dani
kubectl exec -it -n dani deployment/dani-demo-app -- bash

kubectl apply -f cronjob.yaml -n dani
kubectl get jobs -n dani
kubectl logs job/dani-demo-app-28505726 -n dani
```
