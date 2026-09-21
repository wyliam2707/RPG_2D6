# RPG_2D6

Este repositório contém um sistema de RPG narrativo 2D6 pensado para ser usado por jogador humano e IA.

O objetivo não é criar uma regra específica para cada situação. O sistema usa **regras universais** que devem ser aplicadas ao contexto da cena sempre que forem compatíveis.

> **Não invente uma regra nova quando uma regra geral já resolver a situação.**

## Como usar este repositório

Uma IA sem contexto deve primeiro identificar o que precisa fazer e abrir somente os arquivos necessários.

### Para criar uma campanha

Abra:

1. `criacao-de-campanha.md`
2. `criacao-de-personagem.md`, quando precisar criar fichas
3. `personagens-ia.md`, se houver personagens controlados por IA
4. `salvamento.md`, para criar a estrutura em `campanhas/`

Não comece escrevendo uma história pronta. A criação da campanha prepara premissa, direção, situação inicial, personagens e forças em movimento. A história deve surgir durante o jogo.

### Para retomar uma campanha existente

Abra primeiro:

1. `consulta.md`
2. `regras-basicas.md`
3. `narrador-ia.md`
4. `personagens-ia.md`
5. `campanhas/nome-da-campanha/README.md`

Depois siga a rota indicada por `consulta.md` e carregue somente o estado, fichas e arquivos necessários para a situação atual.

Não releia toda a campanha por padrão.

### Para narrar uma sessão

Use:

- `regras-basicas.md` para possibilidade, testes, escala, PA, efeitos e resolução mecânica;
- `narrador-ia.md` para interpretar declarações, conduzir cenas e transformar resultados em narrativa;
- `personagens-ia.md` para decisões de personagens controlados por IA;
- os arquivos da campanha para fatos, estado, mundo, personagens e continuidade.

O Narrador julga a realidade e os resultados. Ele não decide voluntariamente pelo personagem do jogador.

### Para criar ou revisar um personagem

Use:

1. `criacao-de-personagem.md`
2. `regras-basicas.md`
3. `personagens-ia.md`, se o controle for IA

A ficha define capacidades, identidade, conhecimento e tendências. Não conceda capacidades apenas porque combinam com um arquétipo, gênero ou personagem famoso.

### Para salvar uma sessão

Use:

- `salvamento.md`
- `continuidade.md`, quando houver fechamento do dia ou encerramento de capítulo

As campanhas ficam em:

`campanhas/`

O salvamento separa:

- presente ativo em `estado/`;
- fichas em `personagens/`;
- verdades estáveis em `mundo/`;
- material reservado em `mestre/`;
- acontecimentos completos em `livro/`.

## Arquivos principais

| Arquivo | Função |
|---|---|
| `regras-basicas.md` | Motor mecânico universal do sistema |
| `narrador-ia.md` | Condução de cena, julgamento e narração |
| `personagens-ia.md` | Decisão e interpretação de personagens controlados por IA |
| `criacao-de-personagem.md` | Criação e revisão de fichas |
| `criacao-de-campanha.md` | Preparação e direção de campanhas |
| `consulta.md` | Carregamento e busca de contexto |
| `salvamento.md` | Organização e atualização dos arquivos da campanha |
| `continuidade.md` | Fechamento do dia, agenda, encerramento de capítulo e ressincronização |
| `campanhas/` | Armazenamento das campanhas |

## Princípios operacionais

Ao usar este sistema:

- trate a declaração do jogador como **intenção**, não como resultado;
- verifique primeiro se a ação é possível;
- só role quando houver incerteza, oposição ou necessidade real de medir a execução;
- use somente **Perícia Final** nos testes;
- aplique escala, PA, dificuldade, alcance, área, estados e efeitos pelas regras universais;
- não crie subsistemas para situações que o sistema já consegue resolver;
- não importe regras de outros RPGs;
- não invente falha mínima, falha crítica ou chance automática de erro quando o sistema não disser isso;
- não transforme sucesso parcial em falha disfarçada;
- não complete escolhas voluntárias do jogador por conta própria;
- mantenha separado o que a IA sabe do que cada personagem sabe;
- preserve fatos estabelecidos e consulte a fonte correta quando houver dúvida;
- use `consulta.md` para evitar carregar arquivos desnecessários;
- use `salvamento.md` para manter a campanha canônica organizada;
- use `continuidade.md` para fechamento do dia, agenda e checkpoints de capítulo.

## Regra de prioridade

Se houver dúvida sobre como proceder:

1. consulte o arquivo responsável pela função atual;
2. aplique as regras universais existentes;
3. use a situação concreta da ficção para interpretar a aplicação;
4. só peça esclarecimento quando faltar uma decisão realmente necessária.

> **As regras definem as ferramentas. A situação define como elas se aplicam.**
