# K8s Kind Tool - FullCycle

- Install
  - [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)

  - [kind](https://kind.sigs.k8s.io/docs/user/quick-start/#installation)

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

- Get Nodes

```sh
kubectl get nodes
```

- Apply Pod

```sh
kubectl apply -f k8s/pod.yaml
```

- Port Forward Pod

```sh
kubectl port-forward pod/goserver 8080:8080
```

- URL

  - [http://localhost:8080](http://localhost:8080)

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
