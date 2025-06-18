cd taller-06


eval $(minikube docker-env)
minikube start
kubens k8sdemo1

echo -n mongouser | base64
echo -n mongopassword | base64

```sh
kubectl apply -f mongo-config.yaml
kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo.yaml
kubectl apply -f webapp.yaml
```

kubectl get all
kubectl describe service webapp-service
kubectl logs webapp-deployment-6bb4795f54-8qgwf
kubectl get services
-> da el puerto pero cual es la ip?
minikube ip
kubectl get node -o wide 

http://192.168.49.2:30100

goto `echo http://$(minikube ip):30100`

