cd taller-05

```sh
kubectl create deployment nginx-depl --image=nginx

kubectl edit deployment nginx-depl
#edit replicas to 2


kubectl get replicaset #(cuando hay mas de un nodo)
kubectl get pod # para ver pods cereados
kubectl logs ___<pod-name>__ # para ver logs
kubectl describe pod __<pod-name>__
kubectl exec -it __<od-name>__ -- bin/bash # interactive terminal
kubectl get deployment
```

o bien usar 
`kubectl apply -f 05-kubectl-nginx.yaml`

luego: 
`kubectl apply -f 05b-kubectl-service.yaml`


accederlo via:
`echo http://$(minikube ip):30081`


`kubectl get pod -o wide`

```
* posteriormetne eliminar

```sh
kubectl delete -f 05-kubectl-nginx.yaml
```
