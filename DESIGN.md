# Design — dev-Jefferson (portal cinematográfico)

## Mundo

O portfólio é um **portal cinematográfico de fantasia escura**. A primeira viewport é uma cena em camadas — céu em tempestade, cordilheiras em profundidade, silhuetas laterais e um nome em dourado com relevo — que se abre como a abertura de um jogo. Os trabalhos são "missões concluídas" em molduras angulares sob luz. A referência de gramática é o League of Legends (luz, escala, tempo); nenhuma arte ou marca foi copiada.

## Tokens

| Token | Valor |
| --- | --- |
| `void` | `#0a0d14` — fundo, carvão profundo |
| `void-2` | `#0e1420` — superfícies elevadas |
| `panel` | `#121a28` — placas de projeto |
| `gold` | `#d4af37` — primeira voz de luz: nome, relevo, detalhes |
| `gold-deep` | `#8a6a1c` — sombra do relevo |
| `cyan` | `#39c5e8` — segunda voz de luz: CTA de agendamento, rótulos |
| `mist` | `#8e9aab` — névoa do horizonte e texto secundário |
| `ink` | `#f2f4f7` — texto principal |
| `line` | `rgba(212,175,55,.22)` — filetes dourados |
| `shadow` | `0 28px 70px -24px rgba(0,0,0,.9)` — profundidade |
| `ease` | `cubic-bezier(.16,1,.3,1)` — singular curva de movimento |
| `clip` | `polygon(16px 0,100% 0,100% calc(100% - 16px),calc(100% - 16px) 100%,0 100%,0 16px)` — canto angular recorrente |

## Tipografia

Sem fontes externas. Display em pilha serif do sistema (Georgia), peso 700 e tracking `-.045em`, com relevo feito de camadas de `text-shadow` — nunca gradiente de texto. Corpo em sans do sistema. Rótulos em caixa alta com tracking `.16em` a `.3em`.

## Composição

- Topbar fixa, preta, translúcida com blur: marca à esquerda, navegação ao centro, CTA ciano em cápsula à direita.
- Hero de `100svh`: cinco camadas com parallax (céu, névoa, duas cordilheiras, silhuetas), 26 partículas douradas, grão SVG e vinheta; nome central, subtítulo, botão dourado, indicador "ROLAR".
- Sobre: texto editorial à esquerda, selo `12+` angular à direita, stack em etiquetas.
- Trabalhos: 8 projetos em grade 12 colunas com tamanhos alternados, molduras angulares, varredura de luz no hover e revelaçãoBlur ao entrar na viewport. **Sem links externos dos projetos** — a página mostra o trabalho, não distribui apps.
- Contato: portal iluminado com formulário funcional via `mailto:`.

## Movimento

Um momento autoral orquestrado: a cena abre com o loader (barra dourada que carrega, 1,45 s), o nome/lede/botão sobem com blur em cascata, as camadas fazem parallax no scroll, as seções revelam com blur, as molduras varrem luz no hover e as partículas derivam. O indicador de rolagem pulsa. Tudo respeita `prefers-reduced-motion`.

## Acessibilidade e performance

Contraste verificado, foco visível em ciano, `alt` nas imagens, `loading="lazy"`, formulário com `aria-live`, HTML/CSS/JS estáticos sem dependências de rede, grão e relevo desenhados em SVG/CSS.

## Histórico

Substitui o mundo anterior "gallery wall" (páginas claras, moldura passe-partout, luz de teto). Esta é uma substituição de identidade visual; os fatos, nomes e descrições dos projetos foram preservados.
