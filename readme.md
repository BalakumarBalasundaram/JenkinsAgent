content here

# Kubernetes
## Use minikube to run a local kubernetes cluster
```
minikube start --cpus=4 --memory=8GB --disk-size=20G --addons=registry,ingress

// Create a namespace
kubectl create namespace my-namespace

// Create a deployment
kubectl create deployment my-deployment --image=nginx --namespace=my-namespace

// Create a service
kubectl expose deployment my-deployment --port=80 --target-port=80 --namespace=my-namespace

// Create an ingress
kubectl apply -f ingress.yaml --namespace=my-namespace

// Create a secret
kubectl create secret generic my-secret --from-literal=secret-key=secret-value --namespace=my-namespace

// Create a configmap
kubectl create configmap my-configmap --from-literal=config-key=config-value --namespace=my-namespace

// Create a job
kubectl apply -f job.yaml --namespace=my-namespace

// Create a cronjob
kubectl apply -f cronjob.yaml --namespace=my-namespace

// Create a statefulset
kubectl apply -f statefulset.yaml --namespace=my-namespace

// Create a daemonset
kubectl apply -f daemonset.yaml --namespace=my-namespace

// Create a pod
kubectl apply -f pod.yaml --namespace=my-namespace

// Create a serviceaccount
kubectl apply -f serviceaccount.yaml --namespace=my-namespace

// Create a role
kubectl apply -f role.yaml --namespace=my-namespace

// Create a rolebinding
kubectl apply -f rolebinding.yaml --namespace=my-namespace

// Create a clusterrole
kubectl apply -f clusterrole.yaml --namespace=my-namespace

// Create a clusterrolebinding
kubectl apply -f clusterrolebinding.yaml --namespace=my-namespace

// Create a persistentvolume
kubectl apply -f persistentvolume.yaml --namespace=my-namespace

// Create a persistentvolumeclaim
kubectl apply -f persistentvolumeclaim.yaml --namespace=my-namespace

// Create a storageclass
kubectl apply -f storageclass.yaml --namespace=my-namespace

// Create a resourcequota
kubectl apply -f resourcequota.yaml --namespace=my-namespace

// Create a limitrange
kubectl apply -f limitrange.yaml --namespace=my-namespace

// Create a horizontalpodautoscaler
kubectl apply -f horizontalpodautoscaler.yaml --namespace=my-namespace

// Create a priorityclass
kubectl apply -f priorityclass.yaml --namespace=my-namespace

// Create a poddisruptionbudget
kubectl apply -f poddisruptionbudget.yaml --namespace=my-namespace

// Create a networkpolicy
kubectl apply -f networkpolicy.yaml --namespace=my-namespace

// Create a podsecuritypolicy
kubectl apply -f podsecuritypolicy.yaml --namespace=my-namespace

// Create a podpreset
kubectl apply -f podpreset.yaml --namespace=my-namespace

// Create a customresourcedefinition
kubectl apply -f customresourcedefinition.yaml --namespace=my-namespace
```

## Use kubectl to interact with a kubernetes cluster
```
// Get all namespaces
kubectl get namespaces

// Get all pods
kubectl get pods --namespace=my-namespace

// Get all services
kubectl get services --namespace=my-namespace

// Get all deployments
kubectl get deployments --namespace=my-namespace

// Get all ingresses
kubectl get ingresses --namespace=my-namespace

// Get all secrets
kubectl get secrets --namespace=my-namespace

// Get all configmaps
kubectl get configmaps --namespace=my-namespace

// Get all jobs
kubectl get jobs --namespace=my-namespace

// Get all cronjobs
kubectl get cronjobs --namespace=my-namespace

// Get all statefulsets
kubectl get statefulsets --namespace=my-namespace

// Get all daemonsets
kubectl get daemonsets --namespace=my-namespace

// Get all pods
kubectl get pods --namespace=my-namespace

// Get all serviceaccounts
kubectl get serviceaccounts --namespace=my-namespace

// Get all roles
kubectl get roles --namespace=my-namespace

// Get all rolebindings
kubectl get rolebindings --namespace=my-namespace

## Setting up minikube

// Install minikube
brew install minikube

// Install kubectl
brew install kubectl

// Install hyperkit
brew install hyperkit

// Install helm
brew install helm

// Install kubectx
brew install kubectx

// Install kubens
brew install kubens

## Windows setup minikube

// Install minikube
choco install minikube

// Install kubectl
choco install kubernetes-cli

// Install hyperkit
choco install hyperkit

// Install helm
choco install kubernetes-helm

// Install kubectx
choco install kubectx


##Prerequisites
Please make sure the following prerequisites are met:
An existing Kubernetes Cluster (v1.17.0 or higher) - This can also be Minikube (See below for setting up Minikube)
The kubectl client (v1.17.0 or higher) - Available from here - https://kubernetes.io/docs/tasks/tools/install-kubectl/
Helm v3 - Available from here - https://helm.sh/docs/intro/install/

Reference:
https://github.com/gogodi91/K8sDevTools


