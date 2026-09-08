# Trade no ritmo da FTW — 75LAB × FTW

Apresentação comercial em HTML (arquivo único) da proposta de **fee de planejamento,
criação e gestão de trade** da 75LAB para a FTW. Resumo dos 24 slides do PPTX R03 em
**9 telas** com racional de começo, meio e fim.

## Estrutura

| # | Tela | Parte |
|---|------|-------|
| 01 | Trade no ritmo da FTW | Abertura |
| 02 | O que ouvimos (diagnóstico) | 01 · Contexto |
| 03 | A carteira de 6 frentes | 02 · A solução |
| 04 | Capacidade: 180 h/mês | 02 · A solução |
| 05 | Como trabalhamos juntos | 02 · A solução |
| 06 | Exemplo aplicado · Natal | 03 · A prova |
| 07 | Por onde começamos + 90 dias | 03 · A prova |
| 08 | Investimento proposto | 04 · A decisão |
| 09 | Ideia boa é a que acontece | 04 · A decisão |

## Como usar

Abra `index.html` em qualquer navegador. Navegação: **← →**, **espaço**, **Home/End**,
swipe no mobile, **M** abre o índice, **Esc** fecha. `index.html#6` abre direto na tela 6.
O botão **Baixar PDF** usa a impressão do navegador (9 páginas, 1600×900 paisagem).

## Interações

- Cartões com borda vermelha ao passar o mouse **abrem detalhe ao clicar** (telas 02, 03 e 07)
- Tela 04: alternador **Por entregável / Por especialidade** — as mesmas 180 h em duas leituras
- Tela 08: alternador **Contempla / Não contempla**
- Botões de CTA saltam entre telas (`data-go="N"`, índice base zero)

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
idêntico em qualquer resolução. Imagens embutidas em base64. Fontes via Google Fonts.
