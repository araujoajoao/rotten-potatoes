Criar o cluster Kubernetes com o seguinte comando:
```
k3d cluster create clusterconversao --agents 1 --servers 1 -p 8080:30000@loadbalancer
```