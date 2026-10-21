# PROJETO: LP Viver de Terapia (MP-Le01)

- Marca: Psicologia em Doses, Nathália Andrade. Idioma pt-BR.
- Página: `psiprime-a/index.html`, arquivo único. Produção: `psicologiaemdoses.com.br/mp-Le01/psiprime-a/`.
- Deploy: Hostinger, diretório `mp-Le01` (clone do repositório). Auto-deploy do hPanel já está ocupado pelo `fped-003`, então aqui o deploy é manual (pull via conector).
- Noindex/nofollow: sim (página de anúncio).
- Config no começo do `<script>` (objeto CONFIG): GTM_ID `GTM-W4N7VFD9` (container compartilhado com o Destrave, separar por URL no GTM), CHECKOUT_URL Hotmart `Y108097135Q` (off z7z8hjjn), PRICE_CHANGES_AT pendente, CRP 2331-4 (informado pela Nathália).
- Eventos: `cta_click` (cta_id) e `begin_checkout` (BRL 29.97). Clarity: instalar pelo GTM.
- Pendências: link do checkout Hotmart, data da virada de preço, CRP, nomes e autorização das 6 alunas dos prints, revisão jurídica, página de obrigado (link do grupo WhatsApp).

## Inventário de páginas
| URL de produção | Objetivo | Evento | Observação |
|---|---|---|---|
| `psicologiaemdoses.com.br/mp-Le01/psiprime-a/` | LP do ingresso (workshop 07/11) | `cta_click`, `begin_checkout` | publicada, checkout Hotmart configurado |
| `psicologiaemdoses.com.br/mp-Le01/obrigado-a/` | Obrigado pós-compra do ingresso | `whatsapp_click`, `add_to_calendar_click`, `support_click` | pendente: WHATSAPP_GROUP_URL e SUPPORT_URL no CONFIG |


## Atualizacao 21/10/2026
- Pagina de obrigado oficial: https://psicologiaemdoses.com.br/cp-Le01/boas-vindas-a-ldobg/ (branch `cp-le01`, pasta `cp-Le01` no servidor).
- `/mp-Le01/obrigado-a/` agora apenas redireciona para a URL oficial.
- Link curto da LP: https://psicologiaemdoses.com.br/workshop/ (branch `link-workshop`).
- LP de vendas oficial: https://psicologiaemdoses.com.br/cp-Le01/inscricao-a/ (branch `cp-le01`). `/mp-Le01/psiprime-a/` e `/workshop/` apenas redirecionam para ela.
