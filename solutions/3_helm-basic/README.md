```
helm install dani-nginx oci://registry-1.docker.io/bitnamicharts/nginx -n dani
kubectl get service -n dani
curl http://4.182.0.241/ bzw. Browser
helm upgrade dani-nginx oci://registry-1.docker.io/bitnamicharts/nginx -n dani -f values.yaml
helm delete dani-nginx -n dani
```
