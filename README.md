# QA API Tests

Projeto de testes de API utilizando Postman.

## Cenários testados

### Login com sucesso
- Método: POST
- Endpoint: /api/login
- Esperado: 200 OK
- Validação: retorno de token

### Login com erro
- Método: POST
- Endpoint: /api/login
- Esperado: 400 Bad Request
- Validação: retorno de mensagem de erro

## Ferramentas
- Postman
- JSON

## Objetivo
Validar comportamento de APIs, garantindo respostas corretas para cenários de sucesso e erro.
