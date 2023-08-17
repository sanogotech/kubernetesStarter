# Kubernetes 

* https://youtu.be/2vMEQ5zs1ko

  - Déploiement facile ( avec scalabilité et résidence au panneau redemarre seul)
    
  - Développemen de microservive ( service registre et loadbalnacing et api gateway)
 
  - Monitoring et log ( Graphana et prometheus)

Pas d'opposition entre Docker et Kubernetes car Kubernetes est un  orchestrateur de Containers.


## Différences en entre Virtual Macine et Docker

* https://youtu.be/a1M_thDTqmU
  
*** Virtual Machine

   - Vm1, Vm2, Vm3
   - Hyperviseur
   - Machine physique
ici on veux juste virtualiser la machine physique hardware

** Docker 

- Container1( instance imgage1),  Container 2
- Docker Engine
- OS
- Hardware ou Virtual Machine

  Docker est pour virtualiser OS uniquement et chaque image est isolé et est comme un mini Os linux


## REX Nelson DjaloNelson Djalo

🚀 Founder of Amigoscode | Helping millions of people break into Software Engineering and DevOps 🤝| 500K Community🚀 Founder of Amigoscode | Helping millions of people break into Software Engineering and DevOps 🤝| 500K Community


Kubernetes is a powerful container orchestration platform that has become increasingly popular in recent years.

However Monitoring a Kubernetes cluster can be a daunting task. With so many moving parts, it can be difficult to know where to start. But it's essential to get monitoring right, or you could be setting yourself up for failure.

🧨 One of the biggest challenges of Kubernetes monitoring is the dynamic nature of the platform. Pods are constantly being created, updated, and deleted. This means that your monitoring solution needs to be able to keep up with the changes.

🌐Another challenge is the distributed nature of Kubernetes. Metrics are collected from different parts of the cluster, and it can be difficult to get a unified view of the health of the system.

🎯But there are solutions to these challenges.

✅ Prometheus is a popular open-source monitoring system that is designed to be scalable, flexible, and easy to use.

It can collect metrics from all parts of the Kubernetes cluster, and it provides a unified view of the health of the system.

✅ Grafana is a popular open-source dashboarding solution that can be used to visualize Prometheus metrics.

 It allows you to create custom dashboards that track the health of your Kubernetes cluster.

🤝Together, Prometheus and Grafana can provide you with a comprehensive monitoring solution for your Kubernetes cluster. With the right monitoring in place, you can be confident that your cluster is healthy and running smoothly.

Let's have a quick look at some additional tips for Kubernetes monitoring:

✅ Use a service discovery tool to automatically discover your pods.

✅ Use a centralized logging solution to collect logs from all parts of your cluster.

✅ Set up alerts so that you are notified of any problems.

✅ Regularly review your monitoring data to identify trends and potential problems.

With these tips you can ensure that your Kubernetes cluster is properly monitored and that you are alerted to any problems as soon as they occur.
