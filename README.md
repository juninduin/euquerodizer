# Eu Quero Dizer

Prancha de comunicação digital (CAA) para crianças — projeto de feira de ciências
sobre **acessibilidade intelectual**: a criança toca numa imagem e o aparelho fala
a frase, ajudando a mostrar o que precisa e como está se sentindo.

## Como usar

Abra o arquivo **`index.html`** em qualquer navegador (celular ou computador).
Não precisa instalar nada.

1. Tela inicial → botão **INICIAR** (também libera o som e a voz).
2. Escolha uma aba: **Básico · Preciso · Sinto · Ajuda · Rotina**.
3. Toque numa figura → o app fala a frase e guarda no histórico do dia.
4. Ícones de cima: sobre o projeto, histórico da semana, ouvir a tela,
   e acessibilidade (alto contraste, texto maior, menos animação).

O histórico de sentimentos fica salvo **só no próprio aparelho** (localStorage).

## Imagens dos botões

Cada botão tenta carregar uma ilustração em `imagens/<código>.png`
(também aceita `.webp .jpg .jpeg .svg`). Se não houver arquivo, o botão usa
um desenho de reserva feito em código (SVG), então o app funciona mesmo sem
nenhuma imagem.

- `imagens/LEIA-ME.txt` — lista dos 40 códigos, rótulos e frases.
- `imagens/PROMPTS.txt` — sugestões de prompt para gerar as ilustrações
  (uma criança fazendo cada ação, estilo material didático).
- `imagens/_originais/` — backup das primeiras imagens.

## Tecnologia

Um único arquivo `index.html` (HTML + CSS + JavaScript puro).
Voz pela `SpeechSynthesis` do navegador, em português.
