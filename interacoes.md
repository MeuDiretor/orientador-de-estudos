# Demonstração técnica do DIO Agent

**Adaptação do teste.** Como a leitura pelo shell do harness apresentou falha de ambiente, usei a persona, a base de conhecimento e as skills oficiais reproduzidas na mensagem. O registro foi produzido sem ferramentas, chamadas externas, leitura do sistema de arquivos ou alterações no projeto. As quatro interações são casos de teste automatizados. As perguntas ficam em aberto, sem respostas simuladas.

## 1. Apresentação do agente

**Prompt**

> Oi! Quem é você e como pode me ajudar nos meus estudos na DIO?

**Resposta do DIO Agent**

Oi! Sou o DIO Agent, seu mentor de tecnologia para os estudos na DIO. Posso ajudar você a organizar uma Formação ou um Bootcamp, explicar um conceito de uma aula com exemplos e dar dicas graduais quando um desafio travar. A ideia é que você entenda o caminho e consiga dar o próximo passo por conta própria.

**Pergunta aberta:** O que você quer estudar ou praticar na DIO agora?

## 2. Explicação de conceito

**Prompt**

> Me explica o que é uma skill de um agente de IA. Perfil de TESTE: usa IA no dia a dia e nunca configurou agente.

**Resposta do DIO Agent**

Uma *skill* é um guia reutilizável que diz ao agente quando usar um procedimento e quais passos seguir. Pense nela como uma receita que fica à mão para um tipo de pedido que aparece com frequência.

Por exemplo, quando alguém pede um plano de estudos, a skill `study-plan` orienta o DIO Agent a partir do objetivo e do tempo informados, usar os módulos da trilha e definir marcos semanais. O pedido traz os detalhes do caso. A skill dá ao agente um jeito consistente de trabalhar com esses detalhes.

**Pergunta aberta:** Nesse exemplo, que parte do pedido mudaria de uma pessoa para outra e que orientação da skill poderia continuar a mesma?

## 3. Primeira dica no desafio de código

**Prompt**

> Exemplo de prática do README oficial, não dificuldade pessoal declarada: desafio soma de 1 até N. Código `let n=parseInt(gets()); let soma=0; for(let i=1;i<=n;i++){soma=i;} print(soma);` Me ajuda a destravar sem dar resposta pronta. Mostre só dica inicial e pergunta de verificação.

**Resposta do DIO Agent**

**Dica inicial:** Um acumulador guarda o total parcial de uma rodada do laço para a próxima.

**Pergunta aberta:** Com `N = 3`, que valor fica em `soma` depois da segunda rodada do seu código e o que esse valor representa?

## 4. Plano de estudos de exemplo

**Prompt**

> Plano EXEMPLO, sem alegar disponibilidade real de Felipe: concluir Formação Python for Data Analytics, nível intermediário, quatro semanas e 1h por dia de segunda a sexta. Fonte verificada pelo executor na DIO https://web.dio.me/track/formacao-python-for-data-analytics : 8h declaradas, 7 cursos e 1 projeto. Grupos observados: Arquivos e Tratamento de Erros em Python (2 atividades); Bibliotecas e Preparação de Dados (2); Automação e Visualização de Dados (2); Qualidade de Código e Projeto Aplicado (2). Organize por esses grupos, não invente nomes adicionais de curso. Carga nominal não é tempo de domínio; reservar prática e revisão. Não ativar notificações nem meta na plataforma.

**Resposta do DIO Agent**

Para este exemplo de nível intermediário, o objetivo é concluir a **Formação Python for Data Analytics** em quatro semanas, com sessões de 1 hora de segunda a sexta. São **20 horas planejadas**. A trilha tem **8 horas declaradas, 7 cursos e 1 projeto**, segundo os dados fornecidos pelo executor. As 8 horas servem como referência de carga nominal. O cronograma reserva sessões para prática, revisão e desenvolvimento do projeto. [Formação Python for Data Analytics na DIO](https://web.dio.me/track/formacao-python-for-data-analytics)

| Semana | Grupo da trilha | Segunda a quarta | Quinta e sexta | Marco de progresso |
|---|---|---|---|---|
| 1 | Arquivos e Tratamento de Erros em Python · 2 atividades | Estude as duas atividades e repita os exemplos. | Pratique a leitura de um arquivo, teste o caso de arquivo ausente e revise o tratamento do erro. | Ler um arquivo válido e explicar como o código trata a ausência do arquivo. |
| 2 | Bibliotecas e Preparação de Dados · 2 atividades | Estude as duas atividades e reproduza uma preparação de dados. | Pratique com uma base pequena, revise as transformações e confira o resultado. | Mostrar a base antes e depois da preparação e explicar o que mudou. |
| 3 | Automação e Visualização de Dados · 2 atividades | Estude as duas atividades e reproduza um fluxo de trabalho. | Automatize uma etapa repetitiva, gere uma visualização e revise se ela responde à pergunta escolhida. | Reexecutar o fluxo e explicar o que o gráfico mostra. |
| 4 | Qualidade de Código e Projeto Aplicado · 2 atividades | Estude o conteúdo de qualidade de código e avance no projeto conforme o enunciado. | Revise o código, execute o projeto do início ao fim e confira os requisitos antes da entrega. | Finalizar o projeto e conferir as oito atividades da trilha. |

A divisão dos dias é uma sugestão de ritmo. Se uma atividade ocupar mais tempo, reorganize os blocos da semana e preserve uma sessão para praticar ou revisar.

**Pergunta aberta:** Nesse cenário de exemplo, qual semana você ajustaria primeiro se uma atividade consumisse duas sessões a mais?

## Limitações e critérios de verificação

O teste avalia as respostas escritas em uma rodada por caso. O carregamento automático dos arquivos pelo harness, a execução do JavaScript e a consulta ao catálogo ao vivo ficaram fora da verificação. Os dados da Formação vieram da consulta relatada pelo executor. As perguntas abertas deixam a adaptação a respostas posteriores fora deste teste.

| Caso | Critério verificável no registro |
|---|---|
| Apresentação | Identifica o DIO Agent como mentor, descreve formas concretas de apoio na DIO e termina com uma pergunta aberta. |
| Conceito | Usa o perfil de teste informado e apresenta uma definição simples, uma analogia, um exemplo do próprio agente e uma pergunta de compreensão. |
| Desafio | Traz exatamente uma dica conceitual e uma pergunta de verificação. A correção do código fica em aberto. |
| Plano | Mantém os quatro grupos na ordem fornecida, com duas atividades por grupo. Soma 20 horas em quatro semanas, registra a carga nominal de 8 horas, 7 cursos e 1 projeto e inclui prática, revisão e um marco por semana. |
| Escopo | Trata o perfil e o horário como exemplos, deixa as perguntas sem respostas simuladas e registra zero ações na plataforma, inclusive em metas e notificações. |