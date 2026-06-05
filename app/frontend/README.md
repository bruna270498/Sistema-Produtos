# Frontend - Sistema de Gerenciamento de Produtos

## Sobre

Aplicação Web desenvolvida em Vue.js responsável pela interação do usuário com o sistema de gerenciamento de produtos.

O Front-end consome uma API REST desenvolvida em TypeScript para realizar operações de cadastro, consulta, atualização e exclusão de produtos.

---

## Tecnologias Utilizadas

* Vue.js 3
* Vue Router
* Axios
* JavaScript
* Webpack

---

## Funcionalidades

### Listagem de Produtos

Rota:

```text
/
```

Exibe todos os produtos cadastrados no sistema.

---

### Consulta de Produto por ID

Rota:

```text
/produto/:id
```

Permite visualizar os detalhes de um produto específico.

Exemplo:

```text
/produto/1
```

---

### Cadastro de Produto

Rota:

```text
/cadastro
```

Permite cadastrar novos produtos através de formulário integrado à API.

---

## Estrutura de Rotas

| Página         | Rota           |
| -------------- | -------------- |
| Produtos       | `/`            |
| Produto por ID | `/produto/:id` |
| Cadastro       | `/cadastro`    |

---

## Instalação

Instalar dependências:

```bash
npm install
```

---

## Executar Projeto

Modo desenvolvimento:

```bash
npm run serve
```

---

## Gerar Build

```bash
npm run build
```

---

## Comunicação com API

O Front-end realiza chamadas HTTP para os endpoints disponibilizados pela API de Produtos.

Exemplos:

### Listar Produtos

```http
GET /produtos
```

### Buscar Produto por ID

```http
GET /produtos/:id
```

### Cadastrar Produto

```http
POST /produtos
```

### Atualizar Produto

```http
PUT /produtos/:id
```

### Excluir Produto

```http
DELETE /produtos/:id
```

---

## Diferenciais

* Navegação SPA (Single Page Application).
* Rotas com carregamento Lazy Loading.
* Integração com API REST.
* Interface desacoplada do Back-end.
* Arquitetura baseada em componentes Vue.
