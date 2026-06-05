# Sistema de Gerenciamento de Produtos

## Sobre o Projeto

Este projeto consiste em uma aplicação Full Stack para gerenciamento de produtos, composta por uma API REST desenvolvida em TypeScript, uma interface Web desenvolvida em Vue.js e testes automatizados End-to-End utilizando Python.

A aplicação permite o cadastro, consulta, atualização e exclusão de produtos, garantindo a comunicação entre Front-end, Back-end e Banco de Dados através de containers Docker.

---

## Funcionalidades

### Produtos

* Cadastro de produtos
* Listagem de todos os produtos
* Consulta de produto por ID
* Atualização de produtos
* Exclusão de produtos

### Testes Automatizados

* Validação dos fluxos da interface
* Validação da integração Front-end e Back-end
* Validação dos dados retornados pela API
* Testes End-to-End utilizando Selenium

---

## Arquitetura

```text
┌─────────────────┐
│    Frontend     │
│     Vue.js      │
└────────┬────────┘
         │ HTTP
         ▼
┌─────────────────┐
│    Backend      │
│ TypeScript API  │
│ Express         │
│ Sequelize ORM   │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│      MySQL      │
└─────────────────┘

         ▲
         │
┌─────────────────┐
│ Selenium Tests  │
│ Python + Pytest │
└─────────────────┘
```

---

## Tecnologias Utilizadas

### Front-end

* Vue.js 3
* Vue Router
* Axios
* JavaScript

### Back-end

* Node.js
* TypeScript
* Express
* Sequelize
* MySQL

### Testes

* Python
* Selenium WebDriver
* Requests
* Pytest

### Infraestrutura

* Docker
* Docker Compose

---

## Estrutura do Projeto

```text
.
├── frontend/
├── backend/
├── tests/
├── docker-compose.yml
└── README.md
```

---

## Executando o Projeto

### Pré-requisitos

* Docker
* Docker Compose

### Subir todos os serviços

```bash
docker compose up --build
```

ou

```bash
docker-compose up --build
```

---

## Serviços Disponíveis

| Serviço      | Descrição                             |
| ------------ | ------------------------------------- |
| Front-end    | Interface Vue.js                      |
| Back-end     | API REST TypeScript                   |
| MySQL        | Banco de Dados                        |
| Testes       | Automação E2E                         |
| Health Check | Validação da disponibilidade do banco |

---

## Diferenciais do Projeto

* Arquitetura Full Stack.
* API REST desenvolvida em TypeScript.
* Persistência utilizando Sequelize ORM.
* Front-end desacoplado consumindo API REST.
* Testes automatizados End-to-End.
* Ambiente totalmente conteinerizado com Docker.
* Integração completa entre Front-end, Back-end e Banco de Dados.

---

## Autor

Bruna Almeida

Projeto desenvolvido para estudo prático de desenvolvimento Full Stack, automação de testes e conteinerização utilizando Docker.
