# <<<<<<<<< Required/Must Basics - before starting kubernetes. >>>>>>>>>>>>>> #

1. Getting Started with Docker & Working with Containers.
	url: [https://devopscube.com/getting-started-with-docker-contianers/]

   > Containers are sandboxed environments which run multiple processes sharing the same host kernel.
   > All the layers in an image are read-only except the topmost layer. The writable layer can be called as a container.
   > Containers are created from docker images,An image can contain multiple layers. Layer 0 is called the base image.

A container as we all know, is a self-contained environment where we package applications and their dependencies. Typically a container runs a single process (Although there are ways to run multiple processes). Each container gets an IP address and can attach volumes and control CPU and memory resources, among other things. All these happen via the concepts of namespaces and control groups.

2. Getting Started with Kubernetes & Pods;
	url: [https://devopscube.com/kubernetes-pod/]
 
Kubernetes is a container orchestration system for deploying, scaling, and managing containerized applications and it has its own way of running containers. We call it a pod. A pod is the smallest deployable unit in Kubernetes that represents a single instance of an application.

  > Containers must run with in a host by using host kernal/libs/resources. 
  > In Kubernetes - Continaers will not run directly on hosts - Pod acts as a host in kubernetes for containers.

  > Pods are the smallest deployable units in Kubernetes.
  > Pods are ephemeral in nature; they can be created, deleted, and updated.
  > A pod can have more than one container; there is no limit to how many containers you can run inside a pod.
  > Each pod gets a unique IP address.
  > Pods communicate with each other using the IP address.
  > Containers inside a pod connect using localhost on different ports.
  > Containers running inside a pod should have different port numbers to avoid port clashes.
  > You can set CPU and memory resources for each container running inside the pod.
  > Containers inside a pod share the same volume mount.
  > All the containers inside a pod are scheduled on the same node; It cannot span multiple nodes.
