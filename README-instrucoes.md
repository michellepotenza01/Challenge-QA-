# Instruções para Execução dos Testes Automatizados com Postman 
(Readme principal com todas as informações do projeto de Java e dos test realizados no README.md)

## Introdução

Este documento contém as instruções para a execução dos testes automatizados desenvolvidos para o sistema **Mottu**. A coleção de testes foi criada no **Postman** e tem como objetivo validar os principais endpoints da API REST do sistema.

## Pré-requisitos

Antes de executar os testes, certifique-se de que você tem o seguinte:

1. **Postman** instalado em sua máquina. Caso não tenha, baixe e instale o Postman [aqui](https://www.postman.com/downloads/).
2. A variável de ambiente `baseUrl` configurada no Postman para apontar para o seu servidor de teste. O valor de `baseUrl` deve ser a URL onde a API está sendo executada (exemplo: `http://localhost:8080`).

## Como Executar a Coleção de Testes no Postman

### 1. Baixe o arquivo da coleção de testes

A coleção de testes foi exportada no formato `.json`. Você pode **baixar o arquivo** da coleção de testes **aqui**:

- [Challenge Mottu – QA.postman_collection.json](Postman/Challenge%20Mottu%20%E2%80%93%20QA.postman_collection.json)

### 2. Importe a Coleção para o Postman

1. Abra o **Postman**.
2. Clique no botão **Import** (geralmente no canto superior esquerdo).
3. Selecione a opção **Upload Files**.
4. Navegue até o arquivo `.json` que você baixou (o arquivo `Challenge Mottu – QA.postman_collection.json`).
5. Clique em **Open** para importar a coleção no Postman.

### 3. Configure a variável de ambiente `baseUrl`

1. No **Postman**, clique no ícone de **engrenagem** no canto superior direito (ao lado de **Environment**).
2. Selecione **Manage Environments** e crie uma nova variável de ambiente chamada `baseUrl`.
3. Defina o valor da variável `baseUrl` para a URL da API (por exemplo, `http://localhost:8080`).
4. Salve a configuração da variável de ambiente.

### 4. Execute os Testes Usando o **Postman Runner**

1. Rode a aplicação de Java com: 
```bash
.\gradlew BootRun
```   
No **Postman**, vá até a **coleção** de testes que você importou.
2. Clique na **seta verde** ao lado da coleção e selecione **Run** para abrir o **Collection Runner**.
3. No Collection Runner, certifique-se de que a variável de ambiente `baseUrl` está selecionada.
4. Clique em **Run** para executar todos os testes da coleção.

Os testes irão ser executados automaticamente, e você verá o status de cada um no **Collection Runner**. O resultado incluirá os status dos testes (passando ou falhando), além das respostas da API para cada endpoint.

## Detalhes dos Testes

A coleção de testes contém os seguintes tipos de requisição:

### 1. **POST** - Criação de recursos (Cliente, Funcionário, Moto, Pátio)
- Valida a criação de novos registros na API.
- Testa se o status retornado é 201 (Created) e se a resposta contém as propriedades corretas.

### 2. **GET** - Consultas de recursos (Cliente, Funcionário, Moto, Pátio)
- Valida a listagem e a consulta de recursos específicos por ID.
- Testa se a resposta tem o status 200 (OK) e se os dados estão corretos.

### 3. **PUT** - Atualização de recursos
- Valida a atualização de recursos existentes.
- Testa se o status retornado é 200 ou 201 e se os dados são atualizados corretamente.

### 4. **DELETE** - Exclusão de recursos
- Valida a exclusão de recursos.
- Testa se o status retornado é 200 ou 204 e se o recurso é removido corretamente.

## Resultados Esperados

Os testes devem retornar os seguintes resultados esperados para cada tipo de requisição:

- **POST (Criação)**: Status 201, com os dados do recurso criado.
- **GET (Consulta)**: Status 200, com os dados do recurso correto.
- **PUT (Atualização)**: Status 200 ou 201, com os dados atualizados.
- **DELETE (Exclusão)**: Status 200 ou 204, e verificação de que o recurso foi excluído com sucesso (tentando buscar o recurso após a exclusão deve retornar 404).

## Conclusão

Após executar a coleção no Postman, você terá uma visão clara do status de todos os testes automatizados. Se algum teste falhar, o Postman mostrará o erro detalhado para que você possa investigar o problema.

