
```sh
cd taller-04
```

```sh
minikube status

kubectl apply -f 04-kubectl-api_simple-pod.yaml
kubectl run hello-cloud --image=gcr.io/google-samples/hello-app:2.0 --restart=Never  --port=8080 ​
minikube dashboard​

```

entrar con k9s y hacer un port forward para verlo funcionando


# taller 4b
eliminar el/los pod creados

```sh
kubectl delete -f 04-kubectl-api_simple-pod.yaml
```

