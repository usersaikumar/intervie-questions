# Kubernetes
## Components of Kubernetes
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
      - containerPort: 80
- status

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

