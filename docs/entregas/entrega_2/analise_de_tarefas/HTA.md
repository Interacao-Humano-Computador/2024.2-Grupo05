## Introdução

Utilizando a metodologia **HTA (Hierarchical Task Analysis)**, as interações dos usuários com o sistema foram detalhadas, abordando os processos físicos e cognitivos associados às tarefas. A análise baseia-se em princípios de interação humano-computador, que destacam a importância de compreender o contexto de uso, as características humanas e os objetivos dos usuários para desenvolver sistemas mais eficientes e acessíveis. Este trabalho segue uma abordagem sistemática para decompor as tarefas em etapas hierárquicas, promovendo uma visão clara dos processos de interação e suas falhas.

## Metodologia

A análise foi conduzida exclusivamente com a metodologia HTA, alinhada às boas práticas da interação humano-computador, que enfatizam a compreensão do contexto e as características dos usuários para propor soluções centradas neles. 

**HTA (Hierarchical Task Analysis):**

   - **Objetivo:** Identificar e estruturar as etapas e subprocessos que compõem as principais interações dos usuários na plataforma CD-MOJ.
   - **Procedimento:** Cada tarefa foi decomposta em etapas hierárquicas, conectadas por relações de sequência, seleção ou paralelismo.

### **Falta de feedback em tempo real durante a análise de submissões**

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

Autor(es): [Felipe Rodrigues](https://github.com/felipeJRdev), 2024.

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa central a ser alcançada, neste caso, garantir feedback em tempo real durante a análise de submissões.
- **Sub-tarefas**: Dividem o processo em etapas menores que devem ser realizadas para completar a tarefa principal.
- **Setas**: Indicam a sequência de execução das tarefas.

#### **Representação em Tabela (HTA)**

**Tabela 1:** Tabela HTA Falta de feedback.

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

Autor(es): [Felipe Rodrigues](https://github.com/felipeJRdev), 2024.

### **Troca de senha do usuário**

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

Autor(es): [Jéssica Eveline](https://github.com/xzxjesse), 2024.

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa central a ser alcançada, neste caso, "Trocar a senha da conta".
- **Sub-tarefas**: Dividem o processo em etapas menores que devem ser realizadas para completar a tarefa principal.
- **Setas**: Indicam a sequência de execução das tarefas, com tarefas dependentes.

#### **Representação em Tabela (HTA)**

**Tabela 2:** Tabela HTA Troca de senha.

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

Autor(es): [Jéssica Eveline](https://github.com/xzxjesse), 2024.

### **Problema com o FAQ**

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

Autor(es): [João Vitor Santos](https://github.com/Jauzimm), 2024.

#### **Legenda do Diagrama:**

- **Tarefa Principal**: A tarefa principal a ser realizada é resolver o problema com o FAQ e entregar a atividade.
- **Sub-tarefas**: As tarefas que devem ser realizadas para completar a tarefa principal, divididas em etapas menores.
- **Setas**: Indicam a sequência de execução das tarefas.

#### **Representação em Tabela (HTA)**

**Tabela 3:** Tabela HTA Problema com o FAQ.

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

Autor(es): [João Vitor Santos](https://github.com/Jauzimm), 2024.

### **Falta de mecanismos de busca e acesso a enunciados de competições passadas**

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

Autor(es): [Marcelo Adrian](https://github.com/Marcelo-Adrian), 2024.

#### **Legenda do Diagrama:**

- **Tarefa Principal**: O objetivo principal é revisar competições passadas no CD-MOJ para se preparar para futuros contests.
- **Sub-tarefas**: As etapas menores que o usuário deve seguir para completar a tarefa principal.
- **Setas**: Indicando a sequência de atividades a serem realizadas.

#### **Representação em Tabela (HTA)**

**Tabela 4:** Tabela HTA Falta de mecanismos de busca.

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

Autor(es): [Marcelo Adrian](https://github.com/Marcelo-Adrian), 2024.

### **Ausência de informações em submissões erradas**

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

Autor(es): [Ruan Carvalho](https://github.com/Ruan-Carvalho), 2024.

#### **Legenda do Diagrama:**

- **Tarefa Principal**: O objetivo é encontrar os casos de teste que geram erros no algoritmo para análise e correção.
- **Sub-tarefas**: São as etapas que o usuário segue para completar a tarefa.
- **Setas**: Indicam a sequência das ações.

#### **Representação em Tabela (HTA)**

**Tabela 5:** Tabela HTA Ausência de informações.

| **Número da Tarefa** | **Descrição da Tarefa**                                                      | **Dependência** |
| -------------------- | ---------------------------------------------------------------------------- | --------------- |
| 1                    | O usuário acessa a plataforma CD-MOJ                                         | Nenhuma         |
| 2                    | O usuário envia sua solução da atividade                                     | 1               |
| 3                    | O usuário recebe a mensagem "Wrong Answer 50p"                               | 2               |
| 4                    | O usuário procura outros conjuntos de entradas e saídas                      | 3               |
| 5                    | O usuário entra em contato com o Mojinho pelo Telegram                       | 4               |
| 6                    | O usuário recebe outros conjuntos de entradas e saídas para testar a solução | 5               |
| 7                    | O usuário identifica os casos de erro e faz as correções no código           | 6               |

Autor(es): [Ruan Carvalho](https://github.com/Ruan-Carvalho), 2024.

## Bibliografia

BARBOSA, Simone Diniz Junqueira; DA SILVA, Bruno Santana. **Planejamento da avaliação de IHC**. In: INTERAÇÃO Humano-Computador. Rio de Janeiro: Elsevier Editora, 2010.

## Histórico de Versão

**Tabela 6:** Histórico de versões.

| Versão |      Descrição       |                                              Autor(es)                                              |    Data    | Revisor(es) | Data de Revisão |
| :----: | :------------------: | :-------------------------------------------------------------------------------------------------: | :--------: | :---------: | :-------------: |
|  1.0   | Criação do documento | [Felipe Rodrigues](https://github.com/felipeJRdev), [Jéssica Eveline](https://github.com/xzxjesse), [João Vitor](https://github.com/Jauzimm), [Ruan Carvalho](https://github.com/Ruan-Carvalho), [Marcelo Adrian](https://github.com/Marcelo-Adrian)| 03/12/2024 |      [Felipe Rodrigues](https://github.com/felipeJRdev), [Jéssica Eveline](https://github.com/xzxjesse), [João Vitor](https://github.com/Jauzimm), [Ruan Carvalho](https://github.com/Ruan-Carvalho), [Marcelo Adrian](https://github.com/Marcelo-Adrian)       |        03/12/2024         |
