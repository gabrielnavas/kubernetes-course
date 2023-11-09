- Scale Up
	- Para aumentar a quantidade de réplicas de `Pods`, é só alterar o número de replicas no manifesto do `ReplicaSet`
	
	manifesto `my-replicaset.yml`
	```yml
	...
	replicas: 8 # quantidade de pods de 4 para 8
	...
	```
	
	- Logo após a alteração, save o arquivo e rode o comando
	```bash
	kubectl apply -f my-replicaset.yml
	``````
	
	- O `ReplicaSet` aumentará a quantidade de `Pods` até o número configurado dentro do manifesto.

- Scale Down
	- Da mesma forma que fizemos o Scale Up, aumentando a quantidade de `Pods`, podemos diminuir também, funciona da mesma forma.
	
	 - Para diminuir a quantidade de réplicas de `Pods`, é só alterar o número de replicas no manifesto do `ReplicaSet`
	
		manifesto `my-replicaset.yml`
	```yml
	...
	replicas: 3 # quantidade de pods de 8 para 3
	...
	```
	
	- Logo após a alteração, save o arquivo e rode o comando
	```bash
	kubectl apply -f my-replicaset.yml
	``````
	
	- O `ReplicaSet` diminuirá a quantidade de `Pods` até o número configurado dentro do manifesto.