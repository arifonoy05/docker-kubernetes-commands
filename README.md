# Docker Commands
### Build image: ``` docker build -t IMAGE_NAME PATH_TO_DOCKERFILE ``` where
- IMAGE_NAME is the name for the image. eg ``` username/project_name ```
- PATH_TO_DOCKERFILE is the path to dockerfile, usually ``` . ``` 

### Run container: ``` docker run -d --name GIVEN_CONTAINER_NAME -v "HOST_PATH:CONTAINER_PATH" -p EXPOSED_PORT:CONTAINER_PORT IMAGE_NAME ``` where
- ``` -d ``` if for detached mode so that the terminal is accessible for use
- ``` --name ``` sets a name for the running container. If the flag is not used, docker will set a random name for the container
- ``` -v ```, volumes, is used to bind a local project path to the docker container. I use this to avoid building and running a container to check for project changes. example command ``` -v $(pwd):usr/share/nginx/html ``` here ```$(pwd)``` gives the present working directory and ```usr/share/nginx/html``` is the project path inside the container. This flag is slightly tricky to use.
- ``` -p ``` maps port to the container so that the container can be accessed.
- ``` IMAGE_NAME ``` is the image you are pulling. It can also be the image you build with ``` docker build ``` command

# Kubernetes
### start minikube: ``` minikube start ```
### special case
```
$env:KUBECONFIG="" 
$env:KUBECONFIG=""
minikube start
```
