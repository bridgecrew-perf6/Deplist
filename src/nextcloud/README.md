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

Use nextcloud-strage.yaml to create a persistent volume for Nextcloud.
```
kubectl create -f . /nextcloud-storage.yaml
```

Use nextcloud-pod.yaml to create a pod for nextcloud.
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
