# `kubectl apply -f k8-postgres.yaml`

### check psql
```kubectl get pods```


```
kubectl exec -it postgres-7b4b876d74-cf4jk -- psql -h localhost -U ps_user --password -p 5432 ps_db
```

`SecurePassword`

### Deploy
```
kubectl apply -f postgres-configmap.yaml
```

### Verify
```
kubectl get configmap
```

```
kubectl apply -f psql-pv.yaml
```

```
kubectl apply -f psql-claim.yaml
```

```
kubectl apply -f ps-deployment.yaml
```


### 
```kubectl get pv```

### 
```kubectl get pvc```

###
```kubectl apply -f ps-service.yaml```

### 
```kubectl get svc```



### check psql
```kubectl get pods```


```
kubectl exec -it postgres-7b4b876d74-cf4jk -- psql -h localhost -U ps_user --password -p 5432 ps_db
```


```minikube service nginx-deployment --url```
```minikube service postgres --url```
```minikube service nginx --url```