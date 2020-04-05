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

# Kubernetes Dashboard

Configuration is at [kubernetes-dashboard.yaml](http://127.0.0.1:8001/api/v1/namespaces/kube-system/services/https:kubernetes-dashboard:/proxy/#!/overview?namespace=default) 
from https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/

Open web page http://127.0.0.1:8001/api/v1/namespaces/kube-system/services/https:kubernetes-dashboard:/proxy/#!/overview?namespace=default to view it.
