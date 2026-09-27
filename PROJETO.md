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
- **Projeto na Vercel:** `lp-01.lp.vd.fped-003.lp-de-venda-direta-a-vsl` — **ainda não conectado a este repositório** (pendente, ver conversa)
- **Domínio(s) de produção:** pendente
- **Fluxo de git:** branch por página → preview da Vercel → aprovação no preview → merge na `main` = no ar
- **Preview protegido?** pendente confirmar (padrão da Vercel é pedir login no preview)

## Medição

- **Container do GTM** (`GTM-XXXXXXX`) e quem pode publicar: pendente — o código já está com o snippet do GTM instalado, mas com `GTM-XXXXXXX` de placeholder até o id real chegar
- **Projeto do Clarity** (id) e conta dona: `yp3175pi2j` — instalado no `index.html`, conta dona pendente de confirmação
- **Banner de consentimento (LGPD)?** pendente
- **Evento de conversão padrão:** `begin_checkout` (página de venda direta, sem formulário — o clique no CTA da oferta manda direto pro checkout)
- **Outros eventos de conversão:** `cta_click` em cada botão (`hero`, `oferta`, `fechamento`) como evento de intenção

## Destino do lead

- não se aplica — página de venda direta (VSL), sem formulário. A conversão é o clique que leva ao checkout.

## Checkout

- **Link de checkout:** pendente — o botão da oferta (`#oferta`) e o botão de fechamento estão com `CHECKOUT_URL = null` no `index.html`; enquanto isso, o clique só rola a página até a oferta em vez de navegar pra lugar nenhum.
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
| (ainda não publicada) | Venda direta do Destrave (VSL) | `begin_checkout` | — | — |
