# Casos de Teste (Test Cases)

Os **Casos de Teste** descrevem de forma estruturada **como validar uma condição de teste**, especificando pré-condições, passos, dados de entrada e resultados esperados.  
Eles são fundamentais para garantir que o requisito e os critérios de aceite foram implementados corretamente.  

Existem diferentes níveis de detalhamento:

---

## Casos de Teste de Alto Nível

- Também chamados de **testes abstratos**.  
- Descrevem **o que deve ser testado**, mas não entram em detalhes técnicos ou passo a passo.  
- São úteis para revisões rápidas com o cliente, Product Owner ou equipe de negócio.  

**Exemplo (Cadastro de Usuário):**  
- Validar que o sistema permite o cadastro de um novo usuário.  
- Validar que o sistema não permite cadastro com e-mail duplicado.  
- Validar que o sistema exige senha forte.  

---

## Casos de Teste de Baixo Nível

- Também chamados de **testes detalhados**.  
- Incluem informações completas sobre **pré-condições, dados de entrada, passos, resultados esperados** e podem ser usados diretamente por QAs para execução manual ou automatizada.  
- São úteis para garantir padronização e rastreabilidade.  

**Exemplo (Cadastro de Usuário - Baixo Nível):**  

---

### Caso de Teste Completo

**ID:** CT-001  
**Título:** Cadastro de usuário com sucesso  
**Requisito Relacionado:** O sistema deve permitir o cadastro de novos usuários.  
**Prioridade:** Alta  
**Pré-condições:**  
- O usuário não deve estar logado no sistema.  
- O e-mail utilizado não deve existir na base de dados.  

**Dados de Entrada:**  
- Nome: Rafael Zanella  
- E-mail: rafael.teste@email.com  
- Senha: Senha@123  
- Confirmação de Senha: Senha@123  

**Passos para Execução:**  
1. Acessar a página de cadastro de usuário.  
2. Preencher o campo "Nome" com "Rafael Zanella".  
3. Preencher o campo "E-mail" com "rafael.teste@email.com".  
4. Preencher o campo "Senha" com "Senha@123".  
5. Preencher o campo "Confirmação de Senha" com "Senha@123".  
6. Clicar no botão "Cadastrar".  

**Resultado Esperado:**  
- O sistema deve redirecionar o usuário para a tela de login.  
- Exibir a mensagem: **"Cadastro realizado com sucesso!"**  

---

### Outros Exemplos de Casos de Teste (em baixo nível)

**ID:** CT-002  
**Título:** Cadastro com e-mail já existente  
**Resultado Esperado:** O sistema deve exibir a mensagem: **"Este e-mail já está em uso."**  

**ID:** CT-003  
**Título:** Cadastro com senhas divergentes  
**Resultado Esperado:** O sistema deve exibir a mensagem: **"As senhas não conferem."**  

---
