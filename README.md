# kubernetes-practice

When running kubernetes in local docker desktop, please use below command for setting the context between AKS and docker-desktop
```
kubectl config use-context docker-desktop
```

To create a yaml file for pod definition file, please use below command.

```
 kubectl run redis --image=redis --dry-run=client -o yaml > redis.yaml
```

To set the default namespace,
```
kubectl config set-context $(kubectl config current-context) --namespace=dev
```