# Metabolismo Reativado · Desafio Jejum 5 em 7

Site estático (sem build): publique a raiz do repositório (Netlify, Vercel ou GitHub Pages).

| Página | Caminho | O que é |
|---|---|---|
| Quiz + oferta | `/` | Teste "idade do metabolismo" (22 telas) → resultado → oferta R$ 27 → checkout Cakto |
| Upsell | `/upsell/` | Fase 2: 21 Dias Sem Sanfona, R$ 37 |
| Obrigado | `/obrigado/` | Confirmação + primeiros passos |

## Configurar (só o bloco CONFIG no topo de cada página)
- `index.html` → `window.M30`: `CHECKOUT_URL` (checkout Cakto do principal) e `META_PIXEL_ID`.
- `upsell/index.html` → `window.MR_UP`: `UPSELL_CHECKOUT_URL` ou o código do upsell 1 clique da Cakto dentro de `#cakto-upsell`, e `META_PIXEL_ID`.
- `obrigado/index.html` → `window.MR_OK`: `META_PIXEL_ID` e `SUPORTE_EMAIL` (opcional).

Na Cakto: página de obrigado do produto principal → `/upsell/`; recusa/compra do upsell → `/obrigado/`.
UTMs da URL do anúncio são repassadas pro checkout.
