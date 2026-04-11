**API de Teste Rafaela - Collection Postman**

Este repositório contém uma **Collection do Postman** para praticar testes de API com CRUD completo e testes negativos usando a API pública **JSONPlaceholder**.

**A Collection possui:**
- **CRUD completo**: Create (POST), Read (GET), Update (PUT), Delete (DELETE).
- **Testes positivos**: validação de status code e campos retornados.  
- **Testes negativos**: validação de erros e comportamentos inesperados.  
- **Environment configurável**: para URL base e IDs de usuário.


**Ordem recomendada de execução dos testes**
**Testes Positivos (CRUD)**
1. **Criar Usuário (POST)** – valida criação e campos retornados.  
2. **Listar Usuários (GET)** – verifica se o usuário criado aparece na lista.  
3. **Atualizar Usuário (PUT)** – altera dados do usuário e valida resposta.  
4. **Deletar Usuário (DELETE)** – remove o usuário criado.  


**Testes Negativos**
1. **Criar sem Body (POST)** – testa resposta da API quando o body está vazio.  
2. **Buscar usuário inexistente (GET)** – verifica comportamento ao buscar ID inexistente.  
3. **Atualizar com dados inválidos (PUT)** – testa se a API rejeita dados incorretos (em JSONPlaceholder, aceita qualquer dado).


