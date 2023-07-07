# Proyecto Práctico

## Infraestructura III
### Certified Tech Developer
### Digital House
### 2023

***

## Docker Images

1. Back

    `docker build -t alejamarin/getting-started-back .`

    `docker push alejamarin/getting-started-back`

2. Front

    `docker build -t alejamarin/gs-front .`

    `docker push alejamarin/gs-front`

## Host

<http://examen.dh/>

## Kubernetes

`kubectl create namespace getting-started`

`kubectl config set-context --current --namespace getting-started`

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.8.1/deploy/static/provider/cloud/deploy.yaml`

`kubectl apply -f mongo.yaml`

`kubectl apply -f back-deployment.yaml`

`kubectl apply -f back-service.yaml`

`kubectl apply -f front-deployment.yaml`

`kubectl apply -f front-service.yaml`

`kubectl apply -f ingress.yaml`

> Ejecuta todos los archivos
>
>> `kubectl apply -f .`

`kubectl get all`