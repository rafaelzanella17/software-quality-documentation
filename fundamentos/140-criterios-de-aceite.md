# Critérios de Aceite

Os **Critérios de Aceite** são condições objetivas e testáveis que definem quando uma História de Usuário pode ser considerada concluída.  
Eles traduzem requisitos e regras de negócio em **condições verificáveis**, garantindo que a funcionalidade atenda exatamente ao que foi solicitado.  

- São a principal base para a criação dos **cenários de teste**.  
- Costumam ser escritos em formato simples ou com sintaxe **Gherkin** (Dado, Quando, Então), para facilitar a automatização.  

---

### Exemplo: Cadastro de Novo Usuário

**Requisito:**  
O sistema deve permitir o cadastro de novos usuários.  

**Regras de Negócio:**  
- O e-mail deve ser único.  
- A senha deve ter no mínimo 8 caracteres e conter letras e números.  
- A confirmação de senha deve ser idêntica à senha informada.  

---

### Critérios de Aceite (em formato de cenários)

**Cenário 1: Cadastro com sucesso**  
> **Dado** que eu estou na página de cadastro  
> **E** preencho todos os campos obrigatórios corretamente  
> **Quando** eu clico no botão "Cadastrar"  
> **Então** o sistema deve redirecionar para a tela de login  
> **E** exibir a mensagem "Cadastro realizado com sucesso!"  

---

**Cenário 2: Tentativa de cadastro com e-mail já existente**  
> **Dado** que o e-mail "usuario.existente@email.com" já está cadastrado  
> **Quando** eu tento cadastrar um novo usuário com esse mesmo e-mail  
> **Então** o sistema deve exibir a mensagem "Este e-mail já está em uso."  

---

**Cenário 3: Tentativa de cadastro com senhas que não conferem**  
> **Dado** que eu estou na página de cadastro  
> **Quando** eu informo "Senha@123" e "Senha@456" nos campos de senha e confirmação  
> **Então** o sistema deve exibir a mensagem "As senhas não conferem."  

---

### Critérios de Aceite (sem formato de cenários)

**Requisito:**  
O sistema deve permitir o cadastro de novos usuários.  

**Critérios de Aceite:**  
- O sistema deve salvar corretamente os dados de um novo usuário quando todos os campos obrigatórios forem preenchidos de forma válida.  
- Após o cadastro bem-sucedido, o sistema deve redirecionar o usuário para a tela de login e exibir a mensagem **"Cadastro realizado com sucesso!"**.  
- O sistema não deve permitir o cadastro de um e-mail já existente e deve exibir a mensagem **"Este e-mail já está em uso."**.  
- A senha deve atender aos requisitos mínimos (no mínimo 8 caracteres, contendo letras e números).  
- A confirmação de senha deve ser obrigatória e idêntica à senha informada. Caso contrário, deve ser exibida a mensagem **"As senhas não conferem."**.  
