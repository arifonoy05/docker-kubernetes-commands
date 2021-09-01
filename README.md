# Docker Commands
Build image ``` docker build -t *IMAGE_NAME* *PATH_TO_DOCKERFILE* ``` where
- IMAGE_NAME is the name for the image. eg ``` username/project_name ```
- PATH_TO_DOCKERFILE is the path to dockerfile, usually ``` . ``` 
Run container ``` docker run -d --name ** ```
# Kubernetes
```
minikube start
```
### special case
```
$env:KUBECONFIG="" 
$env:KUBECONFIG=""
minikube start
```
