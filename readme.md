#### Minikube commands

```
minikube start --driver=docker
```

#### set default driver

```
minikube config set driver docker
```


#### Get the ip

```
minikube ip
minikube service list
```

or 

```
kubectl get node -o wide
```


#### Encode with base64

username: mongouser
password: mongopassword

```
echo -n mongouser | base64
```


#### List the pods

```
kubectl get pod
```

#### List the service

```
kubectl get svc
```

or 


```
kubectl get service
```

#### List all 

```
kubectl get all
```

#### List configmap

```
kubectl get configmap
```

#### List secret

```
kubectl get secret
```


#### see the log

```
kubectl logs <podname>
```

#### Apply changes through files

```
kubectl apply -f mongo-config.yaml
kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo.yaml
kubectl apply -f webapp.yaml
```

#### On windows needs to port forward

syntax: kubectl port-forward service/<service-name> <fwd-port>:<service-port>


```
kubectl port-forward service/webapp-service 31000:3000
```