## 🚀 SOLUÇÃO PARA MOTTU
## 👥 Integrantes
Ana Carolina de Castro Gonçalves - RM554669

Luisa Danielle - RM555292

Michelle Marques Potenza - RM557702

## 📋 Sobre o Projeto
Automação de testes para API REST desenvolvida em Spring Boot para o sistema Mottu. Este projeto contém uma suíte completa de testes automatizados para validar todos os endpoints da API.

## 📊 Resumo dos Testes
Caso de Teste	Requests	Status
CRUD Cliente	4	✅
Validações Cliente	3	✅
CRUD Moto	4	✅
CRUD Funcionário	4	✅
CRUD Pátio	4	✅
Total	19	✅


## 🔧 Requisições Implementadas
## 👥 Módulo Cliente
POST /clientes - Criar novo cliente

GET /clientes/{id} - Buscar cliente por ID

PUT /clientes/{id} - Atualizar cliente

DELETE /clientes/{id} - Excluir cliente

## 👨‍💼 Módulo Funcionário
POST /funcionarios - Criar novo funcionário

GET /funcionarios - Listar funcionários

GET /funcionarios/{id} - Buscar funcionário por ID

PUT /funcionarios/{id} - Atualizar funcionário

DELETE /funcionarios/{id} - Excluir funcionário

## 🏍️ Módulo Moto
POST /motos - Criar nova moto

GET /motos - Listar motos

GET /motos/{id} - Buscar moto por ID

PUT /motos/{id} - Atualizar moto

DELETE /motos/{id} - Excluir moto

## 🅿️ Módulo Pátio
POST /patios - Criar novo pátio

GET /patios - Listar pátios

GET /patios/{id} - Buscar pátio por ID

PUT /patios/{id} - Atualizar pátio

DELETE /patios/{id} - Excluir pátio

## 🧪 Plano de Testes Manuais
Testes Planejados
Aqui estão os principais testes realizados para validar os endpoints da API:

## 👥 Módulo Cliente
**Criar Cliente**

Método HTTP: POST

Endpoint: /clientes

Objetivo: Verificar se um cliente é criado com sucesso.

Prioridade: Alta

**Listar Cliente**

Método HTTP: GET

Endpoint: /clientes

Objetivo: Verificar se a listagem de clientes funciona.

Prioridade: Média

**Buscar Cliente por ID**

Método HTTP: GET

Endpoint: /clientes/{clienteId}

Objetivo: Verificar se a busca por um cliente funciona corretamente.

Prioridade: Alta

**Atualizar Cliente**

Método HTTP: PUT

Endpoint: /clientes/{clienteId}

Objetivo: Verificar se a atualização do cliente ocorre corretamente.

Prioridade: Média

**Excluir Cliente**

Método HTTP: DELETE

Endpoint: /clientes/{clienteId}

Objetivo: Verificar se a exclusão do cliente funciona corretamente.

Prioridade: Alta

## 👨‍💼 Módulo Funcionário
**Criar Funcionário**

Método HTTP: POST

Endpoint: /funcionarios

Objetivo: Verificar se um funcionário é criado com sucesso.

Prioridade: Alta

**Listar Funcionários**

Método HTTP: GET

Endpoint: /funcionarios

Objetivo: Verificar se a listagem de funcionários funciona.

Prioridade: Média

**Buscar Funcionário por ID**

Método HTTP: GET

Endpoint: /funcionarios/{funcionarioId}

Objetivo: Verificar se a busca por funcionário funciona.

Prioridade: Alta

**Atualizar Funcionário**

Método HTTP: PUT

Endpoint: /funcionarios/{funcionarioId}

Objetivo: Verificar se a atualização do funcionário ocorre corretamente.

Prioridade: Média

**Excluir Funcionário**

Método HTTP: DELETE

Endpoint: /funcionarios/{funcionarioId}

Objetivo: Verificar se a exclusão do funcionário funciona.

Prioridade: Alta

## 🏍️ Módulo Moto
**Criar Moto**

Método HTTP: POST

Endpoint: /motos

Objetivo: Verificar se uma moto é criada com sucesso.

Prioridade: Alta

**Listar Motos**

Método HTTP: GET

Endpoint: /motos

Objetivo: Verificar se a listagem de motos funciona.

Prioridade: Média

**Buscar Moto por ID**

Método HTTP: GET

Endpoint: /motos/{motoId}

Objetivo: Verificar se a busca por moto funciona.

Prioridade: Alta

**Atualizar Moto**

Método HTTP: PUT

Endpoint: /motos/{motoId}

Objetivo: Verificar se a atualização da moto ocorre corretamente.

Prioridade: Média

**Excluir Moto**

Método HTTP: DELETE

Endpoint: /motos/{motoId}

Objetivo: Verificar se a exclusão da moto funciona.

Prioridade: Alta

## 🅿️ Módulo Pátio
**Criar Pátio**

Método HTTP: POST

Endpoint: /patios

Objetivo: Verificar se um pátio é criado com sucesso.

Prioridade: Alta

**Listar Pátios**

Método HTTP: GET

Endpoint: /patios

Objetivo: Verificar se a listagem de pátios funciona.

Prioridade: Média

**Buscar Pátio por ID**

Método HTTP: GET

Endpoint: /patios/{patioId}

Objetivo: Verificar se a busca por pátio funciona.

Prioridade: Alta

**Atualizar Pátio**

Método HTTP: PUT

Endpoint: /patios/{patioId}

Objetivo: Verificar se a atualização do pátio ocorre corretamente.

Prioridade: Média

**Excluir Pátio**

Método HTTP: DELETE

Endpoint: /patios/{patioId}

Objetivo: Verificar se a exclusão do pátio funciona.

Prioridade: Alta


# Instruções de uso
Rode a aplicação java na raiz do projeto com:
```bash
.\gradlew BootRun   
```


## 📝 Dados de Entrada
## 👥 Módulo Cliente
**Criar Cliente**

Método HTTP: POST

Endpoint: /clientes

Dados de Entrada (JSON):

```bash

{
  "nome": "João Silva",
  "email": "joao.silva@example.com",
  "cpf": "123.456.789-09",
  "telefone": "11999999999",
  "dataNascimento": "1990-01-15"
}
```
**Buscar Cliente por ID**

Método HTTP: GET

Endpoint: /clientes/{iclienteId}

Dados de Entrada: O id do cliente a ser buscado.

**Atualizar Cliente**

Método HTTP: PUT

Endpoint: /clientes/{clienteId}

Dados de Entrada (JSON):

```bash
{
  "nome": "João Silva Atualizado",
  "email": "joao.atualizado@example.com",
  "cpf": "123.456.789-09",
  "telefone": "11888888888",
  "dataNascimento": "1990-01-15"
}
```
## 👨‍💼 Módulo Funcionário
**Criar Funcionário**

Método HTTP: POST

Endpoint: /funcionarios

Dados de Entrada (JSON):
```bash

{
  "nomeUsuario": "funcionario_teste",
  "email": "funcionario@empresa.com",
  "senha": "senha123"
}
```

**Buscar Funcionário por ID**

Método HTTP: GET

Endpoint: /funcionarios/{funcionarioId}

Dados de Entrada: O id do funcionário a ser buscado.

## 🏍️ Módulo Moto
**Criar Moto**

Método HTTP: POST

Endpoint: /motos

Dados de Entrada (JSON):
```bash

{
  "modelo": "Honda CB 500",
  "placa": "ABC1D23",
  "status": "Disponível",
  "setor": "bom"
}
```

**Buscar Moto por ID**

Método HTTP: GET

Endpoint: /motos/{notoid}

Dados de Entrada: O id da moto a ser buscada.

## 🅿️ Módulo Pátio
**Criar Pátio**

Método HTTP: POST

Endpoint: /patios

Dados de Entrada (JSON):
```bash
{
  "localizacao": "São Paulo - Centro",
  "quantidadeVagas": 50
}
```

**Buscar Pátio por ID**

Método HTTP: GET

Endpoint: /patios/{id}

Dados de Entrada: O id do pátio a ser buscado.

## ✅ Dados de Saída Esperados
## 👥 Módulo Cliente
**Criar Cliente**

Código de Status Esperado: 201 Created

Corpo da Resposta Esperado (JSON):
```bash

{
  "idCliente": 1,
  "nome": "João Silva",
  "email": "joao.silva@example.com",
  "cpf": "123.456.789-09",
  "telefone": "11999999999",
  "dataNascimento": "1990-01-15"
}
```

**Buscar Cliente por ID**

Código de Status Esperado: 200 OK

Corpo da Resposta Esperado (JSON):

```bash

{
  "idCliente": 1,
  "nome": "João Silva",
  "email": "joao.silva@example.com",
  "cpf": "123.456.789-09",
  "telefone": "11999999999",
  "dataNascimento": "1990-01-15"
}
```

## 👨‍💼 Módulo Funcionário
**Criar Funcionário**

Código de Status Esperado: 201 Created

Corpo da Resposta Esperado (JSON):
```bash

{
  "idFuncionario": 1,
  "nomeUsuario": "funcionario_teste",
  "email": "funcionario@empresa.com",
  "senha": "senha123"
}
```

## 🏍️ Módulo Moto
**Criar Moto**

Código de Status Esperado: 201 Created

Corpo da Resposta Esperado (JSON):

```bash

{
  "idMoto": 1,
  "modelo": "Honda CB 500",
  "placa": "ABC1D23",
  "status": "Disponível",
  "setor": "bom"
}
```

## 🅿️ Módulo Pátio
**Criar Pátio**

Código de Status Esperado: 201 Created

Corpo da Resposta Esperado (JSON):
```bash

{
  "idPatio": 1,
  "localizacao": "São Paulo - Centro",
  "quantidadeVagas": 50
}
```

## 🔍 Procedimento de Teste
**Configuração Inicial**

Inicie a API Spring Boot na porta 8080

Abra o Postman

Configure o Environment com variável baseUrl: http://localhost:8080

## 👥 Testes do Módulo Cliente
**Criar Cliente**

Selecione o método POST

Insira a URL: {{baseUrl}}/clientes

No corpo da requisição (raw JSON), insira os dados de entrada fornecidos

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide o corpo da resposta (deve conter o ID e os dados do cliente)

**Buscar Cliente por ID**

Selecione o método GET

Insira a URL: {{baseUrl}}/clientes/{clienteId}

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide o corpo da resposta (deve retornar os dados do cliente)

**Atualizar Cliente**

Selecione o método PUT

Insira a URL: {{baseUrl}}/clientes/{clienteId}

No corpo da requisição, insira os dados atualizados

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide se os dados foram atualizados corretamente

**Excluir Cliente**

Selecione o método DELETE

Insira a URL: {{baseUrl}}/clientes/{clienteId}

Clique em Send

Verifique se o código de status retornado é 200 OK

Confirme a exclusão tentando buscar o cliente novamente (deve retornar 404)

## 👨‍💼 Testes do Módulo Funcionário
Procedimento de Teste - Funcionário

**Criar Funcionário**

Selecione o método POST

Insira a URL: {{baseUrl}}/funcionarios

No corpo da requisição (raw JSON), insira os dados:

```bash

{
    "nomeUsuario": "funcionario_teste",
    "email": "funcionario@empresa.com",
    "senha": "senha123"
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide o corpo da resposta (deve conter o ID e os dados do funcionário)

Salve o ID retornado para uso nos próximos testes

**Listar Funcionários**

Selecione o método GET

Insira a URL: {{baseUrl}}/funcionarios

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide se a resposta contém array de funcionários com estrutura de paginação

**Buscar Funcionário por ID**

Selecione o método GET

Insira a URL: {{baseUrl}}/funcionarios/{funcionarioId} 

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide o corpo da resposta (deve retornar os dados do funcionário específico)

**Atualizar Funcionário**

Selecione o método PUT

Insira a URL: {{baseUrl}}/funcionarios/{funcionarioId}

No corpo da requisição, insira os dados atualizados:
```bash

{
    "nomeUsuario": "funcionario_atualizado",
    "email": "func.atualizado@empresa.com",
    "senha": "novasenha456"
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide se os dados foram atualizados corretamente

**Excluir Funcionário**

Selecione o método DELETE

Insira a URL: {{baseUrl}}/funcionarios/{funcionarioId}

Clique em Send

Verifique se o código de status retornado é 200 OK

Confirme a exclusão tentando buscar o funcionário novamente (deve retornar 404)

## 🏍️ Testes do Módulo Moto
Procedimento de Teste - Moto

**Criar Moto**

Selecione o método POST

Insira a URL: {{baseUrl}}/motos

No corpo da requisição (raw JSON), insira os dados:
```bash

{
    "modelo": "Honda CB 500",
    "placa": "ABC1323",
    "status": "Disponível",
    "setor": "Bom"
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide o corpo da resposta (deve conter o ID e os dados da moto)

Salve o ID retornado para uso nos próximos testes

**Listar Motos**

Selecione o método GET

Insira a URL: {{baseUrl}}/motos

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide se a resposta contém array de motos com estrutura de paginação

**Buscar Moto por ID**

Selecione o método GET

Insira a URL: {{baseUrl}}/motos/{motoId} 

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide o corpo da resposta (deve retornar os dados da moto específica)

**Atualizar Moto**

Selecione o método PUT

Insira a URL: {{baseUrl}}/motos/{motoId}

No corpo da requisição, insira os dados atualizados:

```bash

{
    "idMoto": 1,
    "modelo": "Honda PCX",
    "placa": "ABC1323",
    "status": "Disponível",
    "setor": "Bom"
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide se os dados foram atualizados corretamente

**Excluir Moto**

Selecione o método DELETE

Insira a URL: {{baseUrl}}/motos/{motoId}

Clique em Send

Verifique se o código de status retornado é 200 OK

Confirme a exclusão tentando buscar a moto novamente (deve retornar 404)

## 🅿️ Testes do Módulo Pátio
Procedimento de Teste - Pátio

**Criar Pátio**

Selecione o método POST

Insira a URL: {{baseUrl}}/patios

No corpo da requisição (raw JSON), insira os dados:

```bash

{
  "localizacao": "São Paulo - Centro",
  "quantidadeVagas": 50
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide o corpo da resposta (deve conter o ID e os dados do pátio)

Salve o ID retornado para uso nos próximos testes

**Listar Pátios**

Selecione o método GET

Insira a URL: {{baseUrl}}/patios

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide se a resposta contém array de pátios com estrutura de paginação

Buscar Pátio por ID

Selecione o método GET

Insira a URL: {{baseUrl}}/patios/{patioId} 

Clique em Send

Verifique se o código de status retornado é 200 OK

Valide o corpo da resposta (deve retornar os dados do pátio específico)

**Atualizar Pátio**

Selecione o método PUT

Insira a URL: {{baseUrl}}/patios/{patioId}

No corpo da requisição, insira os dados atualizados:
```bash

{
  "localizacao": "Rio de Janeiro - Copacabana",
  "quantidadeVagas": 30
}
```

Clique em Send

Verifique se o código de status retornado é 201 Created

Valide se os dados foram atualizados corretamente

**Excluir Pátio**

Selecione o método DELETE

Insira a URL: {{baseUrl}}/patios/{patioId}

Clique em Send

Verifique se o código de status retornado é 200 OK

Confirme a exclusão tentando buscar o pátio novamente (deve retornar 404)

## 🎯 Dicas para Execução Correta
**Ordem Recomendada de Testes:**

Testes de Criação (POST) - para gerar os IDs

Testes de Leitura (GET) - para validar os dados criados

Testes de Atualização (PUT) - para modificar os dados

Testes de Exclusão (DELETE) - para limpar os dados de teste

## 🎯 Resultados Obtidos
✅ 100% dos testes passando

✅ Cobertura completa dos endpoints CRUD

✅ Validações de negócio testadas

✅ Testes de erro e sucesso implementados

✅ 19 requisições automatizadas funcionando

## 🔗 Links da Entrega
Repositório GitHub: https://github.com/michellepotenza01/Challenge-QA-

Azure Boards: https://dev.azure.com/Challenge-QA-RM557702/Challenge-QA

Vídeo de Demonstração: 

--Pasta Postman com: .json da coleção de tests 

