# Kubernetes 

![architecture Kubernetes](https://github.com/sanogotech/kubernetesStarter/blob/main/archikubernetes.png)


##  Docker  vs Kubernetes

![Docker vs Kubernetes](https://github.com/sanogotech/kubernetesStarter/blob/main/images/dokervskubernetes.jpg)
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

## Kubernetes

* What is k8s (Kubernetes)

k8s is a container orchestration system. It is used for container deployment and management. Its design is greatly impacted by Google’s internal system Borg.


A k8s cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node. [1]

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers and a cluster usually runs multiple nodes, providing fault tolerance and high availability. [1]

![Kubernetes ](https://github.com/sanogotech/kubernetesStarter/blob/main/kubernetesComponent.jpg)

* Control Plane Components

- API ServerThe API server talks to all the components in the k8s cluster. All the operations on pods are executed by talking to the API server.

- SchedulerThe scheduler watches the workloads on pods and assigns loads on newly created pods.

- Controller ManagerThe controller manager runs the controllers, including Node Controller, Job Controller, EndpointSlice Controller, and ServiceAccount Controller.

- etcd etcd is a key-value store used as Kubernetes' backing store for all cluster data.

* Nodes

- PodsA pod is a group of containers and is the smallest unit that k8s administers. Pods have a single IP address applied to every container within the pod.

- KubeletAn agent that runs on each node in the cluster. It ensures containers are running in a Pod. [1]

- Kube Proxykube-proxy is a network proxy that runs on each node in your cluster. It routes traffic coming into a node from the service. It forwards requests for work to the correct containers.

👉 Over to you: Do you know why Kubernetes is called “k8s”?

Reference [1]: kubernetes.io/docs/concepts/overview/components/

## kafka-docker-kubernetes
configuration for running kafka in docker and kubernetes

## Best practices for creating stateful applications
1. Create a separate namespace for databases.
2. Place all the needed components for stateful applications, such as ConfigMaps, Secrets, and Services, in the particular namespace.
3. Put your custom scripts in the ConfigMaps.
4. Use headless service instead of load balancer service while creating Service objects.
5. Use the HashiCorp Vault for storing your Secrets.
6. Use the persistent volume storage for storing the data. Then your data won’t be deleted even if the Pod dies or crashes.
