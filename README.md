# redis-kubernetes-cluster

Deploy

`kubectl create -f redis-master-pod.yml`

`kubectl create -f sentinel-service.yml`

`kubectl create -f redis-controller.yml`

`kubectl create -f sentinel-controller.yml`

Scale

`kubectl scale rc redis --replicas=3`

`kubectl scale rc redis-sentinel --replicas=3`

Delete

`kubectl delete pods redis-master`
