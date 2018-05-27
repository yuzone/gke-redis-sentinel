# gke-redis-sentinel

## Howto

### Settings(asia-northeast1-a)
```
# region
gcloud config set compute/region asia-northeast1
# zone
gcloud config set compute/zone asia-northeast1-a
```

### Create Cluster
```
gcloud deployment-manager deployments create my-redis --config cluster.yaml
```

### Get Credentials
```
gcloud container clusters get-credentials my-redis
```

### Create ConfigMap
```
kubectl apply -f configmap.yaml
```

### Create Service
```
kubectl apply -f service.yaml
```

### Create StatefulSet
```
kubectl apply -f statefulset.yaml
```

