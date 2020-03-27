# Kubernetes command

To apply yaml

```shell script
kubectl apply -f client-deployment.yaml
kubectl apply -f client-node-port.yaml
```

To get list of active services

```shell script
kubectl get services
kubectl get deployments # list of deployments
kubectl get pods # list of pods 
```

Imperative command to update image

```shell script
kubectl set image deployment/client-deployment client=stephengrider/multi-client:v5
```
