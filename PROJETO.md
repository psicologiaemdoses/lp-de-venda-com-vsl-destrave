# PROJETO: a ficha deste projeto

A skill lê este arquivo antes de todo trabalho. Preencha uma vez e mantenha em dia.

- Campo que não se aplica: escreva **"não se aplica"**. Campo vazio faz a skill parar e perguntar.
- Nada de senha, token ou chave aqui: este arquivo vai pro git. Ids públicos (GTM, pixel, Clarity)
  podem ficar.

## Marca e conteúdo

- **Marca / cliente:** Psicologia em Doses — Nathália Andrade (produto: Destrave)
- **Idioma das páginas:** pt-BR
- **Onde está a marca** (logo em SVG/PNG, cores em hex, fontes com licença, banco de fotos reais): pendente — cores usadas por enquanto: `--cream #FDF6E3`, `--ink #15140E`, `--lime #E7ED4D`, `--coral #D9486A`; fonte Sora (Google Fonts)
- **Onde está o briefing** (público, dores, voz, palavras proibidas): pendente — copy atual veio do rascunho de design aprovado (artifact "Destrave — LP de Venda Direta A (VSL)")
- **Exclusões** (concorrente que não pode aparecer em foto, termo proibido, promessa que não se faz): pendente
- **Regras de escrita:** sem travessão (—) na copy, porque denuncia texto de IA; use vírgula,
  ponto, dois-pontos ou parênteses.

## Site e deploy

- **Repositório (git):** psicologiaemdoses/lp-de-venda-com-vsl-destrave
- **Tipo de site:** HTML estático
- **Onde publica de fato:** hospedagem principal (Hostinger, WordPress) de `psicologiaemdoses.com.br`, via auto-deploy do Git conectado no hPanel. O diretório de destino do auto-deploy é `fped-003` (a raiz do repo vira o conteúdo de `fped-003/`), então cada página vira uma subpasta do repo: `destrave-a/index.html` → `fped-003/destrave-a/`, `boas-vindas-a-vdobg/index.html` → `fped-003/boas-vindas-a-vdobg/`.
- **Vercel:** projeto `lp-01.lp.vd.fped-003.lp-de-venda-direta-a-vsl` existe e fica conectado ao mesmo repositório (preview de branch antes de aprovar), mas a produção real é servida pela Hostinger, não pela Vercel.
- **Domínio(s) de produção:** `psicologiaemdoses.com.br` (site principal em WordPress, hospedagem Hostinger)
- **Fluxo de git:** branch por página → preview (Vercel ou revisão local) → aprovação → merge na `main` → auto-deploy da Hostinger publica em minutos
- **Preview protegido?** não se aplica pro fluxo atual (produção sai direto na Hostinger, não por link de preview da Vercel)

## Medição

- **Container do GTM** (`GTM-XXXXXXX`) e quem pode publicar: pendente — o código já está com o snippet do GTM instalado, mas com `GTM-XXXXXXX` de placeholder até o id real chegar
- **Projeto do Clarity** (id) e conta dona: `yp3175pi2j` — instalado no `index.html`, conta dona pendente de confirmação
- **Banner de consentimento (LGPD)?** pendente
- **Evento de conversão padrão:** `begin_checkout` (página de venda direta, sem formulário — o clique no CTA da oferta manda direto pro checkout)
- **Outros eventos de conversão:** `cta_click` em cada botão (`hero`, `oferta`, `fechamento`) como evento de intenção

## Destino do lead

- não se aplica — página de venda direta (VSL), sem formulário. A conversão é o clique que leva ao checkout.

## Checkout

- **Link de checkout:** Hotmart, `https://pay.hotmart.com/I107780246C?off=mz614nlu&checkoutMode=10` — configurado no `index.html` (`CHECKOUT_URL` e nos dois botões de oferta/fechamento).
- **Onde a VSL está hospedada:** VTurb. O player fica embutido no bloco `#vturb-video` do `index.html`; falta colar o embed real exportado do VTurb.
- **Botão de oferta dentro do vídeo:** é o próprio VTurb que exibe o botão no momento certo do vídeo (configurado lá). Por isso a barra fixa de preço + botão que aparecia desde a entrada da página foi removida do `index.html` — ela fazia o preço aparecer antes da hora.

## Anúncio

| Plataforma | Id (pixel / conta) | Conversão que otimiza (evento, id e rótulo) |
|---|---|---|
| Meta | pendente | pendente |
| Google Ads | pendente | pendente |
| TikTok | pendente | pendente |

- **Antes de renomear evento de conversão**, confira quem otimiza por ele (acima).

## Aprovação

- **Quem aprova** (nome e canal): pendente
- **O que custa e precisa de OK** (ex.: imagem gerada por IA, ferramenta paga): pendente

## Inventário de páginas

| URL de produção | Objetivo | Evento de conversão | Última verificação | Resultado |
|---|---|---|---|---|
| `psicologiaemdoses.com.br/fped-003/destrave-a` | Venda direta do Destrave (VSL) | `begin_checkout` | 2026-09-27 | publicada, GTM ainda com id placeholder |
| `psicologiaemdoses.com.br/fped-003/boas-vindas-a-vdobg` | Página de obrigado pós-compra do Destrave (confirmação + primeira ação, sem formulário) | não se aplica — conversão já disparou no checkout; aqui só `page_view` padrão | 2026-09-27 | publicada, GTM ainda com id placeholder |
