# Design system: Tigress Expertise Elétrica

Base: logo (pata preta com raio dourado), bio do Instagram e fotos de obra (ferramentas amarelas, quadros elétricos, galpão industrial).

## Tom visual em 3 linhas
1. Preto profundo com dourado elétrico: a pata e o raio do logo viram a paleta inteira.
2. Técnico e seguro: tipografia geométrica, cantos firmes, linhas de circuito e pulso de energia como detalhe.
3. Contraste forte entre blocos escuros e creme, com o verde só no botão do WhatsApp.

## 1. Cores

| Token | Hex | Uso |
|---|---|---|
| ink-950 | #08080A | Fundo principal, hero, rodapé |
| ink-900 | #101014 | Seções escuras alternadas |
| ink-800 | #18181E | Cards sobre fundo escuro |
| ink-700 | #24242C | Bordas fortes, campos |
| gold-500 | #F2B705 | Cor de destaque (raio do logo), faixas, ícones |
| gold-400 | #FFC933 | Hover, brilho |
| gold-300 | #FFD966 | Destaques em texto sobre escuro |
| gold-700 | #7A5A00 | Texto de destaque sobre creme (contraste 5,6:1) |
| cream-50 | #F7F2E7 | Seções claras |
| cream-200 | #E8DEC8 | Bordas em seção clara |
| ink-600 | #5A5548 | Texto secundário sobre creme |
| text | #F4F1EA | Texto sobre escuro |
| muted | #B9B5AA | Texto secundário sobre escuro (contraste 10:1) |
| wa-500 | #25D366 | Exclusivo do botão de WhatsApp |
| wa-ink | #052E16 | Texto do botão de WhatsApp |

Regras: verde só no WhatsApp (na primeira dobra: o botão do hero e o botão flutuante; o botão do cabeçalho é dourado). Dourado nunca como texto de corpo sobre creme. Texto sobre dourado é sempre ink-950.

## 2. Tipografia (Google Fonts)
- Títulos: **Sora** (600, 700, 800). Geométrica e arredondada como a palavra "tigress" do logo.
- Corpo: **Inter** (400, 500, 600, 700).

| Nível | Desktop | Mobile | Peso | Entrelinha | Espaçamento |
|---|---|---|---|---|---|
| H1 | 68 px | 38 px | 800 | 1,05 | -0,02em |
| H2 | 44 px | 28 px | 700 | 1,15 | -0,015em |
| H3 | 30 px | 23 px | 700 | 1,3 | 0 |
| Corpo | 17 px | 16 px | 400 | 1,7 | 0 |
| Etiqueta | 12 px | 12 px | 700 | 1,2 | 0,12em, maiúsculas |

Uma única cor de destaque por dobra (dourado).

## 3. Componentes
- **Botão WhatsApp:** fundo #25D366, texto e ícone #052E16, altura 56 px, cantos 12 px. Hover: sobe 2 px. Foco: contorno dourado de 3 px (preto sobre fundo creme).
- **Botão dourado:** fundo #F2B705, texto #08080A, mesmo formato. Usado no botão do cabeçalho (que abre o WhatsApp) e em ações de apoio, para manter no máximo dois verdes por dobra.
- **Botão contorno:** transparente, borda branca 28%, texto claro.
- **Campos (select):** fundo ink-800, borda ink-700, 52 px de altura, foco com borda dourada; erro com borda #FF6B4A.
- **Cards:** fundo ink-800, borda 1px branca 12%, cantos 20 px, hover com borda dourada.
- **Abas:** pílulas de 48 px de altura, ativa em dourado.

## 4. Estética
- Cantos: 6 / 12 / 20 px, e círculo completo em ícones.
- Sombras: só brilho dourado suave (0 0 40px rgba(242,183,5,.25)) em destaques; sem sombra preta pesada.
- Espaçamento (escala de 8): 8, 16, 24, 32, 48, 80 px. Seções com 96 px no desktop e 60 px no mobile.
- Detalhes: linhas de circuito e pulso de energia em SVG, raio como marcador.
- Movimento sutil (entrada ao rolar, pulso no hero); tudo desligado com prefers-reduced-motion.

## 5. Conversão para o WhatsApp
- CTA no topo, hero, serviços, como funciona, sinais de alerta, montador de mensagem, atendimento e final, mais o botão flutuante.
- O montador de mensagem tira o "não sei o que escrever" e leva a conversa pronta.
- Prova social real (5,0 e 46 avaliações) colada no primeiro CTA.
- Verde aparece só nos botões de WhatsApp (CTA de cada seção e o botão flutuante); o resto da página é preto e dourado.

## Tokens prontos (CSS)
```css
:root{
  --ink-950:#08080A; --ink-900:#101014; --ink-800:#18181E; --ink-700:#24242C;
  --gold-300:#FFD966; --gold-400:#FFC933; --gold-500:#F2B705; --gold-600:#C79200; --gold-700:#7A5A00;
  --cream-50:#F7F2E7; --cream-200:#E8DEC8; --ink-600:#5A5548;
  --text:#F4F1EA; --muted:#B9B5AA; --line:rgba(255,255,255,.12);
  --wa-500:#25D366; --wa-ink:#052E16; --alert:#FF6B4A;
  --font-display:'Sora',system-ui,sans-serif; --font-body:'Inter',system-ui,sans-serif;
  --r-sm:6px; --r-md:12px; --r-lg:20px; --r-full:999px;
  --glow:0 0 40px rgba(242,183,5,.25);
}
```
