- O objetivo do `ReplicaSet` é sempre recriar um `Pod` caso ele dê algum problema e pare de funcionar.

- Se caso deletarmos um pod desse replicaset, para teste
```bash
kubectl delete pod <nome da pod>
```

Ele criará novamente a `Pod` deletada, nesse caso foi intencional, num caso específico onde algum container dê problema dentro da `Pod` e ela para por algum motivo, o `ReplicaSet` criará novamente também.

- Mesmo se deletarmos todos os `Pods` e verificarmos novamente os `Pods`, eles estarão sendo criados novamente.
```bash
kubectl delete --all pods && kubectl get pods
```
