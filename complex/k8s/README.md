## Create Secret Service

It must be created with imperative command to be safe

```shell script
kubectl create secret [type] [secret name] --from-literal [key=value]
kubectl create secret generic pgpassword --from-literal PG_PASSWORD=root_password
```

## Kubernetes Nginx Ingress Controller

### Prerequisite Generic Deployment Command

```shell script
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.30.0/deploy/static/mandatory.yaml
kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.30.0/deploy/static/mandatory.yaml
```

### Provider Specific Steps - Docker

```shell script
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.30.0/deploy/static/provider/cloud-generic.yaml
kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.30.0/deploy/static/provider/cloud-generic.yaml
```
