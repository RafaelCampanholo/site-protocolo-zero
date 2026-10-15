# site-protocolo-zero

Página de vendas do **Protocolo Zero Cólica** (HTML estático, um único arquivo: `index.html`).

## Configurar os links de checkout

No final do `index.html`, edite o objeto `CHECKOUT` com os links da sua plataforma (Ticto, Kiwify, Hotmart…):

```js
var CHECKOUT = {
  essencial: "https://...", // R$10
  premium:   "https://...", // R$39,90
  upsell:    "https://..."  // Premium com desconto, R$19,90
};
```

Parâmetros da URL (UTMs) são repassados automaticamente para o checkout.

## Publicação

O site é estático (sem build). A Hostinger publica o conteúdo da branch `main`
na pasta `public_html` pela integração Git do hPanel: cada merge na `main` atualiza o site.
