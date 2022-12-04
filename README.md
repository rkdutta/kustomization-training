# kustomization-training


## create the namespaces
```
kubectl apply -f namespaces.yaml
```

### create all tenants at once
```
kubectl apply -k tenants/
```

### create one tenant at a time
```
kubectl apply -k tenants/dev/sample-app-1
kubectl apply -k tenants/acc/sample-app-1
kubectl apply -k tenants/prod/sample-app-1
```