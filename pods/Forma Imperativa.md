
verificar pods criadas
```bash
kubectl get pods
```

verificar os pods criados em todos os namespaces
```bash
kubectl get pods --all-namespaces
```

criar um pod com o nome de "my-pod-apache-server" e a imagem "httpd" (apache)
```bash
kubectl run my-pod-apache-server --image httpd
```

verificar pods criados com detalhes
```bash
kubectl get pods -o wide
```

deletar um pod por nome "my-pod-apache-server"
```bash
kubectl delete pods my-pod-apache-server
```

delete todos os pods
```bash
kubectl delete --all pods
```
