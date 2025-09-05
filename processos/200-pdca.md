# Método PDCA (Plan, Do, Check, Act)

O **PDCA** é um ciclo de melhoria contínua usado para identificar problemas, analisar dados e propor soluções.  
Ele é muito aplicado em **qualidade de software**, mas também pode ser usado em qualquer processo dentro de uma empresa.

---

### Por que usar o PDCA?

Não basta dizer **"isso não funciona"**.  
Quando alguém pergunta **"como podemos melhorar?"**, é necessário ter **dados do processo atual** e uma **proposta de solução**.  
O PDCA organiza esse raciocínio em quatro etapas.

---

### Exemplo prático aplicado ao ciclo PDCA

#### Problema identificado
A execução dos testes manuais de regressão está levando **5 dias completos** antes de cada release, atrasando entregas.

---

#### 1. Plan (Planejar)
- Coletar dados: tempo médio de execução dos testes = 5 dias.  
- Impacto: atraso de 2 dias em média nas entregas para produção.  
- Objetivo: reduzir a execução de regressão para **2 dias ou menos**.  
- Plano: introduzir automação nos cenários mais críticos.

---

#### 2. Do (Executar)
- Implementar automação dos testes de login, cadastro e checkout.  
- Executar esses testes de forma integrada no pipeline da aplicação.  

---

#### 3. Check (Verificar)
- Nova medição: regressão completa passou de 5 dias para **2 dias e meio**.  
- Conclusão: houve redução de 50%, mas a meta de 2 dias ainda não foi atingida.  

---

#### 4. Act (Agir / Ajustar)
- Expandir a automação para os cenários restantes de maior impacto.  
- Padronizar o uso da automação em todo o time de QA.  
- Reiniciar o ciclo medindo novamente o tempo após os ajustes.

---

### Benefícios do PDCA

- **Para a empresa:** entregas mais rápidas e redução de atrasos.  
- **Para você:** experiência prática, credibilidade e portfólio baseado em dados.  

---

### Outras metodologias e modelos relacionados

- **PDCA** Ciclo de melhoria contínua.  
- **TMMi (Test Maturity Model Integration)** Modelo de maturidade em testes.  
- **TPI Next (Test Process Improvement Next)** Modelo de melhoria de processo de teste.  
- **CTP (Critical Testing Processes)** → Guia de processos críticos de teste.  
- **STEP (Systematic Test and Evaluation Process)** Processo sistemático de teste e avaliação.  
- **AIMA (Automated Intelligent Management of Testing Activities)** Modelo focado em automação e gestão inteligente de atividades de teste.  

---

### Referências

- [PDCA – Wikipédia](https://pt.wikipedia.org/wiki/Ciclo_PDCA)  
- Júlio de Lima em:  https://www.youtube.com/live/fisnJDlqA8E
