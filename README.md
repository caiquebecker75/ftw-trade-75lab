# Trade no ritmo da FTW — 75LAB × FTW

Apresentação comercial em HTML (arquivo único) da proposta de **fee de planejamento,
criação e gestão de trade** da 75LAB para a FTW. Cada tela carrega **um visual próprio**
e o conjunto monta um argumento: por que o fee é necessário, o que ele é, e o que a FTW
ganha no curto e no médio prazo.

## Fluxo de raciocínio

| # | Tela | Visual que carrega a tela | Parte |
|---|------|---------------------------|-------|
| 01 | Trade no ritmo da FTW | totem FTW + feixes diagonais | Abertura |
| 02 | A FTW cria rápido, o trade chega devagar | constelação de demandas convergindo numa agenda só | 01 · Por que um fee |
| 03 | Cada campanha recomeça do zero | quatro ciclos idênticos, cortados entre si | 01 · Por que um fee |
| 04 | De demanda avulsa a uma fila só | comparativo: caixas dispersas → fila priorizada | 01 · Por que um fee |
| 05 | 180 horas já reservadas | medidor radial 36 h rotina / 144 h entrega | 01 · Por que um fee |
| 06 | Em 60 dias, o caos vira calendário | trilho temporal com 4 estações (semana 1 → dia 60) | 02 · Ganhos |
| 07 | Trade deixa de ser esforço e vira ativo | escada ascendente do mês 3 ao mês 6 | 02 · Ganhos |
| 08 | A árvore de potes vira pacote pronto | foto de loja em sangria + sequência de 6 tempos | 03 · A prova |
| 09 | Custo previsível no lugar de imprevistos | preço em tipografia gigante + escopo alternável | 04 · A decisão |
| 10 | Ideia boa é a que acontece | fecho tipográfico + 3 passos | 04 · A decisão |

O argumento em uma linha: **02** mostra a dor → **03** mostra o custo dela → **04** mostra a
virada → **05** define o que é o fee → **06 e 07** entregam os benefícios datados →
**08** prova com um caso real → **09 e 10** fecham.

## Como usar

Abra `index.html` em qualquer navegador. Navegação: **← →**, **espaço**, **Home/End**,
swipe no mobile, **M** abre o índice, **Esc** fecha. `index.html#6` abre direto na tela 6.
O botão **Baixar PDF** usa a impressão do navegador (10 páginas, 1600×900 paisagem).

## Interações

- CTAs que saltam entre telas (`data-go="N"`, índice base zero)
- Tela 09: alternador **Está no fee / Fica à parte**
- Índice em overlay com as 10 telas, contadores animados, cursor customizado
- Cada tela anima na entrada: constelação flutuante, fila que entra, medidor que desenha,
  trilho que preenche, escada que sobe

## Marca

- **FTW** — preto `#08080A`, vermelho de marca `#E1091E` (amostrado das embalagens e do
  logotipo oficial), branco. Logotipo reconstruído em CSS: itálico condensado + slash vermelho.
  Tom de voz: *Feito para Vencer* / *#FORTHEWIN* / *Qualidade que se vê no resultado*.
- **75LAB** — lime `#B2F00F`, presente no topo de todas as telas e no fecho.
- Tipografia: **Anton** (rótulos, números, eyebrows) + **Inter** (títulos e texto) — Inter é
  a família usada no site da FTW.

Imagens de repertório extraídas da apresentação FTW anterior. Não comprovam implantação
nem resultado de vendas.

## Técnico

Arquivo único, sem build. Palco fixo de 1600×900 escalado por transform — o layout é
idêntico em qualquer resolução. Visuais em SVG e CSS puro (nenhuma biblioteca); as
animações disparam por `.slide.on`, sem observadores. Imagens embutidas em base64.
Fontes via Google Fonts. Respeita `prefers-reduced-motion`.
