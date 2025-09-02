# Bug Report

Os **Bug Reports** são documentos que descrevem **problemas encontrados no sistema** durante a execução de testes.  
Eles devem ser claros, objetivos e completos para que a equipe de desenvolvimento consiga reproduzir e corrigir o defeito.

---

## Estrutura de um Bug Report

Um Bug Report típico contém:

- **ID:** Identificador único do bug.  
- **Título:** Descrição curta e objetiva do problema.  
- **Descrição:** Explicação detalhada do bug, contexto e impacto.  
- **Passos para Reproduzir:** Passo a passo para que qualquer pessoa consiga reproduzir o bug.  
- **Resultado Esperado:** Comportamento correto que deveria ocorrer.  
- **Resultado Atual:** Comportamento observado que indica o bug.  
- **Gravidade/Prioridade:** Nível de impacto do bug.  
- **Ambiente:** Informações sobre sistema, navegador, versão, etc.  
- **Anexos/Evidências:** Prints, vídeos, logs ou links que comprovem o bug.

---

## Exemplo de Bug Report

**ID:** BUG-001  
**Título:** Erro ao cadastrar usuário com e-mail válido  

**Descrição:**  
Ao tentar cadastrar um novo usuário com um e-mail válido que ainda não está na base de dados, o sistema retorna uma mensagem de erro genérica e não realiza o cadastro.  
Impacto: impede novos usuários de se registrarem no sistema, bloqueando o fluxo de onboarding.

**Passos para Reproduzir:**  
1. Acessar a página de cadastro de usuário.  
2. Preencher o campo "Nome" com "Rafael Zanella".  
3. Preencher o campo "E-mail" com "novo.usuario@email.com".  
4. Preencher o campo "Senha" com "Senha@123".  
5. Preencher o campo "Confirmação de Senha" com "Senha@123".  
6. Clicar no botão "Cadastrar".  

**Resultado Esperado:**  
- O sistema deve redirecionar o usuário para a tela de login.  
- Exibir a mensagem: **"Cadastro realizado com sucesso!"**  

**Resultado Atual:**  
- O sistema exibe a mensagem: **"Erro ao processar solicitação."**  
- O usuário não é cadastrado.  

**Gravidade/Prioridade:** Alta  

**Ambiente:**  
- Sistema: Web  
- Navegador: Google Chrome 116.0  
- Sistema Operacional: Windows 11  

**Anexos/Evidências:**  
- Print da mensagem de erro (erro_cadastro_usuario.png)  
