---
title: Teste de publicação automática
tipo: nota
area: grc
status: concluido
publish: true
tags: [teste]
data: 2026-08-22
---

# Teste de publicação automática

Esta é uma nota de teste para confirmar que o fluxo completo está funcionando:

1. Nota criada em `04-Portfolio/` com `publish: true` no frontmatter.
2. O plugin Obsidian Git faz commit-and-sync automático (a cada 10 minutos, ou manualmente via `Ctrl/Cmd+P` → "Git: Commit and Sync").
3. O push chega no GitHub e dispara o workflow `.github/workflows/publish.yml`.
4. O Quartz reconstrói o site a partir de `04-Portfolio/` e publica no GitHub Pages.

Se você está vendo esta página no site publicado, o pipeline está funcionando de ponta a ponta. Pode apagar esta nota (e o arquivo correspondente do repositório) depois de confirmar.
