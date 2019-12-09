# kubernetes commands 

###list pods
kubectl get pods

###list services
kubectl get services

###deploy demo files
kubectl create -f voting-app-pod.yml
kubectl create -f voting-app-service.yml

kubectl create -f redis-pod.yml
kubectl create -f redis-service.yml

kubectl create -f postgres-pod.yml
kubectl create -f postgres-service.yml

kubectl create -f worker-app-pod.yml

kubectl create -f result-app-pod.yml
kubectl create -f result-app-service.yml


###execute all files in folder
kubectl create -f .

###lists all pods, services, deployments and replica sets
kubectl get all

###apply changes to running cluster
kubectl apply -f voting-app-deployment.yml
