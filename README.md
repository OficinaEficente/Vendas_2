# Landing Vendas — Oficina Eficiente

Landing page de vendas do treinamento de Direção Hidráulica da Oficina Eficiente.

## Estrutura

- `public/index.html` — página principal
- `public/styles.css` — estilos
- `public/script.js` — interação, captura de leads, Pixel/GA e Chatfuel
- `worker.js` — Cloudflare Worker + Meta CAPI + config pública
- `wrangler.toml` — configuração do Worker
- `.github/workflows/deploy.yml` — deploy automático no Cloudflare

## Captura de leads

Os leads são salvos no Supabase na tabela `Leads_Vendas` com:

- nome
- whatsapp
- email
- origem

## Integrações

- Supabase
- Meta Pixel
- Meta CAPI
- Google Analytics
- Chatfuel
- Checkout Lia

## Deploy

Push na branch `main` dispara o GitHub Actions para Cloudflare Workers.
