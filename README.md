Tela de Login do Telegram Web
Contrução de pagina web com html e css

Nome: Marco Antonio Pasinato
Matrícula: 1139597
Site de referência: https://web.telegram.org/
Disciplina: Front-End
Professor: Matheus Henrique Barquette
---
Sobre o projeto

Fiz uma cópia da tela de login do Telegram Web (a versão de computador),
usando o login por número de telefone. Fiz isso só olhando como o site
original fica na tela, sem copiar o código dele.

Como abrir

É só abrir o arquivo `index.html` no navegador (Chrome, Edge, etc).

---

Checklist da Parte 1

 1.1 HTML organizado e acessível
-  Usei as tags certas: `main`, `section`, `nav` e `footer`, do jeito que a página original é organizada
-  O formulário de login tem um `label` (rótulo) em cada campo: país, telefone e "manter conectado"

*Explicação:* o `main` guarda a tela de login (`section`); o `nav` é o
seletor de idioma que fica embaixo, igual no site original; o `footer` tem o
texto que eu adicionei com meu nome.

*Observação:* não usei imagem (foto) no projeto, porque o site original
também não usa imagem na tela de telefone, só ícones. O ícone do Telegram é
decorativo, então botei `aria-hidden="true"` nele (isso avisa o leitor de
tela que aquele ícone não precisa ser lido).

#1.2 Parecido visualmente com o site original
-  Fundo branco, ícone redondo do Telegram no meio, campos com linha embaixo (sem caixinha), do mesmo jeito que o site de verdade
-  Botão "PRÓXIMO" arredondado, na cor azul do Telegram
-  Mesma organização: logo em cima, formulário no meio, idiomas embaixo
-  O que ficou diferente: o ícone do Telegram é um desenho simples em SVG (não é a logo oficial); o formulário não manda SMS de verdade, porque não tem um servidor por trás

1.3 CSS: seletores, box model e variáveis
- Seletor de classe (`.btn-next`)
- Seletor descendente (`.field select`, `.field__phone-group input`)
- Pseudo-classe (`:hover`, `:focus`, `:focus-within`)
-  Variáveis CSS (`:root { --color-primary... }`)

1.4 Responsivo: Flexbox, Grid e mobile first
-  CSS escrito primeiro pensando no celular (mobile first), funciona sem media query
-  Usei Flexbox para organizar os elementos da página
-  Tem uma media query com `min-width` que ajusta o layout pra telas maiores
-  Testei em tela de celular e de computador

 1.5 Toque pessoal
-  Coloquei um rodapé com meu nome dizendo que é um projeto de estudo — isso não existe no site original

---

Prints comparando com o original

| Site original | 
![alt text](image.png)

| Meu projeto |
![alt text](image-1.png)
---

Validei o HTML em https://validator.w3.org antes de entregar.