# Testes Automatizados

## Objetivo

Garantir o correto funcionamento da aplicação através da validação integrada entre Front-end e Back-end.

Os testes simulam ações reais do usuário na interface e posteriormente validam os dados persistidos e retornados pela API.

---

## Tecnologias Utilizadas

* Python
* Selenium WebDriver
* Pytest
* Requests

---

## Estratégia de Teste

Foi adotada uma abordagem End-to-End (E2E), validando:

* Interface do usuário (Front-end)
* Regras de negócio do Back-end
* Comunicação entre Front-end e API
* Persistência dos dados

---

## Cenários Automatizados

### Atualização de Produto

Fluxo validado:

1. Acessar a tela de detalhes do produto.
2. Acionar a funcionalidade de edição.
3. Alterar os dados do produto.
4. Confirmar a atualização.
5. Validar a mensagem de sucesso na interface.
6. Realizar consulta direta na API.
7. Confirmar que os dados foram efetivamente atualizados.

### Exclusão de Produto

Fluxo validado:

1. Acessar a tela de detalhes do produto.
2. Acionar a exclusão.
3. Confirmar a operação.
4. Validar a mensagem de sucesso na interface.
5. Consultar a API.
6. Confirmar que o produto não existe mais.

---

## Executando os Testes

Instalar dependências:

```bash
pip install -r requirements.txt
```

Executar:

```bash
pytest
```

ou

```bash
python -m pytest
```

---

## Diferenciais

* Validação de Front-end e Back-end em um único fluxo.
* Testes automatizados executados em ambiente Docker.
* Verificação de mensagens visuais para o usuário.
* Validação dos dados diretamente na API após cada operação.
* Cobertura dos fluxos críticos de atualização e exclusão de produtos.
