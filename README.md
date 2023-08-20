# kafka-docker-kubernetes
configuration for running kafka in docker and kubernetes

## Docker Engine,  Docker Image,  Containers,  Kubernetes 

Containers is instance running of Docker Image on Docker Engine .

Kubernetea: Containers Orchestration for nonfunctional features :
- Load balancer 
- Service registry
- Api manager
- supervision Graphana et prometheus
- autoscalling
- restart
- Failover

## Kubernetes en 6 minutes 

* https://youtu.be/TlHvYWVUZyc

## Best practices for creating stateful applications
1. Create a separate namespace for databases.
2. Place all the needed components for stateful applications, such as ConfigMaps, Secrets, and Services, in the particular namespace.
3. Put your custom scripts in the ConfigMaps.
4. Use headless service instead of load balancer service while creating Service objects.
5. Use the HashiCorp Vault for storing your Secrets.
6. Use the persistent volume storage for storing the data. Then your data won’t be deleted even if the Pod dies or crashes.
