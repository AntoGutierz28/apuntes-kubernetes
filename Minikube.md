# MiniKube
## Requisitos 
- Docker
- 2 nucleos 
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
