# K8s Kind Tool - FullCycle

## Install

- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)

- [kind](https://kind.sigs.k8s.io/docs/user/quick-start/#installation)

## Clusters

- Create Cluster

```sh
kind create cluster --config=k8s/kind.yaml --name=fullcycle
```

- Use Cluster

```sh
kubectl cluster-info --context kind-fullcycle
```

- Get Clusters

```sh
kind get clusters
kubectl config get-clusters
```

## Nodes

- Get Nodes

```sh
kubectl get nodes
```

## Pods

- Apply Pod

```sh
kubectl apply -f k8s/pod.yaml
```

- Port Forward Pod - [http://localhost:8080](http://localhost:8080)

```sh
kubectl port-forward pod/goserver 8080:8080
```

- Get Pods

```sh
kubectl get po
kubectl get pod
kubectl get pods
```

- Delete Pod (goserver)

```sh
kubectl delete pod goserver
```

## Replicasets

- Apply Replicaset

```sh
kubectl apply -f k8s/replicaset.yaml
```

- Port Forward Replicaset - [http://localhost:8080](http://localhost:8080)

```sh
kubectl port-forward replicaset/goserver 8080:8080
```

- Get  Replicasets

```sh
kubectl get replicaset
kubectl get replicasets
```

- Delete Replicaset (goserver)

```sh
kubectl delete replicaset goserver
```
