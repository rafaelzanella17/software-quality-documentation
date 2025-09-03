# Naming Convention (Padrão de Nomenclatura)

## Definição
**Naming Convention** é um conjunto de regras e padrões utilizados para nomear branches, commits e outros artefatos de desenvolvimento, garantindo organização, clareza e rastreabilidade no projeto.  

Adotar convenções padronizadas facilita o entendimento entre membros do time, reduz confusões e melhora a comunicação entre desenvolvimento e QA.

---

## Padrão para Branches

Os nomes das branches devem indicar claramente o tipo de trabalho que está sendo realizado e o escopo da funcionalidade ou correção.  

**Exemplos de tipos de branches:**

| Tipo       | Finalidade                            | Exemplo                                       |
|------------|---------------------------------------|-----------------------------------------------|
| feature/ ou feat/  | Novas funcionalidades              | `feature/user-authentication-system`         |
| fix/ ou bugfix/    | Correção de bugs                   | `fix/login-validation-error`                 |
| hotfix/            | Correções urgentes em produção     | `hotfix/payment-gateway-crash`               |
| docs/              | Documentação                       | `docs/update-readme`                         |
| refactor/          | Refatoração de código              | `refactor/user-service-module`               |
| test/              | Testes                             | `test/cypress-login-flow`                    |
| chore/             | Tarefas de manutenção              | `chore/update-dependencies`                  |
| style/             | Formatação ou estilos              | `style/navbar-css`                           |
| perf/              | Melhorias de performance           | `perf/database-query-optimization`           |

**Exemplo de criação de branch e commit:**
```bash
git checkout -b feature/user-registration-system
git commit -m "feat: criar formulário de cadastro de novos usuários"

git checkout -b docs/user-registration
git commit -m "docs: adicionar documentação do fluxo de cadastro de usuários"

git checkout -b test/cypress-user-registration
git commit -m "test: criar teste de fluxo de cadastro de usuários"

git checkout -b docs/rename-bug-report
git commit -m "docs(fundamentos): renomear bug-report de 170 para 180"

git checkout -b refactor/git-naming-convention
git commit -m "refactor(boas-praticas): refatoração do arquivo git-naming-convention"