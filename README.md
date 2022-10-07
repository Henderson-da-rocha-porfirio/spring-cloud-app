# CONFIG SERVER: CLOUD-NATIVE APPLICATIONS COM SPRING CLOUD

## Gerenciamento de configurações

> - 1. Separação de Configs: É a separação das configurações/propriedades dos microsserviços para que essa mesma imagem Docker possa ser implantada em vários ambientes.
> - 2. Injetar Configs: Processo de injetar as configurações/propriedades que o microsserviço precisava durante a inicialidade do serviço.
> - 3. Manter Configs: Manter as configurações/propriedades em um repositório centralizado, juntamente com a versão delas.

|           Microserviços =>                                   |              Gerenciamento de Configs        |                  <=    Dados/Repos           |
|          :---:                                     |         :---:                     |              :---:              |
|               Contas                                         |         O serviço de Config ler              |              DATABASE                      |
|               Empréstimos                                    |         todas as configurações ao conectar   |              CENTRAL DE REPOS              |
|               Cartões                                        |         na central de repositório.           |              File System                   |


> - 4. O Spring Cloud Config oferece suporte ao servidor e ao client para a configuração externalizada em um sistema distribuído.
Com o Servidor Config você tem um lugar central para gerenciar propriedades externas para aplicativos em todos os ambientes.

## Recursos do Spring Cloud Config Server:

> - 1. HTTP, configuração externa baseada em recursos (pares de valor de nome ou conteúdo YAML equivalente).
> - 2. Propriedades de Encriptar e decriptar valores.
> - 3. Incorporado(embeddable) facilmente em um aplicativo Spring Boot usando @EnabIeConfigServer

## Recursos do Config Client(microserviços):

> - 1. Vincular-se ao Servidor Config e inicializa o Ambiente Spring com fontes de propriedade remotas.
> - 2. Propriedades de Encriptar e decriptar valores.

>## Criando um ConfigServer(Spring Cloud Config):

> - 1. No initialzr, procurar config server que possivelmente estará dentro do initialzr
> - 2. Também instalar a dependência actuator.

## Adicionando Spring Cloud a um aplicativo Spring Boot existente([Spring Cloud](https://spring.io/projects/spring-cloud))
Se você possui um aplicativo Spring Boot existente e deseja adicionar o Spring Cloud a esse aplicativo, a primeira etapa é determinar a versão do Spring Cloud que você deve usar. A versão que você usa em seu aplicativo dependerá da versão do Spring Boot que você está usando.

### - A tabela abaixo descreve qual versão do Spring Cloud mapeia para qual versão do Spring Boot.
#### Tabela 1. Compatibilidade do Spring Boot do trem de lançamento
|           2021.0.x - também conhecido como Jubileu                               |              2.6.x, 2.7.x (começando com 2021.0.3)       |
|          :---:                                     |         :---:                     |
|              2020.0.x também conhecido como Ilford                                      |        2.4.x, 2.5.x (começando com 2020.0.3)             |  
|               etc...                                    |         Verificar em: [Spring Cloud](https://spring.io/projects/spring-cloud)  |   
