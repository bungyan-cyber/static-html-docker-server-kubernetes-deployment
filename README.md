static-html-docker-server-kubernetes-deployment <a name="TOP"></a>
===================

- - - - 
# Steps for Deploying a Static HTML Site with Docker  #

    docker build -t index-app:v1 .
    docker build -t index-app:v1 . 
    docker run -d -p 80:80 index-app:v1
    docker ps
    docker container 
    docker image list


# Steps for push to dockerhub repository  #

    docker tag index-app:v1 bungyan07/index-app:v1
    docker login 
    docker push bungyan07/index-app:v1

# Architecture #

# Service Deployment Into Kubernetes  #

    Kubernetes service yaml = default
    kubectl get componentstatuses
    kubectl cluster-info
    kubectl get nodes
    kubectl create namespace staging
    kubectl create namespace production
    kubectl create namespace dev
    
# Service Deployment Into Kubernetes from namespaces  #

    Kubernetes service yaml = dev

# Service Deployment Into Kubernetes from namespaces  #

    Kubernetes service yaml = staging

# Service Deployment Into Kubernetes from namespaces  #

    Kubernetes service yaml = prod

# Run Service Deployment Into Kubernetes #
    kubectl apply -f yaml -n (namespaces)

# add horizontal pod autoscaling on web app with cpu and memory metrics #
    kubectl get pods 
    kubectl get pods --all-namespaces -o wide
    kubectl get pod -o wide
    kubectl get services
    kubectl get pods --all-namespaces
    kubectl get hpa

# Run Service HPA Deployment Into Kubernetes #
    kubectl apply -f yaml -n 
 












