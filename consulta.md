# Consulta e Carregamento

Este documento ensina uma IA a abrir somente os arquivos necessários para iniciar, retomar, narrar, decidir por personagens e pesquisar a memória de uma campanha do RPG 2D6.

Consultar não é carregar todo o repositório. É localizar a fonte correta, extrair o necessário e preservar os limites de conhecimento.

> **Abra primeiro o mapa, depois o presente e somente então as fontes exigidas pela decisão atual.**

## 1. Objetivo

A consulta deve permitir que a IA:

- encontre rapidamente a campanha correta;
- carregue as regras universais necessárias;
- retome o ponto atual;
- interprete somente as personagens relevantes;
- recupere fatos antigos sem ler todo o livro;
- consulte segredos sem transferi-los às personagens;
- diferencie verdade técnica, percepção e conhecimento;
- evite preencher lacunas com memória vaga;
- mantenha o contexto pequeno o bastante para decidir com precisão.

## 2. Tipos de fonte

As fontes possuem funções diferentes:

| Fonte | Função |
|---|---|
| regras-basicas.md | Resolver possibilidade, teste e efeito |
| narrador-ia.md | Julgar e transformar resultado em narrativa |
| personagens-ia.md | Criar e decidir por personagens controladas por IA |
| criacao-de-personagem.md | Criar ou revisar fichas |
| campanhas/nome/README.md | Identificar e orientar a campanha |
| estado/atual.md | Informar o presente operacional |
| personagens/nome.md | Definir identidade, capacidades e conhecimento da personagem |
| mundo/ | Definir verdades estáveis do cenário |
| mestre/ | Preservar verdades e processos reservados |
| livro/ | Preservar a memória histórica integral |

Uma fonte não deve ser usada para uma função diferente sem necessidade.

## 3. Ordem normal de abertura

Ao iniciar ou retomar uma campanha, abra:

~~~text
1. regras-basicas.md
2. narrador-ia.md
3. personagens-ia.md
4. campanhas/nome-da-campanha/README.md
5. campanhas/nome-da-campanha/estado/README.md
6. campanhas/nome-da-campanha/estado/atual.md
7. campanhas/nome-da-campanha/personagens/README.md
8. fichas das personagens presentes ou imediatamente relevantes
~~~

Depois, abra somente quando necessário:

~~~text
mundo/README.md
→ para localizar verdade estável do cenário.

mestre/README.md
→ para localizar segredo, ameaça, plano ou prazo reservado.

livro/README.md
→ para localizar capítulo, período ou acontecimento antigo.

criacao-de-personagem.md
→ somente ao criar ou revisar uma ficha.
~~~

Não abra todos os capítulos, todas as fichas ou todos os arquivos do mundo por padrão.

## 4. Carregamento inicial mínimo

O carregamento inicial precisa responder:

- qual campanha está ativa;
- qual é sua proposta;
- onde e quando a próxima cena começa;
- quem está presente;
- quem controla cada personagem;
- quais condições e recursos estão ativos;
- quais intenções ou processos continuam;
- qual foi o último acontecimento estabelecido;
- qual decisão pertence agora ao jogador;
- quais arquivos adicionais podem ser necessários.

Se essas respostas estiverem claras, o carregamento inicial está completo.

## 5. README como mapa

Abra o README antes de explorar uma pasta.

O README deve informar:

- finalidade da pasta;
- arquivos existentes;
- resumo curto de cada entrada;
- qual arquivo está ativo;
- ordem cronológica quando aplicável;
- restrição de acesso ou conhecimento.

A regra é:

> **O README indica onde procurar; o arquivo indicado contém a informação completa.**

Não trate uma linha de índice como substituta da fonte quando a decisão depender de detalhes.

## 6. Consulta do estado atual

estado/atual.md é a primeira fonte sobre o presente.

Use-o para:

- momento;
- local;
- participantes;
- posição;
- PV e PA atuais;
- Estados e efeitos;
- intenções persistentes;
- processos e prazos;
- objetos relevantes;
- diferenças atuais de conhecimento;
- fios ativos;
- ponto de retomada.

O estado atual é um resumo operacional. Se ele mencionar uma informação histórica sem detalhe suficiente, consulte o livro. Se mencionar uma verdade permanente, consulte a ficha ou o mundo quando a precisão for necessária.

Não conclua que algo nunca aconteceu apenas porque não está no estado atual.

## 7. Consulta de personagens

Antes de decidir, narrar capacidade ou representar uma personagem, abra sua ficha.

A ficha responde:

- quem ela é;
- como aparenta;
- o que tende a querer e evitar;
- quais relações reconhece;
- o que sabe de forma estável;
- quais Atributos e Perícias possui;
- quais Poderes, Recursos e itens possui;
- quais limitações permanentes se aplicam;
- quem controla suas decisões.

Depois combine a ficha somente com:

- estado atual próprio;
- intenção atual;
- fatos que consegue perceber;
- conhecimento legitimamente adquirido.

Não use ficha alheia como conhecimento da personagem consultada.

Ao trocar de personagem, troque também o pacote decisório. Não deixe informação da personagem anterior contaminar a seguinte.

## 8. Consulta do mundo

Abra mundo/README.md para localizar o arquivo temático adequado.

Consulte o mundo quando precisar confirmar:

- lugar;
- organização;
- cultura;
- tecnologia;
- fenômeno;
- regra interna do cenário;
- acontecimento estrutural;
- relação pública entre elementos do mundo.

O mundo informa a verdade técnica. Ele não prova que uma personagem conhece essa verdade.

Antes de usar a informação numa decisão de personagem, confirme como ela aprendeu ou percebeu o fato.

## 9. Consulta do mestre

Abra mestre/ somente quando a função atual exigir conhecimento reservado.

Pode ser necessário para:

- julgar uma ação contra segredo existente;
- movimentar plano adversário;
- conferir prazo oculto;
- aplicar capacidade desconhecida;
- preservar identidade secreta;
- verificar ameaça ou consequência preparada;
- salvar alterações reservadas.

Ao decidir por personagem, forme seu pacote sem o conteúdo reservado que ela desconhece.

~~~text
IA técnica consultou o mestre
≠ personagem recebeu o conhecimento
~~~

Não revele material reservado na narração antes de percepção, descoberta ou consequência legítima.

## 10. Consulta do livro

O livro é a memória integral, mas deve ser consultado seletivamente.

Primeiro abra livro/README.md e procure:

- capítulo;
- período;
- local;
- personagem;
- acontecimento;
- relação;
- objeto;
- descoberta;
- frase ou termo distintivo.

Depois abra somente o capítulo ou conjunto pequeno de capítulos indicado.

Use o livro para responder:

- o que aconteceu;
- em que ordem;
- quem estava presente;
- quem falou;
- quem pensou;
- o que foi revelado;
- como uma relação mudou;
- quando um objeto apareceu ou foi perdido;
- como se chegou ao estado atual.

Não releia toda a campanha quando uma busca dirigida puder localizar a resposta.

## 11. Leitura do formato literário

No livro:

~~~text
texto sem marcador
→ narração canônica.

[Will] —
→ fala audível de Will.

[Will, pensa] —
→ pensamento privado de Will.

[Will, telepatia para Ana] —
→ comunicação mental dirigida a Ana.

[Will, escreve] —
→ conteúdo escrito por Will.

[Voz desconhecida] —
→ fala cuja origem ainda não estava identificada.
~~~

Uma fala pode se tornar conhecimento de quem tinha condições de ouvi-la.

Um pensamento permanece privado.

Uma comunicação dirigida pertence somente aos destinatários capazes de recebê-la.

A IA deve considerar posição, distância, sentidos, ruído, idioma, capacidade e contexto antes de distribuir conhecimento.

## 12. Continuidade literária imediata

Para continuar uma cena sem mudança brusca de voz ou posição:

1. consulte o ponto de retomada em estado/atual.md;
2. identifique o capítulo em andamento;
3. abra o trecho final do capítulo quando o estado não preservar fala, gesto ou ritmo suficientes;
4. confira quem falou ou agiu por último;
5. retome depois do último fato estabelecido;
6. não repita nem antecipe a próxima decisão.

Não é necessário abrir o capítulo inteiro se o trecho final e o estado atual forem suficientes.

## 13. Consulta por tipo de tarefa

### Resolver uma ação

Abra:

~~~text
regras-basicas.md
estado/atual.md
ficha de quem age
ficha ou valor necessário de quem se opõe
arquivo específico citado pela ação, se houver
~~~

Não abra o livro salvo se o presente já contém todos os dados.

### Narrar uma sentença

Abra:

~~~text
narrador-ia.md
sentença ou resultado estabelecido
estado atual relevante
fichas necessárias para voz, aparência e capacidade
trecho final do capítulo, quando houver continuidade direta
~~~

### Decidir por uma personagem IA

Abra:

~~~text
personagens-ia.md
ficha da própria personagem
estado atual que ela conhece
intenção atual
fontes específicas de conhecimento legítimo
~~~

Não abra material reservado para melhorar a decisão.

### Criar ou revisar personagem

Abra:

~~~text
criacao-de-personagem.md
regras-basicas.md
README da campanha
mundo necessário ao conceito
fichas relacionadas, somente quando a relação exigir
~~~

### Pesquisar acontecimento antigo

Abra:

~~~text
livro/README.md
capítulo indicado pelo índice
capítulos adjacentes somente se a sequência exigir
~~~

### Salvar

Abra:

~~~text
salvamento.md
arquivos alterados pela sentença
READMEs das pastas afetadas
capítulo em andamento
estado/atual.md
~~~

## 14. Consulta histórica dirigida

Quando a pergunta for ampla, reduza-a antes de abrir arquivos.

Exemplo:

~~~text
Pergunta: “Como Will e Ana chegaram a confiar um no outro?”

Buscar:
1. relações atuais nas duas fichas;
2. menções a Will e Ana no índice do livro;
3. capítulos em que a relação mudou;
4. cenas específicas de confiança, conflito ou reconciliação.
~~~

Extraia uma linha cronológica dos fatos necessários. Não confunda interpretação posterior com aquilo que cada personagem sabia naquele momento.

Se a busca não encontrar a resposta, declare a lacuna. Não complete automaticamente com convenção de gênero.

## 15. Prioridade e conflito entre fontes

Use a seguinte ordem de autoridade:

1. correção explícita mais recente já aceita;
2. regras universais para procedimentos mecânicos;
3. ficha atual para identidade e capacidades permanentes;
4. mundo atual para verdades estáveis;
5. mestre para verdade reservada e processos ocultos;
6. estado atual para condições e processos presentes;
7. livro para acontecimentos históricos;
8. improvisação neutra somente onde nenhuma fonte definiu.

Essa ordem não apaga a dimensão temporal.

Exemplo:

- o livro pode dizer que uma personagem possuía uma espada no capítulo 2;
- a ficha atual pode dizer que ela não possui mais a espada;
- o estado atual informa onde a espada está agora;
- as três informações podem estar corretas em momentos diferentes.

Quando houver contradição real:

1. verifique datas e momento da fonte;
2. procure correção posterior;
3. preserve fatos não conflitantes;
4. não transforme erro em novo cânone;
5. peça esclarecimento somente se a decisão depender da parte irresolvida.

## 16. Conhecimento técnico e conhecimento ficcional

A IA pode precisar ler todas as fontes relevantes para operar corretamente. Isso não concede onisciência às personagens.

Separe sempre:

~~~text
VERDADE TÉCNICA
→ o que as fontes estabelecem.

CONHECIMENTO DA PERSONAGEM
→ o que ela aprendeu ou percebeu.

INFORMAÇÃO DO JOGADOR
→ o que foi mostrado fora da ficção.

PERCEPÇÃO ATUAL
→ o que está disponível nesta cena.
~~~

Antes de uma personagem usar um fato, deve existir uma origem legítima:

- presenciou;
- ouviu;
- leu;
- recebeu comunicação;
- descobriu;
- deduziu com base suficiente;
- já possuía como conhecimento registrado.

## 17. Economia de contexto

Para manter decisões rápidas e precisas:

- carregue arquivos universais uma vez por sessão ou contexto estável;
- mantenha estado/atual.md disponível;
- carregue somente fichas relevantes;
- prefira índices antes de pastas inteiras;
- consulte capítulos por acontecimento, não por curiosidade geral;
- descarte pacotes de personagens depois da decisão;
- não duplique trechos grandes na memória operacional;
- resuma para raciocinar, mas volte à fonte antes de afirmar detalhe exato;
- não carregue arquivos de criação durante jogo comum;
- não carregue mestre quando a tarefa não precisa de material reservado.

Economia de contexto não autoriza ignorar uma fonte necessária.

## 18. Arquivo ausente ou incompleto

Se um arquivo esperado não existir:

- verifique o README da pasta;
- procure referência alternativa;
- confira se a informação ainda não foi criada;
- não invente conteúdo para preencher o arquivo;
- use salvamento.md para criar a estrutura quando a criação estiver autorizada;
- peça informação apenas quando a ausência impedir decisão segura.

Se o estado atual estiver incompleto, consulte o trecho final do capítulo em andamento e as fichas relevantes para reconstruir somente o necessário. Depois atualize o estado conforme as regras de salvamento.

## 19. Verificação rápida

Antes de agir, confirme:

~~~text
1. Estou na campanha correta?
2. Abri o README da campanha?
3. Abri o estado atual?
4. Sei o ponto exato de retomada?
5. Carreguei somente as fichas relevantes?
6. Preciso realmente consultar mundo, mestre ou livro?
7. Usei o índice antes de abrir arquivos históricos?
8. Separei verdade técnica de conhecimento da personagem?
9. Alguma fonte mais recente corrigiu a anterior?
10. Falta uma informação indispensável ou apenas um detalhe neutro?
11. Estou prestes a reler conteúdo desnecessário?
12. Consigo indicar de qual fonte veio cada fato importante?
~~~

## Regra final

> **Consultar é carregar o mínimo suficiente para decidir corretamente. A IA começa pelas regras necessárias, pelo README da campanha e pelo estado atual; abre fichas conforme as personagens entram em foco; usa os READMEs para localizar mundo, mestre e livro; pesquisa a memória histórica de forma dirigida; e nunca transforma acesso técnico em conhecimento da personagem.**
