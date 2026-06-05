# Backend - API de Gerenciamento de Produtos

## Sobre

API REST desenvolvida em TypeScript responsável pelo gerenciamento de produtos da aplicação.

O projeto utiliza Express para disponibilização dos endpoints, Sequelize como ORM para comunicação com o banco de dados MySQL e Docker para conteinerização da aplicação.

A API é responsável pelas operações de cadastro, consulta, atualização e exclusão de produtos, servindo como camada de negócio para o Front-end desenvolvido em Vue.js.

---

## Tecnologias Utilizadas

* Node.js
* TypeScript
* Express
* Sequelize ORM
* MySQL
* Docker

---

## Funcionalidades

### Cadastro de Produto

Permite registrar um novo produto no banco de dados.

### Listagem de Produtos

Retorna todos os produtos cadastrados.

### Consulta de Produto por ID

Retorna os dados de um produto específico.

### Atualização de Produto

Permite alterar informações de um produto existente.

### Exclusão de Produto

Remove um produto do banco de dados.

---

## Endpoints

### Criar Produto

```http
POST /produtos
```

Exemplo de payload:

```json
{
  "name": "Notebook Dell",
  "price": 4500,
  "tipo": "Eletrônico",
  "description": "Notebook para trabalho e estudos"
}
```

---

### Listar Produtos

```http
GET /produtos
```

---

### Buscar Produto por ID

```http
GET /produtos/:id
```

Exemplo:

```http
GET /produtos/1
```

---

### Atualizar Produto

```http
PUT /produtos/:id
```

Exemplo:

```json
{
  "name": "Notebook Dell Inspiron",
  "price": 4800,
  "tipo": "Eletrônico",
  "description": "Modelo atualizado"
}
```

---

### Excluir Produto

```http
DELETE /produtos/:id
```

---

## Banco de Dados

A aplicação utiliza MySQL como banco de dados relacional.

O acesso e manipulação dos dados são realizados através do Sequelize ORM, permitindo:

* Mapeamento objeto-relacional (ORM)
* Criação e manipulação de modelos
* Consultas simplificadas
* Integração com TypeScript
* Gerenciamento de conexões com o banco

---

## Executando Localmente

### Instalar dependências

```bash
npm install
```

### Executar em modo desenvolvimento

```bash
npm run dev
```

### Gerar build da aplicação

```bash
npm run build
```

### Executar versão compilada

```bash
npm start
```

---

## Variáveis de Ambiente

Exemplo de arquivo `.env`:

```env
DB_HOST=localhost
DB_PORT=3306
DB_NAME=produtos
DB_USER=root
DB_PASSWORD=root

PORT=3000
```

---

## Executando com Docker

Subir todos os serviços:

```bash
docker compose up --build
```

ou

```bash
docker-compose up --build
```

A API ficará disponível em:

```text
http://localhost:3000
```


---

## Boas Práticas Aplicadas

* Arquitetura em camadas
* Separação de responsabilidades
* Utilização de ORM (Sequelize)
* API RESTful
* TypeScript para tipagem estática
* Conteinerização com Docker
* Integração contínua entre Front-end, Back-end e Banco de Dados


