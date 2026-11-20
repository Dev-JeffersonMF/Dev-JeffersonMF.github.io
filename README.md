# dev-Jefferson — portfólio (GitHub Pages)

Página estática do portfólio de Jefferson Macedo Fernandes, publicada em
https://dev-jeffersonmf.github.io/

## Estrutura

- `index.html` — página completa (HTML, CSS e JS inline, sem dependências externas).
- `nexo-icon.png` — ícone do Nexo redimensionado para 420 px.
- `img/` — capturas dos projetos, redimensionadas e otimizadas.
- `PRODUCT.md`, `DESIGN.md`, `.impeccable/` — contexto de produto, decisões visuais e contrato da superfície.

## Rodar localmente

```bash
python3 -m http.server 8000
```

Abra `http://localhost:8000`.

## Publicar

```bash
git add -A
git commit -m "Redesign: galeria de trabalhos e projeto Nexo"
git push
```

O GitHub Pages publica a partir da branch `main`.

## Projeto Nexo

O card do Nexo usa o link público: https://github.com/Dev-JeffersonMF/nexo-app
