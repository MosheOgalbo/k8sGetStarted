## install
choco install minikube

## check install
minikube start --driver docker
kubectl config current-context
minikube status
kubectl get node
kubectl get all
kubectl version

## apply ymls

kubectl apply -f .\mongo-config.yaml
kubectl apply -f .\mongo-secret.yaml
kubectl apply -f .\mongo.yaml
kubectl apply -f .\webapp.yaml

## check node
kubectl get all
kubectl get all
kubectl get configmap
kubectl get secret
kubectl describe service webapp-service
kubectl describe pod pod/webapp-deployment-dcffd6bcc-pplhr
kubectl describe pod webapp-deployment-dcffd6bcc-pplhr
kubectl get all
kubectl get pod
kubectl logs webapp-deployment-dcffd6bcc-pplhr
kubectl get svc
minikube ip

## goto browser
minikube service webapp-service

## show dashboard
minikube dashboard
