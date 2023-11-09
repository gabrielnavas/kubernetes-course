- O `Deployment` Faz a implantação da aplicação.

- Tipos de atualização.
	- `Rolling Updates` (Rolling Release)
		- Atualização dos `Pods` será feita um por um. 
		- No mínimo terá 75% dos pods em status `running`.
		- O Kubernetes verifica qual `Pod` está tendo menor  tráfego, derruba e sobe a nova versão. Isso para cada Pod, até todos os `Pods` terem a nova versão. Quando sobre a nova versão, em cada `Pod`
	  
	- `Recreate Deployment`
		- Para todas as Pods e sobe as novas `Pods` com as novas versões. Pode causar uma indisponibilidade.  
		- Essa estratégia deve ser feita em casos específicos.

	- `Rollback`
		- Voltar ao estado anteriormente.
