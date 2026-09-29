# Tigress Expertise Elétrica: landing page

Landing page em arquivo único (`index.html`), com imagens em `assets/`. Eletricista em Varginha/MG. Status: demo, não publicada.

## Como visualizar
Abra o `index.html` com duplo clique (caminhos relativos). Para conferir no Chrome com a extensão, use `node "_ferramentas/preview-local.mjs" "<esta pasta>"`.

## Estrutura
- `index.html`: HTML + CSS + JS. Seções: hero com fotos e pulso de circuito, faixa de números, sobre, serviços em abas (residencial, predial, industrial), galeria com ampliação, diferenciais, como funciona, sinais de alerta, montador de mensagem para o WhatsApp, avaliações, atendimento, CTA final, rodapé e botão flutuante.
- `assets/`: pata com o raio recortada do logo (`logo-pata.png`), 8 fotos otimizadas, `og.jpg` e `favicon.png`.
- `Copy.txt`: texto da página (fonte da verdade).
- `design-system-tigress-expertise.html` (texto-fonte em `_fontes/`, oculta): design system (preto, dourado #F2B705, Sora + Inter).
- `Imagens/`, `Fotos/`, `Logo/`, `Info para copy/` e os `Link do ...txt`: materiais originais.

## Pendências antes de publicar
- Nome da profissional, anos de experiência, registro (CREA/CFT) e horário: aparecem como `[... A CONFIRMAR]` no site.
- Logo em alta resolução (a original tem 150 px; o arquivo "ChatGPT Image" diz "ENERGY DRINK" e por isso só a pata foi usada).
- Confirmar "a partir de R$ 80,00", a lista de serviços por frente, e que as 8 fotos são da Tigress e podem ser exibidas (têm ~700 px).
- Endereço completo: o Maps lista um apartamento, o site mostra só "Centro, Varginha/MG".
- Fontes carregadas do Google Fonts, como no design system.
