# CONFIG SERVER: LENDO CONFIGS DO GITHUB
### Segurança dos dados
> a. Apontar para o repositório externo do Github

> b. Apagar a pasta "config" e só ler apenas a que está no Github

> c. Fazer estes apontamentos em application properties:
````
spring.profiles.active=git
spring.cloud.config.server.git.uri=https://github.com/Henderson-da-rocha-porfirio/microservices-configserver-properties.git
spring.cloud.config.server.git.clone-on-start=true
spring.cloud.config.server.git.default-label=main(branch só de exemplo. Deve colocar a que deseja)
````
