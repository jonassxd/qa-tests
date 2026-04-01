# 🧪 QA API Collection - Jonas

[![Postman](https://img.shields.io/badge/Postman-Collection-orange?logo=postman)](https://www.postman.com/) 
[![Status](https://img.shields.io/badge/Status-Active-brightgreen)]  

**Collection de testes de API para Postman** — completa com cenários positivos e negativos, pronta para demonstrar **QA manual e automatizado**.

## 🚀 Sobre a Collection

Esta coleção utiliza a API [ReqRes](https://reqres.in/) para simular cenários comuns de teste de APIs:

| Endpoint | Método | Testes Automatizados |
|----------|--------|--------------------|
| 💚 Login - Sucesso | POST | Status 200, token existe |
| 🔴 Login - Erro | POST | Status 400, mensagem de erro existe |
| 💙 Lista de Usuários | GET | Status 200, lista não vazia, email existe |
| ⚫ Usuário Inexistente | GET | Status 404 / data null |

Inclui testes positivos e negativos, validação de respostas, tokens e integridade de dados.

## ⚙️ Pré-requisitos

- [Postman](https://www.postman.com/downloads/) instalado  
- Conexão com a internet  
- JSON da Collection: [`QA_API_Collection.json`](./QA_API_Collection.json)  

## 📂 Como usar

1. Abra o **Postman**  
2. Clique em **Import → Upload Files → selecione `QA_API_Collection.json`**  
3. Crie um **Environment** com a variável `auth_token` (deixe vazio, será preenchido após login)  
4. Execute **Login - Sucesso** primeiro para gerar o token  
5. Copie o token retornado e coloque na variável `auth_token` do Environment  
6. Execute os demais endpoints manualmente  

⚠️ Para evitar erros 401, faça login antes de executar endpoints que exigem token.

## 🧪 Testes Automatizados Incluídos

- ✅ Status Code  
- ✅ Token existe  
- ✅ Lista de usuários não vazia  
- ✅ Email do usuário existe  
- ✅ Usuário inexistente (data null)  
- ✅ Mensagem de erro em login inválido  

## 🔗 Referências

- [ReqRes API Docs](https://reqres.in/)  
- [Postman Learning Center](https://learning.postman.com/)  
- [Allure Reports](https://docs.qameta.io/allure/) para relatórios automáticos  

## 📝 Observações

- Todos os testes estão configurados para rodar no Postman  
- Collection pronta para demonstrar habilidades em QA manual e automatizado  
- Variável do Environment: `auth_token`
