# Portfólio — Lucas Sousa Galdino

Meu primeiro portfólio, publicado no GitHub Pages e também servido localmente com Node.js e Express.js.

## Requisitos

- Node.js 18 ou superior
- npm

## Executar localmente

```bash
npm install
npm start
```

Acesse `http://localhost:3000`. Para usar outra porta, defina a variável de ambiente `PORT`.

O site original está em `public/index.html` e é servido como conteúdo estático pelo Express.

## Publicar no GitHub Pages

O workflow em `.github/workflows/deploy-pages.yml` publica automaticamente o conteúdo da pasta `public` quando há um push para a branch `main`.

1. Crie um repositório no GitHub e envie este projeto para a branch `main`.
2. No repositório, abra **Settings → Pages** e selecione **GitHub Actions** como fonte de publicação.
3. Acompanhe a execução em **Actions**. Após o primeiro deploy, o endereço do site aparecerá no job concluído e em **Settings → Pages**.

O GitHub Pages hospeda o site estático; ele não executa o servidor Express. Para publicar o HTML, o Express não precisa estar rodando.
