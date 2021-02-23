# kubernetes commands 

### version info
```
kubectl version
```

### cluster information
```
kubectl cluster-info
```
### list nodes
```
kubectl get nodes
```

### list nodes with extended infos
```
kubectl get nodes -o wide
```

### list pods
```
kubectl get pods
```

### pod details
```
kubectl describe pods [name]
```


### list services
```
kubectl get services
```

### list replication controllers
```
kubectl get replicationcontroller
```

### list replicasets
```
kubectl get replicaset
```

### list deployments
```
kubectl get deployments
```

### scale replicaset to new value
```
kubectl scale --replicas=[new value] replicaset-definition.yml
```

### scale replicaset with type/name syntax
```
kubectl scale --replicas=[new value] replicaset [name of rs]
```


### update replicaset with new file
```
kubectl replace -f replicaset-definition.yml
```



### deploy demo files
```
kubectl create -f voting-app-pod.yml
kubectl create -f voting-app-service.yml

kubectl create -f redis-pod.yml
kubectl create -f redis-service.yml

kubectl create -f postgres-pod.yml
kubectl create -f postgres-service.yml

kubectl create -f worker-app-pod.yml

kubectl create -f result-app-pod.yml
kubectl create -f result-app-service.yml
```
-f : File Option
--record : Records change cause. Records commmand that created/changes item 

### execute all files in folder
```
kubectl create -f .
```
### lists all pods, services, deployments and replica sets
```
kubectl get all
```
### apply changes to running cluster
```
kubectl apply -f voting-app-deployment.yml
```

### Rollout Status
```
kubectl rollout status deployment/[name of deployment]
```

### Rollout Status
```
kubectl rollout status deployment[name of deployment]
```

### Rollback 
```
kubectl rollout undo deployment[name of deployment]
```

### Deployment Strategies
- Recreate (drop all - recreate all)
- Rolling Update (default strategy)


