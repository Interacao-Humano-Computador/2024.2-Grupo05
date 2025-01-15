# Relato de Resultados do Protótipo de Papel

## Tarefa: Falta de Feedback ao Enviar uma Submissão no Treino Livre

Esta tarefa aborda o processo desde o login até o envio de um código para julgamento na aba de Treino Livre, com foco na avaliação de usabilidade e na identificação de melhorias necessárias para uma experiência mais eficiente e satisfatória.

## Metodologia

A metodologia que foi utilizada é a mesma descrita no [Planejamento do Relato de Resultados do Protótipo de Papel](https://interacao-humano-computador.github.io/2024.2-Grupo05/entregas/entrega_5/prototipo_papel/planejamento_relato).

### Objetivos

O objetivo desta avaliação é identificar pontos de melhoria na usabilidade do sistema a partir da interação de usuários com protótipos de papel. A análise busca compreender como o sistema comunica ações e resultados ao usuário, destacando aspectos críticos, como feedback e acessibilidade.

### Protótipo de Papel

O método de prototipação de papel foi utilizado por ser uma abordagem eficaz para explorar e validar conceitos iniciais de design de interface com baixo custo. Ele permite avaliar rapidamente a interação e a compreensão do usuário sobre a interface, antes de investir em implementações complexas.

### Dados Gerais

Para a realização desta avaliação, foi necessário um avaliador, que orientou e observou a interação, e um participante representando o público-alvo do sistema. Ambos foram selecionados com base em [perfis](https://interacao-humano-computador.github.io/2024.2-Grupo05/entregas/entrega_2/perfil) definidos previamente. As tarefas executadas incluíram a navegação pelo protótipo, com foco no envio de submissões, enquanto o avaliador registrava comportamentos, reações e dificuldades observadas.

### Problemas de Usabilidade Corrigidos Durante os Ciclos de Avaliação e Reprojeto

#### Problema 1: Processo de Login Complexo  
- **Local:** Acesso à plataforma, depois de selecionar um problema na aba de Treino Livre.  
- **Fatores de Usabilidade Prejudicados:**  
  - **Facilidade de aprendizado:** Se refere ao tempo e esforço necessários para
    que o usuário aprenda a utilizar o sistema com determinado nível de competência e
    desempenho.(Nielsen, 1993).  
  - **Eficiência:** Referente aos recursos necessários (tempo, ações) para atingir      objetivos no sistema (Nielsen, 1993).  
- **Descrição e Justificativa:** Anteriormente, os usuários precisavam enviar comandos para um bot no Telegram para obter dados de login e senha. Esse processo não era intuitivo, dificultando o acesso ao sistema e aumentando o tempo necessário para iniciar as tarefas.  
- **Correção Realizada no Protótipo em Papel:** Integração do login diretamente à plataforma, eliminando a etapa intermediária e simplificando o acesso.  
- **Problema Voltou a Ocorrer?:** Não, o problema foi resolvido com sucesso e validado nas interações subsequentes.  

#### Problema 2: Ausência de Atualização Automática do Feedback de Submissões  
- **Local:** Tela de submissão de código na aba de Treino Livre.  
- **Fatores de Usabilidade Prejudicados:**  
  - **Satisfação do usuário:** Relacionada à experiência emocional positiva ao utilizar o sistema (Nielsen, 1993).  
  - **Comunicabilidade:** Diz respeito à
    capacidade da interface de comunicar ao usuário a lógica do design: as intenções do
    designer e os princípios de interação resultantes das decisões tomadas durante todo
    o processo de design (Prates et al., 2000a; de Souza, 2005a; de Souza e Leitão, 2009).
- **Descrição e Justificativa:** O sistema exigia recarregamento manual da página para visualizar os resultados das submissões, gerando confusão e insatisfação.  
- **Correção Realizada no Protótipo em Papel:** Implementação de uma atualização automática do feedback em tempo real, com indicadores visuais claros para o progresso e resultados.  
- **Problema Voltou a Ocorrer?:** Não, o problema foi mitigado de forma eficaz.  

### Problemas de Usabilidade Ainda Não Corrigidos

#### Problema 1: Nenhum Problema Não Corrigido Identificado  
- **Local:** Não aplicável, pois não foram observados problemas adicionais não resolvidos durante as avaliações com o protótipo em papel.  
- **Fatores de Usabilidade Prejudicados:** Não aplicável.  
- **Descrição e Justificativa:** Os ciclos de avaliação e reprojeto atenderam a todas as dificuldades relatadas.  
- **Prioridade para Correção:** Não aplicável.  
- **Sugestões de Correção:** Realizar monitoramento contínuo das interações para identificar possíveis ajustes futuros com base no uso real do sistema.  

### Indicações de Partes do Sistema que Podem Ser Mais Bem Elaboradas

- **Login:** Embora o login proposto atualmente utilize apenas e-mail e senha, ele poderia ser enriquecido para incluir informações adicionais e relevantes do usuário, como nome completo, ou outras configurações que personalizem a experiência. Isso ajudaria a criar um ambiente mais informativo e ajustado às necessidades do usuário.  
- **Progresso em Tempo Real:** Apesar de o progresso em tempo real ser funcional, ele não fornece informações detalhadas sobre a quantidade de testes em que a submissão do usuário está sendo processada. A inclusão dessa funcionalidade poderia aumentar a transparência do sistema, reduzindo a ansiedade do usuário e melhorando a comunicabilidade.  

### Perguntas Respondidas com a Avaliação

1. **O usuário consegue operar o sistema?**  
   - **Resposta:** Sim.  

2. **Ele atinge seu objetivo? Com quanta eficiência? Em quanto tempo? Após cometer quantos erros?**  
   - **Resposta:** Sim.  
     - **Primeiro Protótipo:** O usuário atingiu o objetivo com menos eficiência e mais dúvidas. O tempo para realizar o login foi consideravelmente longo, com o usuário cometendo dois erros antes de concluir a tarefa.  
     - **Segundo Protótipo:** A eficiência aumentou significativamente, com menos dúvidas e um tempo menor para concluir o login, sem erros registrados.  

3. **Que parte da interface e da interação o deixa insatisfeito?**  
   - **Resposta:**  
     - A parte de login no primeiro protótipo, devido à complexidade desnecessária.  
     - O feedback de submissão de código, que não informava adequadamente o progresso das submissões.  

4. **Ele vai entender o que deve fazer em seguida?**  
   - **Resposta:**  
     - **Primeiro Protótipo:** Não. O usuário apresentou dificuldades em entender como obter os dados de login, o que causou frustração.  
     - **Segundo Protótipo:** Sim. O fluxo de interação ficou mais claro e intuitivo, facilitando a navegação e compreensão das ações necessárias.  

## Vídeo da Avaliação

**Vídeo 1** - Avaliação das duas alternativas de protótipo de papel.

<iframe width="560" height="315" src="https://www.youtube.com/embed/37jG-bdPSSY" title="Gravação da Entrevista - Parte 1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Termo de Consentimento

O Termo de Consentimento Livre e Esclarecido assinado está disponível em: [Termo de Consentimento - Felipe Rodrigues](./termos_de_consentimento/.pdf).

## Bibliografia

BARBOSA, Simone Diniz Junqueira; DA SILVA, Bruno Santana. Planejamento da avaliação de IHC. In: INTERAÇÃO Humano-Computador. Rio de Janeiro: Elsevier Editora, 2010.

## Histórico de Versão

| Versão |               Descrição                |   Autor    |    Data    |    Revisor     | Data de revisão |
| :----: | :------------------------------------: | :--------: | :--------: | :------------: | :-------------: |
|  1.0   | Criação do relato de resultado | [Felipe Rodrigues](https://github.com/felipeJRdev) | 14/01/2025 |  |  |