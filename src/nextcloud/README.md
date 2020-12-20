# Build the nextcloud

Create a persistent volume for mariadb using mysql-storage.yaml.
```
kubectl create -f . /mysql-storage.yaml
```

Create a pod for mariadb using mysql-pod.yaml.
```
kubectl create -f . /mysql-pod.yaml
```

Create a mariadb endpoint using mysql-service.yaml.
```
kubectl create -f . /mysql-service.yaml
```

Create a persistent volume for Nextcloud using nextcloud-storage.yaml.
```
kubectl create -f . /nextcloud-storage.yaml
```

Create a pod for Nextcloud using nextcloud-pod.yaml.
```
kubectl create -f . /nextcloud-pod.yaml
```

Create a Nextcloud endpoint using nextcloud-service.yaml.
```
kubectl create -f . /nextcloud-service-.yaml
```

## Operation check

```
minikube service nextcloud-service --url
````
You can access the URL obtained by ...
