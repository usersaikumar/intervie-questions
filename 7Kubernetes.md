# Kubernetes
## Components of Kubernetes
- pod
  - smallest unit of k8s
  - abstraction over container(like a layer)
  - you can only interact with kubernetes layer
  - usaully 1 application per pod(can write multi but recomandad 1)
  - Database
  - each pod gets its own IP address
  - new ip address on re-creation
- services
  - permanent IP address
  - lifecycle of pod and service are not connected
  - external services
  - internal services
  - load balancer
- ingress
  - route traffic in to cluster
- configmap
  - external configuaration of your application
- secrets
  - same like as configmap
  - maintain secret data
  - used to store secret data
  - based on 64 encoded
- volumes
  - data base 
  - mounted or storage on local storage
  - storage on remote, outside of k8s cluster
  - k8s doesn't manage any data persistance
- **pod blue prints**
- deployments
  - blueprints for my app pods
  - you create deployments
  - abstraction of pods
  - DB cant be replica by deployments
  - deployments for stateless apps
- statefull set
  - for statefull apps
  - elastic search
  - mango DB
  - statefull set for stateful apps or databases
  - difficult
===============================================================================================================


- ApiVersions
  - app/v1
  - v1
- kind
  - pod
  - deploy
  - secerets
  - services
  - replicas
  - statefull sets
- metadata
  - name
- specs
  - containers
    - name
    - image
    - ports
      - containerPort:
- status

## k8s Architecture
## **Worker Node**
- each node has multiple pods on it
- 3 process must be installed on every node
  - container runtime
  - kubelet
  - kubeproxy
- worker node do the actuall work
- **kublet**
  - kublet interact with both container and node
  - kubelet start a pod with a container inside
- **kube proxy**
  - forword requests
## **Master**
- 4 process must run every master
  - APi Server
  - secheduler
  - controller manager
  - etcd
- **APi Server**
  - cluster gateway
  - acts as a gatekeeper for authentication
  - validate the request
  - load balancer
- **secheduler**
  - assign the node for pod
  - interlligent enough to assign node for pod
  - communicate to kubelet
- **controller manager**
  - detects cluster changes
  - communicates with secheduler
- **etcd**
  - etcd is cluster brain
  - cluster changes get stored in the key value store
  - is cluster healthy
  - what resources are available
  - did the cluster state changed
  - application data is not stored in etcd


## What is kubectl
- command line tool(CLI) for k8s cluster
- the most powerfull command among
  - UI
  - API
  - CLI
- master process
- worker process

## kubernetes Commands
- status of nodes
```
kubectl get nodes
```
- status of pods
```
kubectl get pods
```
- status of deployments
```
kubectl get deployments
```
## Layers of abstraction
- deployment manages
- replica set
- pod is an abstraction
- container


- status of services
```
kubectl get services
```
- status of replicasets
```
kubectl get replicaset
```
- create nginx deployment
```
kubectl create deployment nginx-deployment --image=nginx
```
- edit ngnix deployment
```
kubectl edit deployment nginx-deployment
``` 
```
kubectl create -f pod.yml
```
```
kubectl apply -f pod.yml
```
```
kubectl delete pod pod_name
```
```
kubectl get pods
```
```
kubectl get pods -o wide
```
## debugung commands
- to see logs
```
kubectl logs pod_name
```
- to see describe
```
kubectl describe pod pod_nmae
```
- to enter into the container(or)pod
```
kubectl exec -it pod_name -- bin/bash
```
## deleting deployment
- to delete

```
kubectl delete deployment name
```
## creating a pod -- example
```
apiVersion: v1
kind: Pod
metadata:
  name: nginx
spec:
  containers:
  - name: nginx
    image: nginx:1.14.2
    ports:
    - containerPort: 80
```
- To run yml file
```
kubectl create file.yml
```
- To update yml file
```
kubectl apply file.yml
```
- To delete exsiting pod
```
kubectl delete pods
```


