# Salvamento de Campanha

Este documento ensina uma IA a criar, organizar e atualizar os arquivos de uma campanha do RPG 2D6.

Salvar não é copiar toda a conversa. É preservar a realidade canônica no lugar correto para que a campanha possa continuar sem contradições.

> **O livro guarda o que aconteceu. O estado guarda o que ainda está acontecendo. As fichas e o mundo guardam o que se tornou estável.**

## 1. Responsabilidade

Ao salvar, a IA deve:

- criar a estrutura da campanha quando ela ainda não existir;
- registrar somente fatos estabelecidos;
- preservar a ordem dos acontecimentos;
- separar informação pública, conhecimento individual e material reservado;
- atualizar condições, recursos, posições e intenções persistentes;
- consolidar mudanças permanentes nas fontes corretas;
- manter índices curtos nos READMEs;
- impedir duplicação e crescimento indefinido do estado atual;
- preservar o livro como memória integral da campanha.

A IA não deve salvar:

- cadeia de raciocínio interna;
- possibilidades descartadas;
- rascunhos não aprovados;
- intenções como se já fossem resultados;
- resultados que ainda não foram julgados;
- suposições técnicas como fatos canônicos;
- regras universais dentro da pasta da campanha;
- a mesma informação completa em vários arquivos.

## 2. Estrutura obrigatória

Ao criar uma campanha, use:

~~~text
campanhas/
└── nome-da-campanha/
    ├── README.md
    ├── estado/
    │   ├── README.md
    │   └── atual.md
    ├── continuidade/
    │   ├── README.md
    │   └── dias/
    │       └── README.md
    ├── personagens/
    │   └── README.md
    ├── mundo/
    │   └── README.md
    ├── mestre/
    │   └── README.md
    └── livro/
        └── README.md
~~~

Os READMEs fazem as pastas existirem no GitHub e funcionam como mapas de consulta.

Use nomes de arquivos estáveis, claros e únicos. Para novos arquivos, prefira letras minúsculas, palavras separadas por hífen e numeração com zeros à esquerda quando houver sequência.

Exemplos:

~~~text
ana-silva.md
cidade-portuaria.md
faccoes.md
capitulo-001-a-chegada.md
2025-09-03-quarta-feira.md
~~~

Não renomeie arquivos canônicos sem atualizar todas as referências.

## 3. Regra de destino

Classifique cada informação antes de salvar:

| Informação | Destino |
|---|---|
| Premissa, gênero, tom e controle das personagens | README da campanha |
| Situação necessária para continuar agora | estado/atual.md |
| Fechamento diário, calendário, agenda e autonomia fora de cena | continuidade/dias/AAAA-MM-DD-dia-da-semana.md |
| Identidade e mudanças permanentes de personagem | personagens/nome.md |
| Verdade estável do cenário | mundo/arquivo-tematico.md |
| Segredo, plano ou ameaça ainda reservada | mestre/arquivo-tematico.md |
| Acontecimentos completos em ordem cronológica | livro/capitulo-NNN-titulo.md |
| Índice e rota de consulta | README da pasta correspondente |
| Regra universal | arquivo de regras na raiz, nunca na campanha |

Pergunta operacional:

> **Esta informação descreve o passado, o presente ativo, uma identidade estável, o mundo estável, um fechamento diário ou algo reservado?**

Se uma informação pertencer a mais de uma função, cada arquivo recebe somente a forma adequada.

Exemplo:

- o livro registra a cena completa em que Ana perdeu a espada;
- o estado atual registra que Ana está sem a espada, se isso ainda importar;
- a ficha remove a espada dos itens possuídos, se a perda for estável;
- o fechamento diário registra a agenda e o que personagens importantes fizeram fora da câmera naquele dia;
- nenhum dos arquivos precisa copiar integralmente os outros.

## 4. README da campanha

O arquivo campanhas/nome-da-campanha/README.md é a porta de entrada da campanha.

Deve conter:

~~~text
# Nome da campanha

STATUS: PREPARAÇÃO, ATIVA, PAUSADA ou ENCERRADA

## Premissa
Descrição curta da proposta.

## Direção
Gênero, tom, temas e limites definidos.

## Personagens com agência
Nome — controle — importância — arquivo da ficha.

## Estrutura
- Estado atual: estado/atual.md
- Continuidade diária: continuidade/README.md
- Personagens: personagens/README.md
- Mundo: mundo/README.md
- Material reservado: mestre/README.md
- Livro: livro/README.md

## Retomada
- Capítulo atual:
- Último capítulo concluído:
- Ponto de continuação:
~~~

O README orienta a navegação. Ele não deve repetir fichas, estado, mundo nem capítulos.

Atualize-o quando mudar:

- status da campanha;
- direção estrutural;
- lista de personagens com agência;
- capítulo atual;
- ponto oficial de retomada.

## 5. README de estado

O arquivo estado/README.md deve declarar:

- atual.md é o ponto operacional de retomada;
- somente informações ativas permanecem nele;
- fatos históricos completos pertencem ao livro;
- fechamentos diários pertencem a continuidade/dias/;
- verdades permanentes devem ser consolidadas em fichas ou mundo;
- material reservado continua separado;
- o arquivo deve ser reescrito para permanecer compacto.

Modelo:

~~~text
# Estado

atual.md contém o presente operacional da campanha.

Abrir este arquivo ao iniciar ou retomar a sessão. Informações encerradas são preservadas no livro ou na continuidade diária e removidas daqui quando não forem mais necessárias para decisões futuras.
~~~

## 6. Estado atual

O arquivo estado/atual.md deve permitir retomar a campanha sem reler todo o livro.

Estrutura recomendada:

~~~text
# Estado atual

## Momento
Data, horário aproximado e tempo transcorrido relevante.

## Cena atual
Local, participantes, situação imediata e última mudança estabelecida.

## Posição e condição
Localização, PV, PA, Estados e efeitos ativos das personagens relevantes.

## Intenções e processos
Atividades persistentes, compromissos, prazos e condições de conclusão.

## Conhecimento distribuído
Somente diferenças de conhecimento necessárias para decisões atuais.

## Relações em mudança
Tensões ou mudanças recentes ainda não consolidadas nas fichas.

## Recursos e objetos relevantes
Posse, perda, consumo, carga ou localização atual.

## Fios ativos
Questões, ameaças, promessas e oportunidades ainda abertas.

## Retomada
Capítulo em andamento, última cena salva e ponto exato da próxima decisão.
~~~

O estado atual deve ser uma fotografia útil, não um resumo de toda a campanha.

Remova do estado:

- cenas encerradas sem efeito atual;
- explicações históricas já acessíveis no livro;
- fatos estáveis já consolidados no mundo;
- mudanças permanentes já consolidadas nas fichas;
- ameaças resolvidas;
- recursos consumidos que não produzem efeito atual;
- duplicações.

Mantenha no estado aquilo cuja ausência poderia causar erro na próxima decisão.

## 6A. Continuidade diária

A pasta continuidade/ guarda fechamentos diários e manutenção leve de calendário, agenda e autonomia de personagens importantes fora da cena principal.

Use:

~~~text
campanhas/nome-da-campanha/continuidade/
├── README.md
└── dias/
    ├── README.md
    └── AAAA-MM-DD-dia-da-semana.md
~~~

Exemplo:

~~~text
campanhas/o-campus/continuidade/dias/2025-09-03-quarta-feira.md
~~~

Cada fechamento diário deve conter:

~~~md
# Fechamento do Dia — DD/MM/AAAA, dia da semana

## Will

Resumo do dia de Will.

### Estado final de Will

- PV:
- PA:
- PE:
- Posição:
- Selo de Velamento:
- Itens relevantes:
- Pendências pessoais:

## Gwen

Resumo narrativo de pelo menos 10 linhas quando aplicável.

## Riri

Resumo narrativo de pelo menos 10 linhas quando aplicável.

## Agenda

- Evento ou compromisso futuro.
- Pendência com data ou período.
- Acontecimento previsto.

## Pendências abertas

- Fios ainda ativos.
- Consequências não resolvidas.
- Investigações em andamento.

## Novo dia

`Novo dia — DD/MM/AAAA, dia da semana`

## Ponto de retomada

Descrição objetiva de onde a campanha deve continuar.
~~~

Função da continuidade diária:

- registrar a data encerrada e o novo dia;
- preservar o que personagens importantes fizeram fora da câmera;
- registrar família, amigos, rotina, estudo, trabalho, patrulha ou atividade própria dessas personagens;
- manter a agenda e compromissos futuros;
- preservar pendências que atravessam a virada de dia;
- dar ao jogador informação de narrador sem transferi-la automaticamente ao personagem.

A continuidade diária não substitui:

- `livro/`, que guarda a versão literária e cronológica dos acontecimentos;
- `estado/atual.md`, que guarda apenas o presente operacional;
- fichas de personagem, que guardam mudanças estáveis;
- `mestre/`, que guarda material reservado.

## 7. README de personagens

O arquivo personagens/README.md é o índice das fichas.

Modelo:

~~~text
# Personagens

Cada arquivo é a fonte canônica de identidade da personagem.

- Will — JOGADOR HUMANO — central — will.md
- Ana — IA — central — ana.md
- Marta — IA — incidental — marta.md
~~~

Atualize o índice quando uma personagem:

- for criada;
- receber ficha própria;
- mudar de controle;
- tornar-se central ou deixar de ser relevante;
- tiver seu arquivo renomeado.

O README não copia personalidade, capacidades ou relações. Essas informações pertencem à ficha.

## 8. Atualização das fichas

Atualize uma ficha somente quando a mudança for estável.

Pode justificar atualização:

- novo Poder, Recurso ou item permanente;
- perda permanente de capacidade ou posse;
- conhecimento que não pode ser esquecido;
- relação consolidada;
- objetivo adotado ou abandonado de modo estável;
- mudança duradoura de personalidade, limite ou código;
- fato passado que continuará influenciando decisões.

Não atualize a ficha por:

- emoção passageira;
- ferimento temporário;
- intenção momentânea;
- localização;
- gasto atual de PA;
- impressão ainda incerta;
- hipótese;
- relação que apenas começou a mudar.

Mudanças temporárias ficam em estado/atual.md. O livro preserva como elas surgiram.

## 9. README e arquivos de mundo

O arquivo mundo/README.md indexa verdades estáveis do cenário.

Exemplo:

~~~text
# Mundo

Esta pasta guarda fatos públicos ou estruturalmente verdadeiros do cenário.

- Cidade Portuária — cidade-portuaria.md
- Facções conhecidas — faccoes.md
- Fenômenos estabelecidos — fenomenos.md
~~~

Crie arquivos temáticos somente quando houver conteúdo real. Não crie dezenas de arquivos vazios.

Mova para o mundo fatos que:

- continuarão verdadeiros além da cena;
- definem lugar, organização, cultura, tecnologia ou fenômeno;
- podem ser consultados por várias cenas;
- não pertencem exclusivamente à memória de uma personagem.

O arquivo de mundo define a verdade técnica. Cada personagem só pode usar essa verdade se possuir conhecimento legítimo dela.

## 10. README e material do mestre

O arquivo mestre/README.md é o índice reservado.

Modelo:

~~~text
# Mestre

Esta pasta guarda verdades, segredos, ameaças e planos que não são conhecimento automático das personagens.

- Conflitos ativos — conflitos.md
- Segredos do cenário — segredos.md
- Planos e prazos — planos.md
~~~

Material reservado pode incluir:

- verdade ainda não revelada;
- motivação secreta;
- plano adversário;
- prazo oculto;
- recurso desconhecido;
- identidade secreta;
- consequência preparada legitimamente;
- informação necessária para julgar, mas não para decidir por personagens.

A IA técnica pode abrir esses arquivos quando estiver exercendo função de Narrador ou atualizando a campanha. Ao decidir por uma personagem, não transfira esse conhecimento para ela.

Quando um segredo for revelado:

- o livro registra como ocorreu a revelação;
- o estado registra quem sabe, se ainda for relevante;
- a ficha recebe o conhecimento quando ele se tornar estável;
- o arquivo reservado é atualizado, mas não precisa ser apagado se ainda contiver verdade técnica útil.

## 11. Livro como memória integral

A pasta livro/ contém a memória cronológica integral da campanha em formato literário.

O livro registra a versão final dos acontecimentos estabelecidos pelo Narrador. Não registra raciocínio interno da IA, tentativas de resposta descartadas ou resultados que nunca aconteceram.

Cada capítulo usa:

~~~text
# Capítulo 001 — Título

STATUS: EM ANDAMENTO ou CONCLUÍDO
Período:
Local inicial:
Perspectiva inicial:
~~~

Durante uma sessão, o capítulo em andamento pode ser atualizado em pontos seguros para impedir perda de memória. Ao encerrar o capítulo, marque-o como CONCLUÍDO e não acrescente acontecimentos posteriores nele.

## 12. Forma literária

O corpo do capítulo pode ser escrito como narrativa literária, preservando clareza causal e ordem cronológica.

Use:

~~~text
[Will] — Fala audível.

[Will, pensa] — Pensamento privado.

[Will, telepatia para Ana] — Comunicação mental dirigida.

[Will, escreve] — Conteúdo escrito pelo personagem.

[Gravação de Will] — Fala reproduzida por um dispositivo.

[Voz desconhecida] — Fala cuja origem ainda não foi identificada.
~~~

Texto sem marcador é narração.

Regras:

- identifique sempre o autor de fala ou pensamento;
- preserve o significado de falas declaradas pelo jogador;
- narre acontecimentos na ordem em que ocorreram;
- marque saltos de tempo e mudanças de local;
- indique ações simultâneas com clareza;
- identifique lembranças ou recuos temporais;
- não reorganize fatos apenas para criar suspense literário;
- não transforme pensamento privado em conhecimento alheio;
- não acrescente acontecimentos novos durante a redação;
- não enfraqueça nem amplie resultados já estabelecidos.

> **O livro pode ser literário, mas continua sendo uma fonte canônica de fatos.**

## 13. README do livro

O arquivo livro/README.md é o índice cronológico.

Modelo:

~~~text
# Livro

Esta pasta guarda a memória integral da campanha em capítulos literários.

## Em andamento
- Capítulo 003 — A ponte vazia
  - Período: segundo dia, noite
  - Arquivo: capitulo-003-a-ponte-vazia.md

## Concluídos
- Capítulo 001 — A chegada
  - Período: primeiro dia, manhã
  - Arquivo: capitulo-001-a-chegada.md
- Capítulo 002 — Vozes no corredor
  - Período: primeiro dia, tarde
  - Arquivo: capitulo-002-vozes-no-corredor.md
~~~

Ao concluir ou criar um capítulo, atualize o índice. Não transforme o README em resumo completo dos capítulos.

## 14. Quando salvar

Salve depois de uma mudança canônica relevante, especialmente quando houver:

- resultado de teste;
- mudança de cena ou local;
- gasto ou recuperação importante;
- dano, cura ou Estado;
- nova informação descoberta;
- decisão que cria compromisso futuro;
- início, avanço ou conclusão de processo;
- mudança de relação;
- criação ou perda de objeto;
- passagem significativa de tempo;
- fechamento diário;
- encerramento de cena, sessão ou capítulo;
- correção explícita do jogador.

Não é necessário gravar novamente arquivos que não mudaram.

## 15. Ciclo de salvamento

Depois de estabelecer uma sentença:

1. confirme o que realmente aconteceu;
2. separe fatos observáveis, pensamentos, conhecimento privado e verdade reservada;
3. acrescente o acontecimento ao capítulo em andamento;
4. atualize estado/atual.md com consequências ainda ativas;
5. salve fechamentos diários em continuidade/dias/ quando o dia for fechado;
6. consolide mudanças permanentes nas fichas;
7. consolide verdades estáveis no mundo;
8. atualize segredos, planos e prazos no mestre;
9. remova do estado o que deixou de ser atual;
10. atualize os READMEs cujos índices mudaram;
11. confira se a próxima decisão pode ser retomada sem reler tudo.

Sempre que possível, trate o conjunto como uma única atualização coerente. Não deixe o estado apontar para um capítulo inexistente nem um índice apontar para arquivo não criado.

## 16. Fechamento de capítulo

Ao fechar um capítulo:

1. confirme que somente acontecimentos estabelecidos entraram no texto;
2. revise ordem, autoria de falas e marcações de pensamento;
3. marque o capítulo como CONCLUÍDO;
4. registre-o no livro/README.md;
5. atualize o README da campanha;
6. mova fatos permanentes para fichas ou mundo;
7. mova segredos e processos ocultos para mestre;
8. compacte estado/atual.md;
9. defina o ponto exato de retomada;
10. crie o próximo capítulo somente quando houver nova cena a registrar.

O capítulo concluído torna-se arquivo histórico. Não o reescreva para adaptar a história a decisões posteriores.

## 17. Correções e continuidade

Diferencie:

- **correção textual:** ortografia, formatação ou frase sem alteração factual;
- **correção canônica:** mudança no que se considera verdadeiro.

Correções textuais podem ser feitas diretamente.

Para correção canônica:

1. identifique a instrução mais recente e explícita;
2. atualize estado, ficha, mundo ou mestre afetado;
3. corrija o capítulo correspondente;
4. marque a correção de modo identificável quando ela alterar o sentido histórico;
5. atualize índices ou referências;
6. não preserve o erro como verdade apenas porque apareceu antes.

Se duas fontes continuarem em conflito, não escolha silenciosamente. Preserve o que estiver confirmado e solicite apenas o esclarecimento indispensável.

## 18. Verificação final

Antes de encerrar o salvamento, confirme:

~~~text
1. Salvei apenas fatos estabelecidos?
2. Mantive intenção separada de resultado?
3. O livro preserva a ordem cronológica?
4. Falas e pensamentos têm autoria clara?
5. Pensamento privado permaneceu privado?
6. O estado contém somente o presente necessário?
7. Mudanças permanentes foram consolidadas?
8. Segredos ficaram na área reservada?
9. Alguma regra foi duplicada dentro da campanha?
10. Os READMEs apontam para arquivos existentes?
11. Existe um ponto exato de retomada?
12. Fechamentos diários foram salvos em continuidade/dias/ quando acionados?
13. A campanha pode continuar sem reler o livro inteiro?
~~~

## Regra final

> **Salvar é transformar acontecimentos estabelecidos em memória organizada. O livro preserva integralmente a história em ordem literária; o estado preserva o presente operacional; a continuidade diária preserva calendário, agenda e vida fora da câmera; fichas e mundo preservam verdades estáveis; o mestre preserva material reservado; e os READMEs indicam onde cada informação deve ser encontrada.**