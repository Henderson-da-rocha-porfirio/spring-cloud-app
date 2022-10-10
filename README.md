# CONFIG SERVER: LENDO CONFIGS NUMA PASTA DO SISTEMA LOCAL
### Segurança dos dados
> a. Copiar a pasta "config" e colar em uma pasta do sistema(C ou D)

> b. Apagar a pasta "config" e só ler apenas a que criou no sistema local

> c. Fazer este apontamento em application properties:
````
spring.cloud.config.server.native.search-locations=file:///D://config
````
