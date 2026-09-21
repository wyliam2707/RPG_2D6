# Continuidade de Campanha

Este documento define quando e como a IA deve fazer manutenção de continuidade durante uma campanha do RPG_2D6.

Ele não substitui `consulta.md` nem `salvamento.md`. Sua função é determinar **quando parar o fluxo normal do jogo para atualizar, consolidar, limpar e recarregar o contexto necessário**.

> **O fechamento do dia mantém o presente organizado. O encerramento de capítulo faz uma revisão completa da campanha.**

## 1. Dois momentos de continuidade

A campanha possui dois momentos principais de manutenção:

1. **Fechamento do dia** — manutenção leve e frequente.
2. **Encerramento de capítulo** — manutenção completa e acionada pelo jogador.

Esses dois momentos têm funções diferentes e não devem ser confundidos.

---

## 2. Fechamento do dia

O fechamento do dia acontece quando a ficção passa para um novo dia, normalmente ao dormir, acordar ou quando houver avanço equivalente de calendário.

Ao iniciar o novo dia, registre explicitamente:

`Novo dia — DD/MM/AAAA, dia da semana`

Exemplo:

`Novo dia — 01/02/2020, sábado`

A data deve permanecer coerente com o tempo transcorrido na campanha.

### 2.1 Agenda de continuidade

A campanha deve manter uma agenda de acontecimentos futuros já estabelecidos.

Exemplos:

- alguém prometeu voltar em determinada data;
- uma cobrança foi marcada;
- uma consulta foi agendada;
- uma viagem possui data de partida;
- uma entrega está prevista;
- um prazo foi estabelecido;
- um encontro foi combinado;
- um processo do mundo possui data conhecida.

A agenda não guarda possibilidades vagas. Registre somente compromissos, previsões, prazos ou acontecimentos futuros que já tenham sido estabelecidos na ficção.

Modelo:

~~~text
## Agenda de continuidade

02/05/2020
- Carlos vem cobrar o aluguel.

05/05/2020
- Consulta de Ana às 14h.

10/05/2020
- Entrega prevista das peças da oficina.
~~~

### 2.2 Durante o dia

Sempre que surgir um novo compromisso ou acontecimento futuro relevante, registre-o na agenda assim que ele estiver estabelecido.

Se um evento mudar de data, for cancelado ou se tornar impossível, atualize a agenda.

### 2.3 Ao começar um novo dia

Ao registrar um novo dia:

1. confirme a nova data e o dia da semana;
2. consulte a agenda;
3. identifique eventos previstos para hoje;
4. identifique compromissos vencidos que ainda possam produzir consequência;
5. remova eventos concluídos, cancelados, impossíveis ou que deixaram de ser relevantes;
6. mantenha pendências ainda ativas;
7. preserve no livro ou no estado o resultado dos eventos já resolvidos quando necessário.

Um evento programado não acontece automaticamente se os fatos da campanha o impedirem. A agenda lembra que ele deveria ser considerado.

### 2.4 Atualizações no fechamento do dia

No fechamento diário:

- atualize `estado/atual.md` se posição, condições, recursos, intenções, prazos ou situação imediata mudaram;
- atualize fichas apenas quando houver mudança estável real;
- atualize a agenda;
- registre processos ou compromissos que continuam no dia seguinte;
- aplique recuperações ou efeitos ligados à passagem do dia conforme `regras-basicas.md`.

O fechamento diário não exige uma revisão completa de todos os arquivos.

---

## 3. Encerramento de capítulo

O encerramento de capítulo só acontece quando o jogador disser explicitamente:

> **Narrador, encerre o capítulo.**

O Narrador não encerra o capítulo por conta própria.

Esse comando inicia uma manutenção completa da campanha e também funciona como **checkpoint técnico de ressincronização**.

O jogador pode usá-lo quando quiser consolidar a história, reorganizar arquivos ou quando perceber sinais de perda de contexto, continuidade ou direção narrativa.

---

## 4. Organização do livro no encerramento

Ao encerrar o capítulo, revise todo o material desde o último encerramento.

O pedido de encerramento não obriga a criar exatamente um novo arquivo de capítulo.

O Narrador pode:

- continuar e concluir um capítulo literário anterior que ainda esteja incompleto;
- salvar todo o material como um único capítulo;
- dividir o material em dois ou mais capítulos quando houver cortes editoriais naturais;
- reorganizar somente a divisão editorial, sem alterar acontecimentos.

A divisão literária deve respeitar ritmo, unidade de cena, mudança de foco, passagem de tempo e estrutura narrativa.

> **O checkpoint encerra um ciclo de jogo. A quantidade de capítulos literários salvos depende do material.**

Não crie capítulos curtos ou artificiais apenas porque houve um checkpoint.

---

## 5. Limpeza geral no encerramento

Depois de organizar o livro, faça uma revisão completa da campanha.

### 5.1 Estado atual

Reescreva `estado/atual.md` para manter somente o presente operacional.

Remova:

- cenas encerradas sem efeito atual;
- fatos históricos já preservados no livro;
- ameaças resolvidas;
- intenções concluídas;
- recursos que deixaram de importar;
- duplicações;
- informações estáveis já consolidadas em ficha ou mundo.

Mantenha apenas o que ainda pode afetar decisões futuras.

### 5.2 Agenda

Revise toda a agenda:

- remova eventos concluídos;
- remova eventos cancelados ou impossíveis;
- mantenha pendências;
- atualize datas alteradas;
- adicione compromissos futuros estabelecidos durante o ciclo encerrado.

### 5.3 Fichas

Atualize fichas somente com mudanças estáveis:

- Poderes ou Recursos permanentes;
- itens obtidos ou perdidos de forma estável;
- conhecimento consolidado;
- relação consolidada;
- objetivo estável alterado;
- mudança real e duradoura de personalidade;
- condição permanente;
- alteração de controle ou importância.

Não transforme emoção passageira ou reação momentânea em mudança permanente de ficha.

### 5.4 Mundo

Atualize `mundo/` quando um fato do cenário se tornar estável e relevante para consultas futuras.

### 5.5 Mestre

Atualize `mestre/` quando segredos, ameaças, planos, prazos ou processos reservados mudarem de forma relevante.

### 5.6 READMEs

Atualize os READMEs necessários para preservar:

- índices corretos;
- arquivos ativos;
- capítulo atual;
- último capítulo concluído;
- ponto de retomada;
- personagens relevantes;
- rotas de consulta.

---

## 6. Recarga do sistema

Depois da limpeza e do salvamento, recarregue o contexto central antes de continuar.

Abra novamente:

1. `regras-basicas.md`;
2. `narrador-ia.md`;
3. `personagens-ia.md`;
4. `campanhas/nome-da-campanha/README.md`;
5. `campanhas/nome-da-campanha/estado/atual.md`;
6. fichas das personagens imediatamente relevantes;
7. direção da campanha e arquivos adicionais indicados por `consulta.md`.

A recarga serve para reduzir deriva de contexto e restaurar:

- regras mecânicas;
- forma correta de narrar;
- autonomia das personagens;
- foco narrativo;
- gênero e tom;
- posição atual;
- intenções em andamento;
- agenda;
- compromissos e fios ativos.

Não dependa apenas da memória da conversa para retomar depois de um encerramento.

---

## 7. Encerramento como ressincronização

O jogador pode pedir um encerramento mesmo quando a história poderia continuar normalmente.

Isso é permitido.

O objetivo pode ser:

- consolidar uma sessão longa;
- corrigir deriva narrativa;
- recuperar foco;
- reforçar regras esquecidas;
- limpar estado acumulado;
- reorganizar o livro;
- preparar uma retomada mais segura.

O Narrador deve executar o ciclo completo sem inventar um final artificial para a cena.

Se o material literário ainda estiver no meio de uma unidade narrativa, o livro pode continuar o capítulo anterior e somente abrir outro quando houver corte editorial adequado.

---

## 8. Relação com consulta e salvamento

Use:

- `continuidade.md` para decidir **quando fazer manutenção**;
- `salvamento.md` para decidir **onde cada informação deve ser salva**;
- `consulta.md` para decidir **o que deve ser recarregado e em que ordem**.

Esses arquivos trabalham juntos e não devem duplicar suas funções.

---

## 9. Referência rápida

### Fechamento do dia

~~~text
1. Registrar nova data e dia da semana.
2. Consultar a agenda.
3. Tratar compromissos de hoje e pendências.
4. Remover eventos encerrados ou irrelevantes.
5. Adicionar novos compromissos.
6. Atualizar estado quando necessário.
7. Atualizar fichas somente se houve mudança estável.
8. Aplicar efeitos da passagem do dia.
~~~

### Narrador, encerre o capítulo

~~~text
1. Revisar o material desde o último encerramento.
2. Completar capítulo anterior se necessário.
3. Dividir o material em um ou mais capítulos quando fizer sentido.
4. Salvar o livro.
5. Limpar e reescrever o estado atual.
6. Revisar a agenda.
7. Consolidar fichas.
8. Atualizar mundo e mestre quando necessário.
9. Atualizar READMEs e ponto de retomada.
10. Recarregar regras, narrador, personagens IA e direção da campanha.
11. Retomar somente depois da ressincronização.
~~~

## Regra final

> **O fechamento diário preserva o relógio e os compromissos do mundo. O encerramento de capítulo preserva a saúde geral da campanha: salva, limpa, consolida e recarrega o sistema antes de continuar.**
