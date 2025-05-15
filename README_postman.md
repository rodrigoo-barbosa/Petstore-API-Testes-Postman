
# Testes de API - Swagger Petstore (Postman) 💻📬

Este projeto contém 5 testes criados no **Postman** para validar a API pública da **Swagger Petstore**. Os testes foram exportados em formato `.postman_collection.json` e podem ser importados em qualquer ambiente Postman para execução manual ou automatizada.

## Casos de Teste Implementados 

### 🟡 1. Cadastrar Novo Pet (Médodo: **POST** /pet)
- **Objetivo:** Verificar se é possível cadastrar um novo pet com ID, nome e status definidos.
- **Corpo da Requisição:**
```json
{
  "id": 123456,
  "name": "Caramelo",
  "status": "Disponível"
}
```
- **Validação Esperada:** Status 200 e retorno dos dados enviados.

---

### 🟢 2. Buscar Pet por ID (Médodo: **GET** /pet/{petId})
- **Objetivo:** Garantir que um pet cadastrado possa ser consultado diretamente pelo ID.
- **URL de exemplo:** `/pet/123456`
- **Validação Esperada:** Status 200 com os dados do pet retornados.

---

### 🔵 3. Atualizar Pet (Médodo: **PUT** /pet)
- **Objetivo:** Validar a atualização dos dados de um pet existente.
- **Corpo da Requisição:**
```json
{
  "id": 123456,
  "name": "Caramelo Atualizado",
  "status": "Adotado"
}
```
- **Validação Esperada:** Status 200 com dados atualizados corretamente.

---

### 🔴 4. Deletar Pet (Médodo: **DELETE** /pet/{petId})
- **Objetivo:** Confirmar a exclusão de um pet do sistema.
- **URL de exemplo:** `/pet/123456`
- **Validações Esperadas:**
  - Status 200 no DELETE
  - Status 404 ao tentar buscar o mesmo ID após exclusão

---

### 🟢 5. Buscar Pets por Status (Médodo: **GET** /pet/findByStatus**)
- **Parâmetro:** `?status=available`
- **Objetivo:** Listar todos os pets com status "available".
- **Validação Esperada:** Status 200 com lista de pets (não vazia).

---

## 📥 Como importar no Postman 

1. Abra o Postman
2. Clique em **Import**
3. Selecione o arquivo `Petstore API Tests.postman_collection.json`
4. Clique em **Importar** para visualizar e executar os testes

---

## 🔗 Acessar coleção Postman diretamente via guest link 

https://rodrigobarbosa-4953199.postman.co/workspace/Rodrigo-Barbosa's-Workspace~e40be582-f58b-494e-86a0-74f6e284d651/collection/44933145-63bb94ea-3aee-483b-99e5-212d078a0751?action=share&creator=44933145

## Ferramentas Utilizadas
- Postman
- JSON
- API Swagger Petstore (https://petstore.swagger.io)

## 📁 Arquivos do projeto
- `Petstore API Tests.postman_collection.json`: Collection com todos os testes
- `README.md`: Documentação do projeto

---

## ✍️ Autor
Desenvolvido por Rodrigo Barbosa
