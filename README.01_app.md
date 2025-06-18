cd ~/.apps/e_nuvu.Apps/02_Proyectos/0031_Nuv_TechTalks_K8s

# prerreqs

* brew
* then...

```sh
brew install docker​
brew install kubectl      # … for configure cluster​
brew install minikube  # … for startup / delete cluster
```

# first run

```sh
eval $(minikube docker-env)​

minikube start #--driver=docker​

minikube profile list​

kubectl get nodes​
kubectl describe node minikube​
kubectl get pods -o wide -A

minikube addons list​
minikube addons enable registry​
minikube addons enable metrics-server​

kubectl get namespaces
kubectl create namespace k8sdemo1​
kubens  k8sdemo1​

kubectl config use-context minikube   ​

```


# taller-04
ver [taller-04](./taller-04/README.md)

# taller-05
ver [taller-05](./taller-05/README.md)

# taller-06
ver [taller-06](./taller-06/README.md)


# finalmente

eliminar el namespace de trabajo
kubectl delete namespace k8sdemo1__