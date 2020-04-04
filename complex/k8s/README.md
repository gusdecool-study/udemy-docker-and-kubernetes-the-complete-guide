## Create Secret

It must be created with imperative command to be safe

```shell script
kubectl create secret [type] [secret name] --from-literal [key=value]
kubectl create secret generic pgpassword --from-literal PG_PASSWORD=root_password
```
