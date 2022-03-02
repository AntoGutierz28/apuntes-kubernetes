# MiniKube
## Requisitos 
- Docker
- 2 nucleos CPU
- 2 GB de RAM
- 20 GB hard disk 

## Instalar en Linux
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
``` 

### Utilizar driver de docker
Utilizar driver de docker 
```
minikube start --driver=docker
``` 
Usar driver de docker por defecto
```
minikube config set driver docker
```

## Encender Minikube
```
minikube start
```
## Apagar Minikube
```
minikube stop
```
## Eliminar Minikube
```
minikube delete
```
## Inicializar Dashboard
```
minikube dashboard
```
## Instalar Kubectl
```
curl -LO https://dl.k8s.io/release/v1.23.0/bin/linux/amd64/kubectl
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
```
## Ejecutar un POD con un imagen
```
kubectl run anker --image=sotobotero/udemy-devops:0.0.1 --port=80 80
```
## Listado de PODs
```
kubectl get pod
``` 
## Informacion de POD
```
kubectl describe pod anker
```
## Crear servicio
```
kubectl expose pod anker --type=LoadBalancer --port=8080 --target-port=80
```
## Lista de servicio 
```
kubectl get services
```
## Informacion del servicio
```
kubectl describe services anker
```
## Exponer servicio 
```
minikube service anker --url
``` 