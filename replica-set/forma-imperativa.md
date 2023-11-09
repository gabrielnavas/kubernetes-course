verificar `ReplicaSet` existentes
```bash
kubectl get replicasets

#ou

kubectl get rs
```

deletar o `ReplicaSet` criado
```bash
kubectl delete replicasets <nome do replicaset>

#ou

kubectl delete rs <nome do replicaset>
```

verificar todos os `ReplicaSets` existes no Kubernetes
```bash
kubectl get rs --all-namespaces
```
