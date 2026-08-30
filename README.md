# Landing page de briefing — nullvision

Página única (`index.html`), sem dependências externas além de fontes do Google (carregam normal quando publicada — só não carregam aqui no ambiente de teste, sem internet). Cliente escolhe a categoria (Cinematic/Motion/Design), preenche o formulário (só nome e e-mail são obrigatórios, o resto é opcional/livre) e envia — o envio vai direto pro seu e-mail via [Formspree](https://formspree.io) (chave já configurada: `mgaevrln`).

## Publicar no GitHub Pages (~5 min, sem conta técnica)

1. Crie uma conta em [github.com](https://github.com) (se ainda não tiver).
2. Crie um repositório novo — pode chamar `nullvision-briefing` — marcado como **Public** (Pages grátis exige público em conta free).
3. Nesse repositório, clique em **Add file → Upload files** e suba o arquivo `index.html` (direto na raiz do repositório, não dentro de subpasta).
4. Vá em **Settings → Pages**. Em "Build and deployment", selecione **Deploy from a branch**, branch **main**, pasta **/ (root)**. Salve.
5. Espere ~1 minuto. O GitHub mostra a URL pública, algo como `https://SEU-USUARIO.github.io/nullvision-briefing/`.
6. Acesse essa URL, preencha o formulário de teste e envie. O Formspree manda um e-mail de **confirmação** pra `contato.mateusaraujom@gmail.com` na primeira submissão — precisa clicar no link de confirmação pra ativar o recebimento definitivo dos briefings.

Depois disso, é só divulgar esse link (bio do Instagram, WhatsApp, proposta comercial) — todo briefing enviado cai direto no seu e-mail, com o assunto `Novo briefing — [Categoria] — [Nome do projeto]`.

## Como o Claude pode processar os briefings automaticamente

Assim que os e-mails começarem a chegar, é possível pedir pro Claude (com o Gmail já conectado) buscar por assunto `Novo briefing —`, extrair as respostas e atualizar `docs/06_CLIENTES.md` / `docs/07_PROJETOS.md` sozinho — inclusive numa rotina automática (verificação diária, por exemplo). Isso ainda não está configurado; é um passo seguinte, a ativar quando você quiser.

## Editar o formulário depois

Todo o conteúdo (perguntas, categorias, textos) está em HTML/CSS/JS simples dentro de `index.html` — qualquer ajuste pode ser pedido ao Claude, que edita o arquivo e você re-sobe no GitHub (ou substitui o arquivo direto pela interface do GitHub, sem precisar mexer em nada técnico).
