# Back-End Challenge - Contas Correntes

## Ferramentas obrigatórias: 
- Docker
- Insomnia
- Java 17

## Executar a aplicação

Execute os comandos separadamente. Obs: Tenha o Docker instalado para subir as aplicações e o RabbitMQ.

```sh
docker compose build
```

```sh
docker compose up
```

## Funcionalidades implementadas

- [x] Criação de usuario - **[USER]**
- [x] Consulta de usuário por documento - **[USER]**
- [x] Criação da conta - **[ACCOUNT]**
- [x] Buscar conta pelo número da mesma - **[ACCOUNT]**
- [x] Consultar conta disponível para efetuar transação - **[ACCOUNT]**
- [x] Criar transação - **[TRANSACTION]**
- [x] Cancelar transação - **[TRANSACTION]**

## Documentação

A documentação Swagger está disponível nas URLs. Obs: Deixe as aplicações em execução para acessar

**[USER]**           - http://localhost:8080/swagger-ui.html

**[ACCOUNT]**        - http://localhost:8081/swagger-ui.html

**[TRANSACTION]**    - http://localhost:8082/swagger-ui.html

## Testes unitários

Nos testes unitários e integrados foi usado as libs. Obs: Necessário Docker para executar os testes
* TestContainers 
* MockServer
* JUnit
* Mockito

## Arquitetura aplicada

[arquitetura_aplicada.png](https://github.com/igorsbezerra/f1rst-backend-challenge/blob/main/arquitetura_aplicada.png)

## Payloads

[Rest Client Insomnia - payloads-insomnia.json](https://github.com/igorsbezerra/f1rst-backend-challenge/blob/main/payloads-insomnia.json)

## Design Patterns

Padrão de projeto aplicado nos serviços

* Publish/Subscribe - RabbitMQ
* Adapter
* Command
* Method Factory
* Dependency Injection
* SOLID
* Microservice pattern
