- É possível aumentar ou diminuir a quantidade de `Pods` de forma imperativa.

- Fazendo um Scale Up
```bash
kubectl scale replicasets <nome do replicaset> --replicas=10
```

- Fazendo um Scale Down
```bash
kubectl scale replicasets <nome do replicaset> --replicas=5
```