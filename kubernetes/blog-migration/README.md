# Migrating an existing Wordpress blog to run on Kubernetes

## Objective
In this series, we want to migrate an existing Wordpress blog (for which
we have an existing MySQL database dump and a Wordpress directory) to run
on a kubernetes cluster.

Along the way, we want to exercies the different parts of installing and
operating a kubernets cluster and deploying applications to it.

## Exploration Areas

  - [ ] Running a local Kubernetes cluster using Minikube
    - [ ] Installing Minikube
    - [ ] Creating Hyper-V virtual switch
    - [ ] Creating Minikube Cluster
          `minikube start --vm-driver=hyperv --hyperv-virtual-switch=minikube`

  - [ ] Using `kubectl` to interact with the cluster
    - [ ] Installing kubectl
    - [ ] Checking cluster connectivity
          `kubectl get pods`

  - [ ] Pointing Docker to Kubernetes cluster
        `& minikube docker-env | Invoke-Expression`

  - [ ] Deploying basic Wordpress pod

  - [ ] Deploying Wordpress using Helm

  - [ ] Creating data initialization containers to load-in existing mysql and wordpress data
 
## Unanswered Questions
  - How to run pods that exceed the declared resources on a node?
    - For testing larger configurations locally on minikube.
