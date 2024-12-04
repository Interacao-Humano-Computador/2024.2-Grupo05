## **Introdução**

O CD-MOJ, apesar de sua utilidade, apresenta desafios que afetam negativamente a experiência do usuário, como falta de feedback em tempo real, dificuldade na navegação e insuficiência de informações em submissões erradas. 

Para investigar esses problemas, aplicamos o modelo **GOMS (Goals, Operators, Methods, and Selection Rules)**, uma metodologia consagrada em estudos de interação humano-computador. O GOMS permite decompor as tarefas realizadas pelos usuários em objetivos, métodos e operações, detalhando as escolhas e ações cognitivas e físicas necessárias. A análise foi realizada com variações específicas do GOMS, como **KLM (Keystroke-Level Model)** e **CMN-GOMS**, para mapear os processos e propor melhorias fundamentadas.

## **Metodologia**

### **Modelo GOMS**

O modelo GOMS analisa as interações entre usuários e sistemas computacionais, estruturando as tarefas em objetivos, métodos, operadores e regras de seleção. Para esta análise, foram utilizadas as seguintes variações:

1. **KLM (Keystroke-Level Model)**:  
   Foco no tempo gasto em interações físicas, como pressionamento de teclas, cliques e navegação.
   
2. **CMN-GOMS (Cognitive Modeling Notation)**:  
   Modela as decisões do usuário com base em condições específicas, como feedback do sistema ou informações contextuais.

Esses métodos foram aplicados a quatro fluxos principais no CD-MOJ: **falta de feedback em tempo real**, **troca de senha**, **falta de mecanismos de busca e acesso a enunciados de competições passadas** e **ausência de informações em submissões erradas**. A análise incluiu a identificação de problemas, cálculo de tempos estimados e descrição das operações cognitivas e físicas realizadas pelos usuários.

### **Falta de feedback em tempo real durante a análise de submissões**

#### **KLM (Keystroke-Level Model)**

**Tabela 1:** KLM da Falta de feedback.

| **Etapa**                        | **Descrição**                                                 | **Tempo (segundos)** |
| -------------------------------- | ------------------------------------------------------------- | -------------------- |
| 1. Acessar plataforma            | Abrir o navegador e acessar o URL da plataforma CD-MOJ        | 2                    |
| 2. Submeter solução              | Preencher os campos e clicar em "Submeter"                    | 4                    |
| 3. Aguardar feedback             | Aguarda a resposta do sistema                                 | 20                   |
| 4. Recarregar página manualmente | Clicar para recarregar a página                               | 3                    |
| 5. Exibir resultado final        | O sistema exibe a resposta final ("Accepted", "Wrong Answer") | 2                    |
| **Total**                        |                                                               | **31 segundos**      |

#### **Modelagem do GOMS (CMN-GOMS)**

**Tabela 2:** CMN-GOMS Falta de feedback.

| **Objetivo**                              | **Método**                         | **Operador**         | **Seleção (Se)**                              |
| ----------------------------------------- | ---------------------------------- | -------------------- | --------------------------------------------- |
| Garantir feedback em tempo real           | Submeter solução                   | Clicar em "Submeter" | Se o sistema não responde, aguardar feedback  |
| Obter status da submissão                 | Verificar status na página         | Verificar            | Se não houver progresso, tentar recarregar    |
| Aguardar feedback e analisar progresso    | Observar as mensagens de progresso | Observar             | Se o sistema não mostra progresso, recarregar |
| Exibir resultado final ("Accepted", etc.) | Visualizar mensagem de resultado   | Observar             | Se resultado final não aparecer, recarregar   |

Neste modelo **CMN-GOMS**, o usuário decide se deve aguardar o feedback do sistema ou tentar recarregar a página caso não obtenha informações, levando em consideração a ausência de informações de progresso em tempo real.


### **Troca de senha do usuário**


#### **KLM (Keystroke-Level Model)**

**Tabela 3:** KLM da Troca de senha do usuário.

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

#### **Modelagem do GOMS (CMN-GOMS)**

**Tabela 4:** CMN-GOMS da Troca de senha do usuário.

| **Objetivo**          | **Método**                      | **Operador** | **Seleção (Se)**                                   |
| --------------------- | ------------------------------- | ------------ | -------------------------------------------------- |
| Trocar senha          | Localizar "Alterar Senha"       | Navegar      | Se opção não encontrada, tente outro menu          |
| Inserir a senha atual | Digitar senha atual             | Digitar      | Se senha atual incorreta, tente novamente          |
| Inserir nova senha    | Digitar nova senha              | Digitar      | Se senha simples, esperar erro, tentar senha forte |
| Confirmar alteração   | Clicar em "Confirmar"           | Clicar       | Se erro de validação, corrigir e tentar novamente  |
| Receber feedback      | Ver mensagem de sucesso ou erro | Verificar    | Se erro, voltar para ajustar a senha               |

Essa análise de GOMS no formato **CMN-GOMS** mostra uma sequência de decisões condicionais baseadas no que o usuário observa ou na situação em que se encontra, como a necessidade de ajustar a senha.

### **Problema com o FAQ**

#### **KLM (Keystroke-Level Model)**

**Tabela 5:** KLM do Problema com FAQ.

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

#### **Modelagem do GOMS (CMN-GOMS)**

**Tabela 6:** GMN-GOMS do Problema com FAQ.

| **Objetivo**                               | **Método**                 | **Operador**                | **Seleção (Se)**                                  |
| ------------------------------------------ | -------------------------- | --------------------------- | ------------------------------------------------- |
| Resolver o problema e entregar a atividade | Acessar FAQ ou Fórum       | Clicar no link ou pesquisar | Se FAQ não fornecer informações, buscar no fórum  |
| Compreender o erro "Time Limit Exceeded"   | Ler sobre o erro no fórum  | Observar                    | Se a informação for útil, aplicar a solução       |
| Enviar novamente a atividade               | Corrigir o erro e reenviar | Clicar em "Reenviar"        | Se o problema for resolvido, reenviar a atividade |

No **CMN-GOMS**, a decisão do usuário de buscar informações em fontes externas (fóruns) depende da falta de explicação adequada no FAQ. A solução ocorre após entender o erro e corrigir o envio da atividade.

### **Falta de mecanismos de busca e acesso a enunciados de competições passadas**

#### **KLM (Keystroke-Level Model)**

**Tabela 7:** KLM do Falta de mecanismos de busca.

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

#### **Modelagem do GOMS (CMN-GOMS)**

**Tabela 8:** CMN-GOMS do Falta de mecanismos de busca.

| **Objetivo**                     | **Método**                          | **Operador**                | **Seleção (Se)**                                                 |
| -------------------------------- | ----------------------------------- | --------------------------- | ---------------------------------------------------------------- |
| Acessar competições passadas     | Acessar a seção "Past"              | Clicar no link              | Se "Past" não estiver visível, rolar a página                    |
| Navegar por competições          | Encontrar a competição de interesse | Clicar entre as competições | Se a competição desejada for encontrada, selecione               |
| Acessar o enunciado das questões | Clicar para acessar o enunciado     | Clicar no link do enunciado | Se for necessário login externo, desistir ou buscar outro método |

No **CMN-GOMS**, a decisão do usuário de desistir ou buscar um método alternativo depende da percepção de que a plataforma não oferece as facilidades necessárias (como filtros de busca) e da frustração causada pelo login externo.

### **Ausência de informações em submissões erradas**

#### **KLM (Keystroke-Level Model)**

**Tabela 9:** KLM da Ausência de informações em submissões erradas.

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

#### **Modelagem do GOMS (CMN-GOMS)**

**Tabela 10:** CMN-GOMS da Ausência de informações em submissões erradas.

| **Objetivo**                     | **Método**                          | **Operador**               | **Seleção (Se)**                                                          |
| -------------------------------- | ----------------------------------- | -------------------------- | ------------------------------------------------------------------------- |
| Receber feedback sobre a solução | Enviar solução para a plataforma    | Submeter código            | Se "Wrong Answer" é exibido, proceder com a busca de novos casos de teste |
| Buscar mais casos de teste       | Procurar ajuda no Telegram          | Clicar no link do Telegram | Se o Mojinho responder, use os casos para corrigir o código               |
| Corrigir o código                | Ajustar a solução conforme feedback | Modificar o código         | Se os erros forem identificados, submeter a nova versão                   |

No **CMN-GOMS**, o usuário toma decisões baseadas nas mensagens recebidas da plataforma e no Mojinho. A escolha entre procurar mais casos de teste ou modificar o código é guiada pela necessidade de ajustar a solução para que ela passe nos testes.

## Bibliografia

BARBOSA, Simone Diniz Junqueira; DA SILVA, Bruno Santana. **Planejamento da avaliação de IHC**. In: INTERAÇÃO Humano-Computador. Rio de Janeiro: Elsevier Editora, 2010.

## Histórico de Versão

**Tabela 11:** Histórico de Versões.

| Versão |      Descrição       |                                              Autor(es)                                              |    Data    | Revisor(es) | Data de Revisão |
| :----: | :------------------: | :-------------------------------------------------------------------------------------------------: | :--------: | :---------: | :-------------: |
|  1.0   | Criação do documento | [Jéssica Eveline](https://github.com/xzxjesse), [Marcelo Adrian](https://github.com/Marcelo-Adrian) | 03/12/2024 |             |                 |