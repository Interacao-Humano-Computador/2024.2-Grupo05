# Análise de Tarefas

## **Introdução:**

Este trabalho analisa a usabilidade da plataforma CD-MOJ, identificando problemas e propondo melhorias para otimizar a experiência do usuário. Utilizando as metodologias HTA (Hierarchical Task Analysis) e GOMS (Goals, Operators, Methods, and Selection Rules), foi possível detalhar os processos de interação, abordando aspectos físicos e cognitivos das tarefas. 

## **Metodologia:**

A análise das tarefas foi realizada em duas etapas principais, utilizando as metodologias HTA e GOMS.

1. **HTA (Hierarchical Task Analysis):**
   - **Objetivo:** Compreender as etapas e subprocessos envolvidos nas tarefas realizadas pelos usuários.
   - **Procedimento:** Cada tarefa foi decomposta em subtarefas hierárquicas para identificar os passos sequenciais necessários. A análise envolveu a descrição do contexto, dos recursos e das interações dos usuários com o sistema em diferentes cenários.
   - **Ferramenta utilizada:** Diagramas de HTA e tabelas para representar a decomposição das tarefas e seus subprocessos.
2. **GOMS (Goals, Operators, Methods, and Selection Rules):**
   - **Objetivo:** Estudar os objetivos dos usuários e os métodos utilizados para alcançar esses objetivos, analisando as operações cognitivas e físicas envolvidas.
   - **Procedimento:** Para cada tarefa analisada, foram definidos os objetivos, as operações necessárias para alcançá-los, os métodos utilizados para executar as operações e as regras de seleção aplicadas em cada decisão. Foram utilizadas três variações do modelo GOMS:
     - **KLM (Keystroke-Level Model):** Para análise do tempo das interações com a interface.
     - **CTT (Cognitive Task Analysis):** Para avaliar os aspectos cognitivos e os desafios enfrentados pelos usuários ao executar as tarefas.
     - **CMN-GOMS e CPM-GOMS:** Para modelar os processos de decisão e a sequência de ações de maneira mais detalhada, considerando também a carga cognitiva.

A combinação dessas metodologias permitiu uma avaliação precisa dos processos realizados pelos usuários, identificando pontos críticos de interação e sugerindo melhorias baseadas em dados objetivos. As recomendações finais foram construídas com o intuito de tornar a plataforma mais intuitiva, eficiente e acessível, melhorando a experiência do usuário em cada um dos cenários analisados.

## Análise de Tarefas:

### Falta de feedback em tempo real durante a análise de submissões

### **1. HTA (Hierarchical Task Analysis)**

#### **Diagrama HTA:**

```plaintext
Tarefa Principal: Garantir feedback em tempo real durante a análise de submissões
|
|--- 1. O usuário acessa a plataforma CD-MOJ
|--- 2. O usuário submete sua solução para o problema
|    |
|    |--- 2.1 O sistema exibe status inicial "Not answered yet"
|    |--- 2.2 O usuário aguarda feedback
|--- 3. O usuário recarrega a página manualmente
|--- 4. O sistema exibe o resultado final ("Accepted", "Wrong Answer", etc.)
|--- 5. O usuário não recebe feedback sobre o progresso da análise
|--- 6. O sistema não fornece atualizações automáticas
|--- 7. O usuário se sente frustrado e desmotivado
```

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa central a ser alcançada, neste caso, garantir feedback em tempo real durante a análise de submissões.
- **Sub-tarefas**: Dividem o processo em etapas menores que devem ser realizadas para completar a tarefa principal.
- **Setas**: Indicam a sequência de execução das tarefas.

#### **Representação em Tabela (HTA)**

| **Número da Tarefa** | **Descrição da Tarefa**                                              | **Dependência** |
| -------------------- | -------------------------------------------------------------------- | --------------- |
| 1                    | O usuário acessa a plataforma CD-MOJ                                 | Nenhuma         |
| 2                    | O usuário submete sua solução para o problema                        | 1               |
| 2.1                  | O sistema exibe status inicial "Not answered yet"                    | 2               |
| 2.2                  | O usuário aguarda feedback                                           | 2.1             |
| 3                    | O usuário recarrega a página manualmente                             | 2.2             |
| 4                    | O sistema exibe o resultado final ("Accepted", "Wrong Answer", etc.) | 3               |
| 5                    | O usuário não recebe feedback sobre o progresso da análise           | 4               |
| 6                    | O sistema não fornece atualizações automáticas                       | 5               |
| 7                    | O usuário se sente frustrado e desmotivado                           | 6               |

### **2. GOMS (Goals, Operators, Methods, and Selection Rules)**

#### **KLM (Keystroke-Level Model)**

O **KLM** modela a tarefa com base nas interações físicas do usuário (como pressionamento de teclas, cliques e movimento do mouse).

| **Etapa**                        | **Descrição**                                                 | **Tempo (segundos)** |
| -------------------------------- | ------------------------------------------------------------- | -------------------- |
| 1. Acessar plataforma            | Abrir o navegador e acessar o URL da plataforma CD-MOJ        | 2                    |
| 2. Submeter solução              | Preencher os campos e clicar em "Submeter"                    | 4                    |
| 3. Aguardar feedback             | Aguarda a resposta do sistema                                 | 20                   |
| 4. Recarregar página manualmente | Clicar para recarregar a página                               | 3                    |
| 5. Exibir resultado final        | O sistema exibe a resposta final ("Accepted", "Wrong Answer") | 2                    |
| **Total**                        |                                                               | **31 segundos**      |

#### **CTT (Cognitive Task Analysis)**

O **CTT** foca nas necessidades cognitivas durante o processo de interação.

**Objetivo**: Garantir feedback em tempo real durante a análise de submissões.

**Tarefas**:

1. **Perception**: O usuário percebe que a solução foi submetida com sucesso, mas não há progresso visível.
2. **Memory**: O usuário lembra de que a plataforma deveria fornecer feedback em tempo real.
3. **Decision Making**: O usuário decide aguardar, mas fica frustrado com a falta de atualizações.
4. **Action**: O usuário recarrega manualmente a página para verificar o status da submissão.

**Subtarefas**:

- Aguardar feedback visual.
- Decidir se espera ou recarrega a página.
- Recarregar a página para ver se há alguma atualização.
- Verificar o status final da submissão.

**Considerações Cognitivas**:

- O usuário precisa perceber rapidamente que não está recebendo feedback em tempo real.
- A frustração pode aumentar se o tempo de espera for longo sem indicações claras de progresso.
- O sistema precisa fornecer informações claras sobre o progresso da análise para evitar a necessidade de recarregar a página manualmente.

#### **Modelagem do GOMS (CMN-GOMS)**

O **CMN-GOMS** expande o modelo de GOMS, incluindo decisões com base em situações específicas.

| **Objetivo**                              | **Método**                         | **Operador**         | **Seleção (Se)**                              |
| ----------------------------------------- | ---------------------------------- | -------------------- | --------------------------------------------- |
| Garantir feedback em tempo real           | Submeter solução                   | Clicar em "Submeter" | Se o sistema não responde, aguardar feedback  |
| Obter status da submissão                 | Verificar status na página         | Verificar            | Se não houver progresso, tentar recarregar    |
| Aguardar feedback e analisar progresso    | Observar as mensagens de progresso | Observar             | Se o sistema não mostra progresso, recarregar |
| Exibir resultado final ("Accepted", etc.) | Visualizar mensagem de resultado   | Observar             | Se resultado final não aparecer, recarregar   |

Neste modelo **CMN-GOMS**, o usuário decide se deve aguardar o feedback do sistema ou tentar recarregar a página caso não obtenha informações, levando em consideração a ausência de informações de progresso em tempo real.

### Troca de senha do usuário

### **1. HTA (Hierarchical Task Analysis)**

**Descrição do Diagrama HTA:**

O HTA divide o processo em tarefas hierárquicas e sub-tarefas, mostrando a relação entre as etapas para alcançar o objetivo principal.

#### **Diagrama HTA:**

```plaintext
Tarefa Principal: Trocar a senha da conta
|
|--- 1. Acessar o site do CD-MOJ
|--- 2. Navegar até o painel de configurações de conta
|    |
|    |--- 2.1 Localizar opção "Alterar Senha"
|    |--- 2.2 Clicar na opção "Alterar Senha"
|--- 3. Inserir a senha atual
|--- 4. Inserir a nova senha
|    |
|    |--- 4.1 Atentar-se aos critérios de segurança
|    |--- 4.2 Confirmar a nova senha
|--- 5. O sistema valida a senha
|    |
|    |--- 5.1 Se a senha for fraca, mostrar mensagem de erro
|    |--- 5.2 Se a senha for forte, confirmar alteração
|--- 6. Confirmar alteração de senha
```

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa central a ser alcançada, neste caso, "Trocar a senha da conta".
- **Sub-tarefas**: Dividem o processo em etapas menores que devem ser realizadas para completar a tarefa principal.
- **Setas**: Indicam a sequência de execução das tarefas, com tarefas dependentes.

#### **Representação em Tabela (HTA)**

| **Número da Tarefa** | **Descrição da Tarefa**                        | **Dependência** |
| -------------------- | ---------------------------------------------- | --------------- |
| 1                    | Acessar o site do CD-MOJ                       | Nenhuma         |
| 2                    | Navegar até o painel de configurações de conta | 1               |
| 2.1                  | Localizar opção "Alterar Senha"                | 2               |
| 2.2                  | Clicar na opção "Alterar Senha"                | 2.1             |
| 3                    | Inserir a senha atual                          | 2.2             |
| 4                    | Inserir a nova senha                           | 3               |
| 4.1                  | Atentar-se aos critérios de segurança          | 4               |
| 4.2                  | Confirmar a nova senha                         | 4.1             |
| 5                    | O sistema valida a senha                       | 4.2             |
| 5.1                  | Se a senha for fraca, mostrar mensagem de erro | 5               |
| 5.2                  | Se a senha for forte, confirmar alteração      | 5               |
| 6                    | Confirmar alteração de senha                   | 5.2             |

### **2. GOMS (Goals, Operators, Methods, and Selection Rules)**

A análise GOMS pode ser aplicada utilizando diferentes modelos, como **KLM**, **CMN-GOMS**, **CPM-GOMS**, e **CTT**. Para este caso, vamos modelar com o **KLM** (Keystroke-Level Model) e **CTT** (Cognitive Task Analysis).

#### **KLM (Keystroke-Level Model)**

O **KLM** modela a tarefa com base nas interações físicas do usuário (como pressionamento de teclas, cliques e movimento do mouse).

| **Etapa**                            | **Descrição**                                            | **Tempo (segundos)** |
| ------------------------------------ | -------------------------------------------------------- | -------------------- |
| 1. Acessar o site                    | Abrir o navegador e acessar a URL do site                | 2                    |
| 2. Navegar até configurações         | Clicar em menus e navegar para o painel de configurações | 4                    |
| 3. Localizar a opção "Alterar Senha" | Procurar pela opção de senha no painel                   | 6                    |
| 4. Clicar na opção                   | Clicar na opção "Alterar Senha"                          | 1                    |
| 5. Inserir senha atual               | Digitar a senha atual                                    | 3                    |
| 6. Inserir nova senha                | Digitar a nova senha                                     | 3                    |
| 7. Confirmar nova senha              | Digitar a confirmação da nova senha                      | 3                    |
| 8. Validação do sistema              | O sistema valida a senha                                 | 3                    |
| 9. Mensagem de erro (se necessário)  | Exibir mensagem de erro                                  | 4                    |
| 10. Confirmação de sucesso           | Exibir mensagem de sucesso                               | 3                    |
| **Total**                            |                                                          | **38 segundos**      |

#### **CTT (Cognitive Task Analysis)**

O **CTT** analisa as necessidades cognitivas para a realização de tarefas. Nesse modelo, podemos ver como o usuário processa a informação e toma decisões.

- **Goal**: Trocar a senha da conta.
- **Tasks**:
  - **Perception**: O usuário percebe o site e localiza a seção de configurações.
  - **Memory**: O usuário lembra da senha atual.
  - **Decision Making**: O usuário decide qual será a nova senha, levando em consideração os critérios de segurança.
  - **Action**: O usuário digita a senha atual, insere a nova senha e confirma.

**Subtarefas**:

- Encontrar o menu de configurações
- Localizar a opção de alteração de senha
- Especificar uma senha que atenda aos critérios
- Aguardar validação do sistema
- Caso haja erro, ajustar a senha e tentar novamente

**Considerações Cognitivas**:

- O usuário deve ter memória suficiente para lembrar a senha atual.
- O sistema precisa fornecer feedback claro sobre os critérios de senha e o status da validação.

#### **Modelagem do GOMS (CMN-GOMS)**

O **CMN-GOMS** expande o modelo de GOMS para incluir decisões baseadas em condições específicas.

| **Objetivo**          | **Método**                      | **Operador** | **Seleção (Se)**                                   |
| --------------------- | ------------------------------- | ------------ | -------------------------------------------------- |
| Trocar senha          | Localizar "Alterar Senha"       | Navegar      | Se opção não encontrada, tente outro menu          |
| Inserir a senha atual | Digitar senha atual             | Digitar      | Se senha atual incorreta, tente novamente          |
| Inserir nova senha    | Digitar nova senha              | Digitar      | Se senha simples, esperar erro, tentar senha forte |
| Confirmar alteração   | Clicar em "Confirmar"           | Clicar       | Se erro de validação, corrigir e tentar novamente  |
| Receber feedback      | Ver mensagem de sucesso ou erro | Verificar    | Se erro, voltar para ajustar a senha               |

Essa análise de GOMS no formato **CMN-GOMS** mostra uma sequência de decisões condicionais baseadas no que o usuário observa ou na situação em que se encontra, como a necessidade de ajustar a senha.

### Problema com o FAQ

### **1. HTA (Hierarchical Task Analysis)**

#### **Diagrama HTA:**

```plaintext
Tarefa Principal: Resolver o problema com o FAQ e entregar a atividade da disciplina
|
|--- 1. O usuário acessa o site do CD-MOJ
|--- 2. O usuário navega até o contest da disciplina cursada
|    |
|    |--- 2.1 O usuário acessa o contest
|    |--- 2.2 O usuário começa a analisar as questões
|    |--- 2.3 O usuário realiza as questões
|--- 3. O usuário se depara com o erro "Time Limit Exceeded, 0p"
|--- 4. O usuário percorre o FAQ do CD-MOJ
|--- 5. O usuário não encontra explicações sobre o problema
|--- 6. O usuário busca soluções em fóruns
|--- 7. O usuário compreende o que aconteceu e resolve o problema
|--- 8. O usuário reenvia sua atividade
```

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa principal a ser realizada é resolver o problema com o FAQ e entregar a atividade.
- **Sub-tarefas**: As tarefas que devem ser realizadas para completar a tarefa principal, divididas em etapas menores.
- **Setas**: Indicam a sequência de execução das tarefas.

#### **Representação em Tabela (HTA)**

| **Número da Tarefa** | **Descrição da Tarefa**                                   | **Dependência** |
| -------------------- | --------------------------------------------------------- | --------------- |
| 1                    | O usuário acessa o site do CD-MOJ                         | Nenhuma         |
| 2                    | O usuário navega até o contest da disciplina cursada      | 1               |
| 2.1                  | O usuário acessa o contest                                | 2               |
| 2.2                  | O usuário começa a analisar as questões                   | 2.1             |
| 2.3                  | O usuário realiza as questões                             | 2.2             |
| 3                    | O usuário se depara com o erro "Time Limit Exceeded, 0p"  | 2.3             |
| 4                    | O usuário percorre o FAQ do CD-MOJ                        | 3               |
| 5                    | O usuário não encontra explicações sobre o problema       | 4               |
| 6                    | O usuário busca soluções em fóruns                        | 5               |
| 7                    | O usuário compreende o que aconteceu e resolve o problema | 6               |
| 8                    | O usuário reenvia sua atividade                           | 7               |

### **2. GOMS (Goals, Operators, Methods, and Selection Rules)**

#### **KLM (Keystroke-Level Model)**

O **KLM** modela a tarefa com base nas interações físicas do usuário (como pressionamento de teclas, cliques e movimento do mouse).

| **Etapa**                  | **Descrição**                                  | **Tempo (segundos)** |
| -------------------------- | ---------------------------------------------- | -------------------- |
| 1. Acessar o site          | Abrir o navegador e acessar o URL do CD-MOJ    | 2                    |
| 2. Navegar até o contest   | Navegar até o contest da disciplina            | 5                    |
| 3. Acessar o contest       | Clicar no contest                              | 2                    |
| 4. Analisar as questões    | Ler as questões do contest                     | 5                    |
| 5. Realizar as questões    | Resolver as questões do contest                | 10                   |
| 6. Verificar erro          | Identificar o erro "Time Limit Exceeded, 0p"   | 2                    |
| 7. Acessar o FAQ           | Navegar até a seção de FAQ do CD-MOJ           | 5                    |
| 8. Buscar solução em fórum | Pesquisar sobre o erro no fórum                | 8                    |
| 9. Compreender o problema  | Ler a solução nos fóruns e entender a situação | 5                    |
| 10. Reenviar atividade     | Enviar novamente a atividade                   | 4                    |
| **Total**                  |                                                | **48 segundos**      |

#### **CTT (Cognitive Task Analysis)**

O **CTT** foca nas necessidades cognitivas durante o processo de interação.

**Objetivo**: Resolver o problema com o FAQ e entregar a atividade da disciplina.

**Tarefas**:

1. **Perception**: O usuário percebe que houve um erro durante o envio da atividade.
2. **Memory**: O usuário lembra da mensagem de erro ("Time Limit Exceeded, 0p").
3. **Decision Making**: O usuário decide investigar o erro utilizando o FAQ.
4. **Action**: O usuário tenta encontrar uma explicação para o erro no FAQ.
5. **Evaluation**: O usuário não encontra explicações no FAQ e decide buscar em fóruns.
6. **Action**: O usuário acessa os fóruns, lê sobre o problema e compreende o que aconteceu.
7. **Solution**: O usuário resolve o problema e reenvia sua atividade.

**Subtarefas**:

- Tentar entender a mensagem de erro.
- Buscar informações no FAQ.
- Buscar soluções em fóruns externos.
- Resolver o erro com base nas informações encontradas.
- Reenviar a atividade após a correção.

**Considerações Cognitivas**:

- O usuário deve ser capaz de identificar rapidamente o erro e decidir como proceder.
- A falta de informações claras no FAQ pode gerar frustração, obrigando o usuário a buscar alternativas (fóruns).
- O sistema deve melhorar a documentação para evitar que o usuário precise recorrer a fontes externas.

#### **Modelagem do GOMS (CMN-GOMS)**

O **CMN-GOMS** expande o modelo de GOMS, incluindo decisões com base em situações específicas.

| **Objetivo**                               | **Método**                 | **Operador**                | **Seleção (Se)**                                  |
| ------------------------------------------ | -------------------------- | --------------------------- | ------------------------------------------------- |
| Resolver o problema e entregar a atividade | Acessar FAQ ou Fórum       | Clicar no link ou pesquisar | Se FAQ não fornecer informações, buscar no fórum  |
| Compreender o erro "Time Limit Exceeded"   | Ler sobre o erro no fórum  | Observar                    | Se a informação for útil, aplicar a solução       |
| Enviar novamente a atividade               | Corrigir o erro e reenviar | Clicar em "Reenviar"        | Se o problema for resolvido, reenviar a atividade |

No **CMN-GOMS**, a decisão do usuário de buscar informações em fontes externas (fóruns) depende da falta de explicação adequada no FAQ. A solução ocorre após entender o erro e corrigir o envio da atividade.

### Falta de mecanismos de busca e acesso a enunciados de competições passadas

### **1. HTA (Hierarchical Task Analysis)**

#### **Diagrama HTA:**

```plaintext
Tarefa Principal: Revisitar competições passadas no CD-MOJ para estudar e se preparar para futuros contests
|
|--- 1. O usuário acessa a plataforma CD-MOJ
|--- 2. O usuário navega até a seção "Past"
|    |
|    |--- 2.1 O usuário encontra a página de competições passadas
|    |--- 2.2 O usuário nota a falta de mecanismos de busca ou filtros
|    |--- 2.3 O usuário navega manualmente por vários minutos
|--- 3. O usuário encontra a competição de interesse
|--- 4. O usuário tenta acessar o enunciado das questões
|--- 5. O usuário descobre que é necessário login externo para acessar o enunciado
|--- 6. O usuário se frustra e desiste da plataforma
```

#### **Legenda do Diagrama:**

- **Tarefa Principal**: O objetivo principal é revisar competições passadas no CD-MOJ para se preparar para futuros contests.
- **Sub-tarefas**: As etapas menores que o usuário deve seguir para completar a tarefa principal.
- **Setas**: Indicando a sequência de atividades a serem realizadas.

#### **Representação em Tabela (HTA)**

| **Número da Tarefa** | **Descrição da Tarefa**                                                    | **Dependência** |
| -------------------- | -------------------------------------------------------------------------- | --------------- |
| 1                    | O usuário acessa a plataforma CD-MOJ                                       | Nenhuma         |
| 2                    | O usuário navega até a seção "Past"                                        | 1               |
| 2.1                  | O usuário encontra a página de competições passadas                        | 2               |
| 2.2                  | O usuário nota a falta de mecanismos de busca ou filtros                   | 2.1             |
| 2.3                  | O usuário navega manualmente por vários minutos                            | 2.2             |
| 3                    | O usuário encontra a competição de interesse                               | 2.3             |
| 4                    | O usuário tenta acessar o enunciado das questões                           | 3               |
| 5                    | O usuário descobre que é necessário login externo para acessar o enunciado | 4               |
| 6                    | O usuário se frustra e desiste da plataforma                               | 5               |

---

### **2. GOMS (Goals, Operators, Methods, and Selection Rules)**

#### **KLM (Keystroke-Level Model)**

O **KLM** modela a tarefa com base em interações físicas, como pressionamento de teclas, cliques e movimento do mouse.

| **Etapa**                                  | **Descrição**                                                | **Tempo (segundos)** |
| ------------------------------------------ | ------------------------------------------------------------ | -------------------- |
| 1. Acessar a plataforma                    | Abrir o navegador e acessar o URL do CD-MOJ                  | 2                    |
| 2. Navegar até a seção "Past"              | Clicar no link da seção "Past"                               | 3                    |
| 3. Encontrar a página de competições       | Rolar a página ou clicar para encontrar competições passadas | 5                    |
| 4. Notar a falta de filtros e busca        | Perceber que a navegação é feita manualmente                 | 2                    |
| 5. Navegar manualmente                     | Clicar para navegar entre as competições passadas            | 10                   |
| 6. Encontrar a competição de interesse     | Identificar a competição desejada                            | 5                    |
| 7. Tentar acessar o enunciado das questões | Clicar para acessar o enunciado da competição                | 3                    |
| 8. Descobrir a necessidade de login        | Perceber que é necessário login externo                      | 2                    |
| 9. Frustração e desistência                | Desistir de continuar a navegação devido à burocracia        | 5                    |
| **Total**                                  |                                                              | **37 segundos**      |

#### **CTT (Cognitive Task Analysis)**

O **CTT** foca nas necessidades cognitivas e decisões durante o processo de interação.

**Objetivo**: Revisitar competições passadas no CD-MOJ para estudar e se preparar para futuros contests.

**Tarefas**:

1. **Perception**: O usuário percebe que deseja revisar competições passadas.
2. **Memory**: O usuário lembra que a plataforma CD-MOJ possui competições passadas que ele pode acessar.
3. **Decision Making**: O usuário decide acessar a seção "Past" da plataforma para encontrar competições passadas.
4. **Action**: O usuário clica para acessar as competições passadas, mas percebe que a página não possui filtros de busca.
5. **Evaluation**: O usuário decide navegar manualmente por várias competições.
6. **Action**: O usuário encontra a competição de interesse, mas descobre que precisa de um login externo (com um professor ou bot do Telegram) para acessar o enunciado.
7. **Solution**: O usuário se sente frustrado e desiste de utilizar a plataforma para esse fim.

**Considerações Cognitivas**:

- A falta de filtros ou mecanismos de busca aumenta a carga cognitiva do usuário, que precisa navegar manualmente.
- A descoberta da necessidade de login externo (com um professor ou bot) gera frustração e desmotiva o usuário a continuar.
- O design da plataforma não facilita a navegação eficiente e o acesso ao conteúdo.

#### **Modelagem do GOMS (CMN-GOMS)**

O **CMN-GOMS** expande o modelo de GOMS, incluindo decisões baseadas em condições específicas.

| **Objetivo**                     | **Método**                          | **Operador**                | **Seleção (Se)**                                                 |
| -------------------------------- | ----------------------------------- | --------------------------- | ---------------------------------------------------------------- |
| Acessar competições passadas     | Acessar a seção "Past"              | Clicar no link              | Se "Past" não estiver visível, rolar a página                    |
| Navegar por competições          | Encontrar a competição de interesse | Clicar entre as competições | Se a competição desejada for encontrada, selecione               |
| Acessar o enunciado das questões | Clicar para acessar o enunciado     | Clicar no link do enunciado | Se for necessário login externo, desistir ou buscar outro método |

No **CMN-GOMS**, a decisão do usuário de desistir ou buscar um método alternativo depende da percepção de que a plataforma não oferece as facilidades necessárias (como filtros de busca) e da frustração causada pelo login externo.

### Ausência de informações em submissões erradas

### **1. HTA (Hierarchical Task Analysis)**

#### **Diagrama HTA:**

```plaintext
Tarefa Principal: Encontrar casos de teste que gerem erros no algoritmo para análise
|
|--- 1. O usuário acessa a plataforma CD-MOJ
|--- 2. O usuário envia sua solução da atividade
|--- 3. O usuário recebe a mensagem "Wrong Answer 50p"
|--- 4. O usuário procura outros conjuntos de entradas e saídas diferentes dos fornecidos
|--- 5. O usuário entra em contato com o Mojinho pelo Telegram
|--- 6. O usuário recebe outros conjuntos de entradas e saídas para testar sua solução
|--- 7. O usuário identifica os casos em que seu código apresenta defeitos e faz as correções
```

#### **Legenda do Diagrama:**

- **Tarefa Principal**: O objetivo é encontrar os casos de teste que geram erros no algoritmo para análise e correção.
- **Sub-tarefas**: São as etapas que o usuário segue para completar a tarefa.
- **Setas**: Indicam a sequência das ações.

#### **Representação em Tabela (HTA)**

| **Número da Tarefa** | **Descrição da Tarefa**                                                      | **Dependência** |
| -------------------- | ---------------------------------------------------------------------------- | --------------- |
| 1                    | O usuário acessa a plataforma CD-MOJ                                         | Nenhuma         |
| 2                    | O usuário envia sua solução da atividade                                     | 1               |
| 3                    | O usuário recebe a mensagem "Wrong Answer 50p"                               | 2               |
| 4                    | O usuário procura outros conjuntos de entradas e saídas                      | 3               |
| 5                    | O usuário entra em contato com o Mojinho pelo Telegram                       | 4               |
| 6                    | O usuário recebe outros conjuntos de entradas e saídas para testar a solução | 5               |
| 7                    | O usuário identifica os casos de erro e faz as correções no código           | 6               |

---

### **2. GOMS (Goals, Operators, Methods, and Selection Rules)**

#### **KLM (Keystroke-Level Model)**

O **KLM** modela a tarefa com base nas interações do usuário com o sistema, considerando os tempos de ações como pressionamento de teclas e cliques.

| **Etapa**                                | **Descrição**                                                | **Tempo (segundos)** |
| ---------------------------------------- | ------------------------------------------------------------ | -------------------- |
| 1. Acessar a plataforma                  | Abrir o navegador e acessar a plataforma CD-MOJ              | 2                    |
| 2. Enviar a solução                      | Submeter o código na plataforma                              | 3                    |
| 3. Receber mensagem "Wrong Answer"       | O sistema exibe a mensagem "Wrong Answer 50p"                | 2                    |
| 4. Procurar outros conjuntos de entradas | Buscar em outros lugares os conjuntos de entradas e saídas   | 5                    |
| 5. Entrar em contato com o Mojinho       | Clicar no link do Telegram para falar com o Mojinho          | 4                    |
| 6. Receber conjuntos de testes           | Aguardar a resposta com os casos de teste fornecidos         | 5                    |
| 7. Identificar erros e corrigir o código | Testar os novos casos de teste e corrigir os erros no código | 10                   |
| **Total**                                |                                                              | **31 segundos**      |

#### **CTT (Cognitive Task Analysis)**

O **CTT** foca nos aspectos cognitivos, como a memória e as decisões feitas durante a execução da tarefa.

**Objetivo**: Encontrar os casos de teste que geram erros no algoritmo para análise e correção.

**Tarefas**:

1. **Perception**: O usuário percebe que sua solução não foi aceita e que a plataforma retornou a mensagem "Wrong Answer".
2. **Memory**: O usuário lembra que a plataforma fornece apenas exemplos de entrada e saída, e começa a procurar por mais casos de teste.
3. **Decision Making**: O usuário decide buscar ajuda no Telegram com o Mojinho para obter mais casos de teste.
4. **Action**: O usuário entra em contato com o Mojinho e aguarda a resposta com mais dados de entrada e saída.
5. **Evaluation**: O usuário identifica os erros no código ao testar os novos casos de teste recebidos e faz as correções necessárias.
6. **Solution**: O usuário submete novamente sua solução, agora corrigida.

**Considerações Cognitivas**:

- A falta de informações sobre os testes pode gerar frustração no usuário, que precisa buscar externamente por casos de entrada e saída.
- A interação com o Mojinho requer a capacidade de lembrar onde obter a ajuda necessária (Telegram).
- O processo de identificar o erro no código exige concentração e análise detalhada dos casos de teste.

#### **Modelagem do GOMS (CMN-GOMS)**

No **CMN-GOMS**, decisões são tomadas com base em condições específicas. O modelo inclui a escolha entre alternativas, como buscar ajuda no Telegram ou corrigir o código diretamente.

| **Objetivo**                     | **Método**                          | **Operador**               | **Seleção (Se)**                                                          |
| -------------------------------- | ----------------------------------- | -------------------------- | ------------------------------------------------------------------------- |
| Receber feedback sobre a solução | Enviar solução para a plataforma    | Submeter código            | Se "Wrong Answer" é exibido, proceder com a busca de novos casos de teste |
| Buscar mais casos de teste       | Procurar ajuda no Telegram          | Clicar no link do Telegram | Se o Mojinho responder, use os casos para corrigir o código               |
| Corrigir o código                | Ajustar a solução conforme feedback | Modificar o código         | Se os erros forem identificados, submeter a nova versão                   |

No **CMN-GOMS**, o usuário toma decisões baseadas nas mensagens recebidas da plataforma e no Mojinho. A escolha entre procurar mais casos de teste ou modificar o código é guiada pela necessidade de ajustar a solução para que ela passe nos testes.

## **Conclusão:**

A análise das tarefas relacionadas à navegação na plataforma CD-MOJ e ao processo de correção de soluções evidenciou pontos críticos que afetam diretamente a experiência do usuário. A falta de filtros e mecanismos de busca adequados dificulta a localização de competições passadas, aumentando a carga cognitiva e a frustração. Além disso, a ausência de feedback claro nas submissões erradas, especialmente no que se refere a entradas e saídas de testes, impede que o usuário compreenda rapidamente os erros e corrija seu código de forma eficiente. A necessidade de recorrer a aplicativos externos, como o Telegram para obter mais casos de teste, adiciona uma camada de complexidade e aumenta o tempo de resolução dos problemas.

## **Recomendações:**

- **Implementação de filtros e mecanismos de busca** para facilitar a navegação e localização de competições passadas.
- **Melhoria no feedback das submissões**, fornecendo informações detalhadas sobre os casos de teste falhos, incluindo entradas e saídas esperadas.
- **Facilidade de acesso direto aos casos de teste** sem a necessidade de recorrer a plataformas externas.
- **Facilitação do acesso aos enunciados das questões**, removendo a dependência de login externo.
- **Melhoria na visibilidade e clareza do fluxo de navegação** para a troca de senha, incluindo uma exibição clara dos critérios de segurança para a nova senha e mensagens de erro informativas que orientem o usuário em caso de falhas.

Com essas melhorias, o CD-MOJ pode proporcionar uma experiência mais eficiente, intuitiva e menos frustrante para os usuários, melhorando a navegação e a correção de soluções. Isso permitirá que os estudantes se concentrem mais no aprendizado e preparação para competições, tornando a plataforma mais útil e acessível.

## Histórico de Versão

| Versão |      Descrição       |                                              Autor(es)                                              |    Data    | Revisor(es) | Data de Revisão |
| :----: | :------------------: | :-------------------------------------------------------------------------------------------------: | :--------: | :---------: | :-------------: |
|  1.0   | Criação do documento | [Jéssica Eveline](https://github.com/xzxjesse), [Marcelo Adrian](https://github.com/Marcelo-Adrian) | 03/12/2024 |             |                 |
