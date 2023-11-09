verificar todos os deployments.
```bash
kubectl get deployments

#ou

kubectl get deploy
```

apagar todos os `Deployments`. isso apaga todas as `ReplicaSet` e `Pods` referentes a esse `Deployment`.
```bash
kubectl delete deployments --all
```

cria um deployment através do manifesto `my-deployment.yml`.
```bash
kubectl apply -f my-deployment.yml
```
