**Cadastro de usuários - Testes API**

Este repositório tem 2 exemplos de testes de API para **cadastro de usuários**, usando **Postman**:
1. **Teste simples**: validações básicas de CRUD.
2. **Teste robusto**: versão avançada, com validações de campos, status code e testes negativos.
<br>
<br>

1.**Teste simples** 

**Testes positivos:**
  * Cria usuário (POST)
  * Lista usuários (GET)
  * Atualiza usuário (PUT)
  * Deleta usuário (DELETE)

**Testes negativos:**
* Busca usuário inexistente
* Cria usuário sem body
* Atualiza com dados inválidos
 <br>
 <br>
 
2.**Teste robusto**

**Testes positivos:**
  * CRUD completo com validação detalhada dos campos
  * Valida formato de e-mail e existência de ID

**Testes negativos:**
  * Usuário inexistente espera 404
  * Cria sem body validação de status
  * Atualiza com dados inválidos validação de status
 <br>
 <br>
 
**Ordem recomendada para os testes**

**Teste positivo (CRUD)**
1. Cria usuário (POST)
2. Lista usuários (GET)
3. Atualiza usuário (PUT)
4. Deleta usuário (DELETE)

**Teste negativo**
1. Cria usuário sem body (POST)
2. Busca usuário inexistente (GET espera 404)
3. Atualiza com dados inválidos (PUT valida status)
 <br>
 <br>
 
**Detalhes dos testes**
* **Teste Simples:** valida apenas status code e presença de dados.
* **Teste Robusto:** valida status code, campos do usuário, formato de e-mail, ID retornado e inclui tratamento de respostas negativas.
 <br>
 <br>

**_Observação:_**
JSONPlaceholder é apenas uma API de teste, então alguns comportamentos podem não refletir APIs reais (ex.: criar usuário retorna sempre um ID simulado).

