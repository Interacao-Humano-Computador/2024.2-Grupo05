# Introdução

Este documento faz parte do desenvolvimento de cenários no âmbito da disciplina de Interação Humano-Computador (IHC), com foco na análise de problemas de usabilidade enfrentados por usuários do CD-MOJ. O objetivo é explorar questões críticas de interação, propor melhorias e, assim, promover uma experiência mais intuitiva e acessível para diferentes perfis de usuários.

# Objetivo

O principal objetivo deste documento é identificar e documentar cenários de uso que evidenciem problemas de usabilidade na plataforma. Esses cenários foram elaborados para compreender como os usuários interagem com o sistema, identificar barreiras e propor soluções que aprimorem a experiência do usuário, alinhando-se aos princípios de design centrado no usuário.

# Metodologia

Para a criação dos cenários, foi utilizada uma abordagem baseada no framework DECIDE, que orienta a análise de usabilidade e coleta de dados para avaliar e propor melhorias em sistemas interativos. O processo seguiu as seguintes etapas:

**1 - Identificação de problemas:**
Foram analisados pontos de frustração e desafios enfrentados pelos usuários do CD-MOJ, como a ausência de feedback em tempo real, dificuldade na troca de senha e falta de mecanismos de busca para competições passadas.

**2 - Coleta de dados:**
A análise foi embasada em observações, relatos de usuários e estudos prévios sobre boas práticas de design para plataformas de juízes online.

**3 - Criação dos cenários:**
Cada cenário foi elaborado detalhando elementos como contexto, objetivos, atores, episódios, restrições e exceções. Essa estrutura permite visualizar as interações dos usuários com a plataforma e identificar lacunas de usabilidade.

# Cénarios

### Falta de feedback em tempo real durante a análise de submissões  

| *Elemento*   | *Descrição* |
| -------------- | ------------- |
| *Objetivo*   | Garantir que o usuário receba feedback claro e em tempo real durante a análise de submissões. |
| *Contexto*   | - *Local:* Participando de uma competição, em casa. <br> - *Tempo:* Durante a submissão de soluções para problemas no CD-MOJ. <br> - *Pré-condições:* Ter acesso à internet, estar logado na plataforma, e ter submetido uma solução válida. |
| *Recursos*   | - Conexão à internet <br> - Computador ou dispositivo com acesso à plataforma CD-MOJ <br> - Sistema de submissões do CD-MOJ funcionando corretamente. |
| *Ator*       | Usuários da plataforma, especialmente programadores iniciantes como o usuário. |
| *Episódios*  | - O usuário participa de uma competição e resolve um problema. <br> - Ele submete sua solução através da interface da plataforma. <br> - O sistema exibe o status inicial "Not answered yet". <br> - O usuário aguarda feedback, mas a página não atualiza automaticamente. <br> - Após alguns minutos, ele recarrega manualmente a página. <br> - Somente após o reload, o sistema exibe o resultado final ("Accepted", "Wrong Answer", etc.). <br> - O usuário não recebe informações sobre o progresso da análise, como a quantidade de casos de teste que foram processados. <br> - A falta de feedback em tempo real deixa o usuário frustrado e desmotivado. |
| *Restrições* | - O sistema deve fornecer atualizações automáticas durante a análise de submissões. <br> - O feedback deve ser claro, indicando progresso (por exemplo, quantidade de casos de teste processados). <br> - Mensagens informativas devem estar disponíveis em caso de problemas técnicos. |
| *Exceção*    | - Problemas no servidor impedem o processamento das submissões. <br> - Falha no sistema de notificações em tempo real. <br> - Perda de conexão à internet durante o processo de submissão. <br> - Submissão inválida devido a erros no código ou formato do arquivo. |

Autor(es): [Felipe Rodrigues](https://github.com/felipeJRdev), 2024.

### Troca de senha do usuário

| *Elemento*   | *Descrição* |
| -------------- | ------------- |
| *Objetivo*   | Alterar a senha da conta para aumentar a segurança pessoal. |
| *Contexto*   | - *Local:* Casa ou qualquer ambiente seguro com acesso à internet. <br> - *Tempo:* Após assistir à palestra sobre segurança digital. <br> - *Pré-condições:* Ter acesso à internet, estar logada na conta CDMOJ, e possuir a senha atual da conta. |
| *Recursos*   | - Conexão à internet <br> - Dispositivo com navegador (notebook, smartphone, etc.) <br> - Plataforma CD-MOJ com suporte à troca de senha. |
| *Ator*       | Usuários cadastrados na plataforma CD-MOJ. |
| *Episódios*  | - O usuário acessa o site do CD-MOJ em seu notebook. <br> - Ela navega até o painel de configurações de conta. <br> - O usuário tem dificuldade em localizar a opção "Alterar Senha", que está posicionada de forma pouco visível. <br> - Após encontrar a funcionalidade, ela insere a senha atual, a nova senha e a confirmação da nova senha. <br> - O sistema não informa os critérios para a nova senha. <br> - O usuário tenta usar uma senha simples e recebe uma mensagem de erro genérica. <br> - Depois de várias tentativas e ajustes, o usuário consegue definir uma senha forte. <br> - O sistema confirma a alteração com uma mensagem de sucesso. |
| *Restrições* | - Fluxo de navegação intuitivo para encontrar a funcionalidade de troca de senha. <br> - Exibição clara dos critérios necessários para a nova senha. <br> - Mensagens de erro informativas e orientadoras. |
| *Exceção*    | - O usuário não se lembra da senha atual. <br> - O sistema não valida corretamente os critérios de segurança da senha. <br> - Falta de conexão à internet durante o processo. <br> - Problemas técnicos na plataforma impedem a alteração da senha. |

Autor(es): [Jéssica Eveline](https://github.com/xzxjesse), 2024.

| *Elemento*   | *Descrição* |
| -------------- | ------------- |
| *Objetivo*   | Realizar e entregar as atividades da disciplina. |
| *Contexto*   | - *Local:* No quarto <br> - *Tempo:* Após chegar da faculdade <br> - *Pré-condições:* Ter acesso à internet, possuir computador e estar logada na conta CDMOJ |
| *Recursos*   | - Conexão à internet <br> - Dispositivo com navegador (notebook, desktop, smartphone, etc.) <br> - Acesso a plataforma CD-MOJ |
| *Ator*       | Usuários que iram realizar atividades de uma disciplina |
| *Episódios*  | - O usuário acessa o site do CD-MOJ. <br> - Ele navega no site até achar o contest da disciplina cursada. <br> - O usuário acessa o contest. <br> - Ele começa a analisar as questões e as realiza. <br> - O usuário se depara com um problema durante o envio do código: "Time Limit Exceeded, 0p" <br> - O usuario percorre pelo FAQ do CD-MOJ para compreender a mensagem. <br> - Ele não encontra explicações sobre o problema. <br> - Ele busca em fóruns a respeito do problema. <br> - O usuário compreende o que aconteceu e reenvia sua atividade. |
| *Restrições* | - O site deve expandir sua documentação sobre problemas frequentemente enfrentados. |
| *Exceção*    | - Problemas de autenticação. <br> - O dispósitivo eletrônico apresenta problemas.  <br> - Falta de conexão à internet durante o processo. <br> - Plataforma fora do ar. |

Autor(es): [João Vitor Santos](https://github.com/Jauzimm), 2024.

### Falta de mecanismos de busca e acesso a enunciados de competições passadas

| **Elemento**   | **Descrição** |
|-----------------|---------------|
| *Objetivo*    | Revisitar competições passadas no CD MOJ para estudar e se preparar para futuros contests. |
| *Contexto*    | - **Local:** Casa, laboratório ou outro local com acesso à internet. <br> - **Tempo:** Durante o planejamento de estudos ou momentos de revisão. <br> - **Pré-condições:** A plataforma deve ter registros de competições passadas, e o usuário deve ter acesso à internet. |
| *Recursos*    | - Conexão à internet <br> - Dispositivo com navegador (computador ou smartphone) <br> - Plataforma CD MOJ com histórico de competições passadas. |
| *Ator*        | Estudantes que busca material de estudo e revisão para contests. |
| *Episódios*   | - O usuário acessa a plataforma CD MOJ. <br> - Ele navega até a seção "Past". <br> - Nota que a página não possui mecanismos de busca ou filtros, dificultando a localização da competição desejada. <br> - Após navegar manualmente por vários minutos, encontra a competição de interesse. <br> - Tenta acessar o enunciado das questões, mas descobre que precisa de autorização externa (login com um professor ou um bot no telegram). <br> - Frustrado com a burocracia, desiste de utilizar a plataforma para este propósito. |
| *Restrições*  | - A página deve permitir acesso direto ao conteúdo das competições. <br> - Necessidade de implementar mecanismos de busca e filtros para facilitar a navegação. |
| *Exceção*     | - A plataforma não possui registros de competições passadas. <br> - O usuário não encontra as competições específicas de seu interesse. <br> - Problemas de autenticação ou indisponibilidade de login com professores. <br> - Falta de conexão à internet. |

Autor(es): [Marcelo Adrian](https://github.com/Marcelo-Adrian), 2024.

### Ausência de informações em submissões erradas

| **Elemento**   | **Descrição** |
|-----------------|---------------|
| *Objetivo*    | Encontar casos de teste que gerem erros no algorítmo para análise |
| *Contexto*    | - **Local:** Casa, laboratório ou outro local com acesso à internet. <br> - **Tempo:** Durante o prazo da lista de exercícios. <br> - **Pré-condições:** Ter acesso à internet, estar logado na plataforma, e ter submetido uma solução parcialmente correta. |
| *Recursos*    | - Conexão à internet <br> - Dispositivo com navegador (computador ou smartphone) <br> - Plataforma CD MOJ aceitando submissões corretamente. |
| *Ator*        | Estudante com problemas em sua solução. |
| *Episódios*   | - O usuário acessa a plataforma CD MOJ. <br> - Ele envia sua solução da atividade. <br> - Recebe a mensagem "Wrong Answer 50p". <br> - Procura outros conjuntos de entradas e saídas diferente dos fornecidos no enunciado. <br> - Entra em contato com o Mojinho pelo Telegram. <br> - Recebe outros conjuntos de entradas e saídas utilizados para testar sua solução. <br> - Identifica os casos em que seu código apresenta defeitos e faz as correções |
| *Restrições*  | - Falta de informações que orientem os estudantes a entregar suas soluções de forma correta. <br> - Uso de aplicativo externo para encontrar outros casos de testes. |
| *Exceção*     | - Instabilidade nos servidores do CD-MOJ. <br> - O usuário entrega sua solução correta na primeira tentativa. <br> - Problemas com o mojinho ou Telegram. <br> - Falta de conexão à internet. |

Autor(es): [Ruan Carvalho](https://github.com/Ruan-Carvalho), 2024.


## Referências Bibliográficas

## Histórico de Versão
| Versão | Descrição | Autor(es) | Data | Revisor(es) | Data de Revisão |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1.0 | Criação do documento | [Jéssica Eveline](https://github.com/xzxjesse), [Marcelo Adrian](https://github.com/Marcelo-Adrian), [Ruan Carvalho](https://github.com/Ruan-Carvalho) | 24/11/2024 |  |  |
