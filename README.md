**🚀 Kubernetes Project --- Hands-on Setup and Management with
Minikube**

This document is a walkthrough of my **Kubernetes project** where I
deploy a basic application stack using Minikube on Ubuntu 24.04. Each
step below includes commands.

**🚀 Step 1: Start Minikube**

minikube start

*Output:*

> • Minikube version: v1.36.0\
> • Kubernetes version: v1.33.1\
> • Driver: Docker\
> • Warnings about Docker disk usage

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image1.png){width="6.5in"
height="2.886110017497813in"}

**🚀 Re-run Minikube with Docker Driver** minikube start \--driver
docker

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image2.png){width="6.5in"
height="2.8847222222222224in"}

✅ **Step 2: Check Minikube Status**\
minikube status

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image3.png){width="6.5in"
height="1.0624989063867016in"}

**🚀 Step 3: Check Cluster Node Info**\
kubectl get node

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image4.png){width="6.5in"
height="0.5625in"}

**🚀 Useful CLI Info**

> • kubectl: used for configuring and managing Kubernetes resources •
> minikube: used for cluster management (start, delete, etc.)

**🚀 Step 4: Apply YAML Configuration Files**

Refer to:

kubectl a\
kubectl apply -f mongo-secret.yaml\
kubectl apply -f mongo.yaml\
kubectl apply -f webapp.yaml

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image5.png){width="6.5in"
height="3.5097222222222224in"}

**🚀 Step 5: Kubernetes Resource Monitoring Commands**

kubectl get node\
kubectl get all\
kubectl get secret

kubectl get pod\
kubectl get configmap\
kubectl help\
kubectl get \--help\
kubectl describe service \<service-name\>\
kubectl describe pod \<pod-name\>

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image6.png){width="6.5in"
height="3.1555555555555554in"}

Resulting webpage on my local:

![](vertopal_97a401fce1fc446eafda662d7e5206df/media/image7.png){width="6.5in"
height="3.0944444444444446in"}

This hands-on demo was a great exercise in managing a Kubernetes
environment locally, simulating real-world microservices deployment with
secrets, configs, and persistent services.
