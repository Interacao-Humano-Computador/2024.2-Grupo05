# Introdução

# Objetivo

# Metodologia

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

Autor(es): [Ruan Carvalho](https://github.com/Ruan-Carvalho), 2024.


## Referências Bibliográficas

## Histórico de Versão
| Versão | Descrição | Autor(es) | Data | Revisor(es) | Data de Revisão |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1.0 | Criação do documento | [Jéssica Eveline](https://github.com/xzxjesse), [Marcelo Adrian](https://github.com/Marcelo-Adrian), [Ruan Carvalho](https://github.com/Ruan-Carvalho) | 24/11/2024 |  |  |
