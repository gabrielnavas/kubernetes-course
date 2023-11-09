criar um pod usando o manifesto
```bash
kubectl create -f my-pod.yml

# ou

kubectl apply -f my-pod.yml
```


manifesto do `Pod` `my-pod.yml`
```yaml
apiVersion: v1 # versão da api
kind: Pod # tipo do objeto, tipo do recurso

metadata:
  name: my-pod-webserver # nome do recurso
  labels: # usado para referenciar esse Pod por essas etiquetas
    apps: my-app
    tier: frontend
  
spec: # especificações do Pod
  containers: # containers que estaram dentro desse pod
    - name: my-container-nginx # nome do container
      image: nginx # imagem usava para o containers
```