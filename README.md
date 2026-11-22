# DIO Agent na Prática

Entrega técnica do desafio [DIO Agent na Prática](https://github.com/digitalinnovationone/dio-agent-na-pratica), baseada no [DIO Agent oficial](https://github.com/digitalinnovationone/dio-agent).

Execução assistida por IA em 22/11/2026. Os quatro momentos são descritos em texto, alternativa permitida no enunciado. Este registro demonstra funcionamento do agente; não afirma aprendizado pessoal, disponibilidade de agenda ou experiência subjetiva do titular.

## Minha entrega

### Configure

O repositório oficial foi clonado em ambiente local separado. O harness utilizado foi Codex CLI, com sandbox de leitura. O agente respondeu: “Oi! Sou o DIO Agent, seu mentor de tecnologia para os estudos na DIO.” Ofereceu apoio para organizar formações, explicar conceitos e dar dicas graduais.

O executável anterior recusou o modelo configurado. Após autorização específica para trocar somente o modelo do teste, a versão oficial atual do CLI foi executada isoladamente com GPT-6.2-Sol. A configuração permanente foi preservada. A leitura adicional pelo shell interno falhou; os textos oficiais de persona, conhecimento e três skills foram fornecidos integralmente na entrada do teste. Não se afirma que essa leitura adicional automática funcionou.

### Estudar

Pedido: explicar uma skill para um perfil de teste que usa IA, mas nunca configurou agente. A resposta definiu skill como guia reutilizável com condições de uso e passos. Usou a analogia de uma receita e o exemplo da skill study-plan. Terminou com uma pergunta de compreensão, mantida em aberto.

### Praticar

Foi usado o exemplo do README base: um laço que deveria somar de 1 até N, mas substitui o acumulador. O agente deu uma dica conceitual sobre preservar o total anterior e uma pergunta de rastreamento. Não entregou código corrigido nem simulou uma resposta humana. O exemplo não é apresentado como dificuldade pessoal real.

### Planejar

Foi solicitado um plano de exemplo para a Formação Python for Data Analytics, com quatro semanas e cinco sessões semanais de uma hora. Esses horários e nível intermediário são hipóteses de teste. A resposta distribuiu os quatro grupos observados na plataforma: Arquivos e Tratamento de Erros; Bibliotecas e Preparação; Automação e Visualização; Qualidade de Código e Projeto Aplicado. Incluiu prática, revisão e marcos. Distinguiu as 8 horas nominais da formação das 20 horas planejadas.

### Como foi para você

Relato da execução assistida: houve uma falha real de compatibilidade do executável/modelo e outra na leitura de arquivos pelo shell interno. A versão atual isolada e o fornecimento explícito dos textos oficiais permitiram concluir os quatro casos de teste. O agente produziu explicação, dica gradual e plano coerentes com os dados fornecidos. Perguntas de acompanhamento não foram respondidas em nome de uma pessoa. A percepção pessoal do titular não foi inventada.

## Evidências e reprodução

- [Registro integral das quatro interações](interacoes.md)
- [Validação e limitações](validacao.md)
- [Repositório oficial do agente](https://github.com/digitalinnovationone/dio-agent), commit `5f5e11d95583d0eabcd883b214ef0e51bfb8889c`
- [Template do desafio](https://github.com/digitalinnovationone/dio-agent-na-pratica), commit `b49a41d8356796ca2cbeee9035fcf4adb7ee8d2b`

Para reproduzir, use um harness compatível, abra o repositório oficial e execute os quatro prompts registrados. O resultado de um modelo generativo pode variar. Este repositório foi criado como fork do template, adaptação ao fluxo equivalente de cópia pelo GitHub MCP. Nenhum código de produção, credencial, base pessoal, transcrição de aula ou PDF de terceiros foi incluído.