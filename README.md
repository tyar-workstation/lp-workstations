# LP Workstations Tyar

Landing page da campanha própria de Google Ads (workstations sob medida).

- `index.html`: página completa (fontes, imagens e scripts embutidos). Já carrega o Google Tag Manager `GTM-N52R2WH`.
- `CNAME`: domínio da página no GitHub Pages (`workstations.tyar.com.br`). Troque se for usar outro subdomínio.

## Publicar no GitHub Pages

1. Crie um repositório (ex.: `tyar/lp-workstations`) e envie estes arquivos para a branch `main`.
2. No repositório: Settings > Pages > Source: "Deploy from a branch", branch `main`, pasta `/ (root)`.
3. No DNS do domínio tyar.com.br, crie um registro **CNAME** `workstations` apontando para `<usuario-ou-org>.github.io`.
4. Volte em Settings > Pages, confirme o domínio e marque "Enforce HTTPS" quando liberar (pode levar alguns minutos).

## Ligar o formulário ao Omie

No fim do `index.html`, preencha `CONFIG.endpoint` com a URL `/exec` do Apps Script "Tyar | Leads LP → Omie" e `CONFIG.k` com o mesmo `LP_SEGREDO` das propriedades do script.
