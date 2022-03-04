# Microk8s
## requisitos minimos
- Docker
- 514 MB de RAM
- 20 GB hard disk 
## Instalacion
```
sudo snap install microk8s --classic
```
## Listado de comandos 
```
microk8s
```
## Iniciar cluster
```
microk8s.start
```
## Estado de cluster
```
microk8s.status
```
## Habilitar dns
```
microk8s.enable dns
```
## Habilitar ingress
```
microk8s.enable ingress
```
## Habilitar istio
```
microk8s.enable istio
```
## Habilitar DNS
```
microk8s.enable dns
```
## Habilitar metricas
```
microk8s.enable metrics-server
```
## Habilitar almacenamiento
```
microk8s.enable storage
```
## Habilitar registry
```
microk8s.enable registry
```
## Listar namespaces
```
microk8s.kubectl get namespaces
```
## Listar pods
```
microk8s.kubectl get pods
```
## Listar nodos
```
microk8s.kubectl get nodes
```
## Listar servicios
```
microk8s.kubectl get services
``` 
## Visualizar dashboard
```
microk8s.dashboard-proxy
```