# 6. Procedimento de Teste (Test Procedure)

O **Procedimento de Teste** especifica a sequência de execução de múltiplos casos de teste para validar um cenário de ponta a ponta (end-to-end).

---

### Exemplo: Ciclo de Vida do Usuário

**ID:** PT01
**Título:** Validar o ciclo de vida do usuário: Cadastro, Login e Logout.
**Sequência de Execução:**
1.  **Executar TC001:** Cadastro com sucesso do usuário `contato@emailvalido.com`.
2.  **Executar TC-LOGIN-001:** Login com sucesso usando as credenciais recém-criadas.
3.  **Executar TC-LOGOUT-001:** Logout da sessão do usuário.