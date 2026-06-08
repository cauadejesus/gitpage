# Site criado para mostrar meu portfólio

Este projeto publica o site estático gerado em `dist/` no GitHub Pages.

## Deploy automático

- O GitHub Actions está configurado em `.github/workflows/deploy.yml`
- A cada `git push` na branch `main`, o projeto é compilado e o conteúdo de `dist/` é publicado no Pages
- A URL pública é:

https://cauadejesus.github.io/gitpage/

## Como usar localmente

1. Instale dependências:
   ```bash
   npm ci
   ```
2. Gere o site:
   ```bash
   npm run build
   ```
3. Inicie o servidor de desenvolvimento:
   ```bash
   npm run start
   ```
