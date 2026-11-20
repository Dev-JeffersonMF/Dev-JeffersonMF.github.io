# Design — dev-Jefferson (gallery wall)

## Mundo

O portfólio é uma parede de galeria: cada projeto é uma obra emoldurada sob luz focada, com uma placa de metadados. O Nexo é a obra de abertura. Não há grade de cards iguais nem hero com botão solto.

## Tokens

| Token | Valor |
| --- | --- |
| `wall` | `#16120f` — fundo da sala, carvão quente |
| `wall-2` | `#1d1814` — campos de formulário |
| `mat` | `#efe9dd` — passe-partout das molduras |
| `ink` | `#f3efe6` — texto sobre a parede |
| `muted` | `#b8ad9c` — texto secundário |
| `brass` | `#c8a35b` — única cor de destaque: obra iluminada, link principal, foco |
| `shadow` | `0 22px 55px -18px rgba(0,0,0,.72)` — elevação neutra |
| `radius` | `2px` — quase sem arredondamento |
| `ease` | `cubic-bezier(.16,1,.3,1)` |

## Tipografia

Sem fontes externas. Corpo e interface em pilha sans do sistema; títulos em pilha serif do sistema, com peso regular e tracking negativo. Nenhum emoji como ícone.

## Composição

- Barra superior discreta com nome e links de seção.
- Primeira viewport: texto à esquerda, obra do Nexo emoldurada à direita; CTA de contato dentro da placa.
- Seções seguintes: sobre/stack em texto corrido; galeria com obras de tamanhos alternados; contato com formulário funcional via mailto.
- Ritmo vertical generoso, mais espaço acima dos títulos do que abaixo.

## Movimento

Um momento autoral: quando cada moldura entra na viewport, a luz sobe (sombra neutra e fundo do frame clareiam). Respeita `prefers-reduced-motion`. Sem animações espalhadas em cada seção.

## Acessibilidade e performance

Contraste verificado, foco visível em latão, textos alternativos nas imagens, `loading="lazy"`, imagens redimensionadas e com provença incorporada, sem dependências de rede.
