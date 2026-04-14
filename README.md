**Cadastro de usuários - Testes API**

Este repositório tem 2 exemplos de testes de API para **cadastro de usuários**, usando **Postman**:
1. **Teste simples**: validações básicas de CRUD.
2. **Teste robusto**: versão avançada, com validações de campos, status code, e testes negativos.


**Teste simples**

|**Testes positivos**
  * Criar Usuário (POST)
  * Listar Usuários (GET)
  * Atualizar Usuário (PUT)
  * Deletar Usuário (DELETE)
 
**Testes negativos:**
    * Buscar usuário inexistente
    * Criar usuário sem body
    * Atualizar com dados inválidos

**Teste robusto**

**Testes positivos**
  * CRUD completo com validação detalhada dos campos
  * Valida formato de e-mail e existência de ID
  * Testes Negativos robustos, incluindo:

**Testes negativos:**
  * Usuário inexistente → espera 404
  * Criar sem body → validação de status
  * Atualizar com dados inválidos → validação de status

**Ordem recomendada para os testes**

**Teste positivo (CRUD)**
1. Criar Usuário (POST)
2. Listar Usuários (GET)
3. Atualizar Usuário (PUT)
4. Deletar Usuário (DELETE)

**Teste negativo**
1. Criar usuário sem body (POST)
2. Buscar usuário inexistente (GET → espera 404)
3. Atualizar com dados inválidos (PUT → valida status)

**Detalhes dos testes**
* **Teste Simples:** valida apenas status code e presença de dados.
* **Teste Robusto:** valida status code, campos do usuário, formato de e-mail, ID retornado, e inclui tratamento de respostas negativas.

*Observações*
* JSONPlaceholder é **apenas uma API de teste**, então alguns comportamentos podem não refletir APIs reais (ex.: criar usuário retorna sempre um ID simulado).

