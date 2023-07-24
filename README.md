# curl-list-pods

## Run

1. Create a Kubernetes cluster. (Using kind for example)

```sh
kind create cluster --name yk8s --image kindest/node:v1.26.6
```

2. Get kubconfig.

```sh
rm ~/.kube/config
kind get kubeconfig --name yk8s > ~/.kube/config
```

3. Apply the YAML.

```sh
kubectl apply -f list-pods.yaml
```

4. Get result.

```sh
kubectl logs list-pods
```



