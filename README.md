# MICROSERVICE WORKER
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Eduguimar/hr-worker/blob/master/LICENSE) 

## Sobre o Projeto

Projeto extra desenvolvido durante o bootcamp Spring-React da [`DevSuperior`](https://devsuperior.com.br).

Sistema de microsserviços Java com Spring Boot, Spring Security e Spring Cloud (Feign, Ribbon, Hystrix, OAuth, JWT, Discovery Server Eureka, API Gateway Zuul, Config Server). Microsserviços executando em containers Docker, utilizando escalonamento automático e balanceamento de carga.

Dados armazenados em banco de dados Postgres 12.

![Microservices](https://github.com/Eduguimar/hr-worker/blob/master/img/microservices.PNG)

### HR-WORKER
Microsserviços de trabalhadores, que comunicam por API passando os nomes, salário por dia e números de dias trabalhados. É um microsserviço escalável.

### HR-PAYROLL
Microsserviços de cálculo de pagamento, que realiza o cálculo do salário total dos empregados de acordo com os dados passados pelo HR-WORKER. Também é um microsserviço escalável.
![Payroll](https://github.com/Eduguimar/hr-worker/blob/master/img/payroll.PNG)

### HR-EUREKA-SERVER
O Eureka é um módulo do Spring Cloud que permite que os microsserviços sejam registrados e descobertos na rede através do nome.
![Eureka](https://github.com/Eduguimar/hr-worker/blob/master/img/spring-eureka.PNG)

### HR-API-GATEWAY-ZUUL
O API Gateway Zuul é um módulo do Spring Cloud responsável pelo recebimento das chamadas do cliente e roteamento delas entre os microsserviços. Nesta aplicação, o API Gateway Zuul também é o servidor de recursos.

### HR-CONFIG-SERVER
Servidor de configuração que realiza a comunicação com o repositório do Github, do qual lê os parâmetros e arquivos de configuração do sistema.

### HR-USER
Serviço responsável pelos usuários que acessam o sistema. Possui conexão com o banco Postgres.

### HR-OAUTH
Serviço responsável pela autenticação e autorização de acesso dos usuários ao sistema.

### Serviços executando no Docker
![Docker](https://github.com/Eduguimar/hr-worker/blob/master/img/docker-ps.PNG)

## Tecnologias utilizadas
### Back end
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- H2
- Postgresql
- PgAdmin
- Feign
- Ribbon
- Hystrix
- OAuth2
- JWT
- Eureka Server
- Config Server
- API Gateway Zuul
- Docker

## Autor
Eduardo Guimarães

## Licença
[MIT](https://github.com/Eduguimar/hr-worker/blob/master/LICENSE)
