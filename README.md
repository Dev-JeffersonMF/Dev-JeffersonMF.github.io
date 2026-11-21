# dev-Jefferson — portfólio (GitHub Pages)

Página estática do portfólio de Jefferson Macedo Fernandes, publicada em
https://dev-jeffersonmf.github.io/

## Estrutura

- `index.html` — página completa (HTML, CSS e JS inline, sem dependências externas).
- `img/` — capturas dos projetos, redimensionadas e otimizadas.
- `PRODUCT.md` — contexto de produto (fatos preservados).
- `DESIGN.md` — decisões visuais do mundo "portal cinematográfico".
- `.impeccable/` — contrato da superfície e capturas de revisão.

## O que mudou na v2

- Redesign completo: de parede de galeria para **portal cinematográfico** inspirado na gramática do League of Legends (luz, escala e tempo — sem arte ou marca copiada).
- Hero com 5 camadas de parallax, partículas douradas, grão e vinheta.
- Título em serif dourado com relevo, CTA ciano e botão de agendamento.
- Trabalhos como "missões concluídas" em molduras angulares com varredura de luz.
- **Removidos os links de aplicativos/repositórios dos projetos**: a página apenas apresenta o trabalho e o autor.
- Loader de abertura com barra dourada e animações em cascata.
- Totalmente responsivo e com `prefers-reduced-motion`.

## Rodar localmente

```bash
python3 -m http.server 8000
```

Abra `http://localhost:8000`.

## Publicar

```bash
git add -A
git commit -m "Redesign: portal cinematográfico"
git push
```

O GitHub Pages publica a partir da branch `main`.
