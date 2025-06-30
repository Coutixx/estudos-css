# Guia Completo de CSS para Desenvolvedor

> Versão profissional e aplicada — do básico ao avançado

# Propriedades CSS Essenciais e Explicações

---

## Texto

- `color`: Define a cor do texto.  
  Ex: `color: #333;`

- `font-family`: Define a fonte do texto.  
  Ex: `font-family: Arial, sans-serif;`

- `font-size`: Define o tamanho da fonte.  
  Ex: `font-size: 16px;`

- `font-weight`: Define a espessura da fonte (normal, bold, números).  
  Ex: `font-weight: 700;`

- `text-align`: Alinha o texto (left, center, right, justify).  
  Ex: `text-align: center;`

- `text-transform`: Transforma o texto (uppercase, lowercase, capitalize).  
  Ex: `text-transform: uppercase;`

- `line-height`: Espaçamento entre linhas.  
  Ex: `line-height: 1.5;`

- `letter-spacing`: Espaçamento entre letras.  
  Ex: `letter-spacing: 2px;`

---

## Espaçamento

- `margin`: Espaço externo ao elemento.  
  Ex: `margin: 10px;`

- `padding`: Espaço interno do elemento.  
  Ex: `padding: 10px;`

---

## Tamanho e Layout

- `width`: Largura do elemento.  
  Ex: `width: 100px;`

- `height`: Altura do elemento.  
  Ex: `height: 50px;`

- `max-width`: Largura máxima permitida.  
  Ex: `max-width: 500px;`

- `min-height`: Altura mínima permitida.  
  Ex: `min-height: 100px;`

- `display`: Define o tipo de exibição.  
  Ex: `display: block;`, `display: inline;`, `display: flex;`, `display: grid;`

- `position`: Define o posicionamento.  
  Ex: `position: static;`, `position: relative;`, `position: absolute;`, `position: fixed;`, `position: sticky;`

- `top`, `bottom`, `left`, `right`: Define a posição do elemento (quando `position` não for static).  
  Ex: `top: 10px;`

- `z-index`: Ordem de sobreposição de elementos.  
  Ex: `z-index: 100;`

---

## Estilo Visual

- `border`: Borda do elemento.  
  Ex: `border: 1px solid #000;`

- `border-radius`: Arredonda os cantos.  
  Ex: `border-radius: 8px;`

- `box-shadow`: Sombra do elemento.  
  Ex: `box-shadow: 0 0 10px rgba(0,0,0,0.3);`

- `background-color`: Cor de fundo.  
  Ex: `background-color: #fff;`

- `background-image`: Imagem de fundo.  
  Ex: `background-image: url('imagem.jpg');`

- `background-size`: Tamanho da imagem de fundo.  
  Ex: `background-size: cover;`

---

## Flexbox

- `display: flex;` — ativa o Flexbox.
- `flex-direction: row | column;` — define a direção dos itens.
- `justify-content: center | space-between | space-around;` — alinha itens horizontalmente.
- `align-items: center | stretch;` — alinha itens verticalmente.
- `gap: 10px;` — espaçamento entre itens.

---

## Grid Layout

- `display: grid;` — ativa o Grid Layout.
- `grid-template-columns: repeat(3, 1fr);` — define colunas iguais.
- `grid-gap: 10px;` — espaço entre linhas e colunas.

---

## Responsividade

- Media Queries:

````css
@media (max-width: 768px) {
  /* regras para telas menores */
}


---

## 🔢 Índice

- [1. Conceito](#1-conceito)
- [2. Formas de uso](#2-formas-de-uso)
- [3. Sintaxe](#3-sintaxe)
- [4. Seletores](#4-seletores)
- [5. Unidades](#5-unidades)
- [6. Propriedades comuns](#6-propriedades-comuns)
- [7. Box Model](#7-box-model)
- [8. Flexbox](#8-flexbox)
- [9. Grid Layout](#9-grid-layout)
- [10. Responsividade](#10-responsividade)
- [11. Variáveis CSS](#11-variáveis-css)
- [12. Animações e transições](#12-animações-e-transições)
- [13. Boas práticas](#13-boas-práticas)
- [14. Reset/Normalize](#14-resetnormalize)
- [15. Exemplo base](#15-exemplo-base)
- [16. Paleta Graphite Blue](#16-paleta-graphite-blue)
- [17. Extras](#17-extras)

---

## 1. Conceito

CSS (Cascading Style Sheets) é a linguagem de estilo usada para controlar visualmente o HTML: layout, cor, espaçamento, animação e responsividade.

## 2. Formas de uso (sempre usar CSS externo)

```html
<link rel="stylesheet" href="css/style.css" />
````

## 3. Sintaxe

```css
seletor {
  propriedade: valor;
}
```

## 4. Seletores

```css
p {
}
.titulo {
}
#menu {
}
nav ul {
}
section > h2 {
}
* a:hover {
}
```

## 5. Unidades

- **Absolutas:** px, cm, in
- **Relativas:** em, rem, %, vw, vh

## 6. Propriedades comuns

### Texto

- color, font-family, font-size, font-weight
- text-align, text-transform, line-height

### Espaçamento

- margin (externo)
- padding (interno)

### Layout e Tamanho

- width, height, max-width, min-height
- display: block | inline | flex | grid
- position: static | relative | absolute | fixed | sticky
- top, bottom, left, right, z-index

### Estilo visual

- border, border-radius, box-shadow
- background-color, background-image, background-size

## 7. Box Model

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

- Todo elemento tem: content > padding > border > margin

## 8. Flexbox

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
}
```

## 9. Grid Layout

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}
```

## 10. Responsividade

```css
@media (max-width: 768px) {
  body {
    font-size: 14px;
  }
}
```

- Usa-se media queries com vw, vh, %
- Ajustar layout, esconder elementos, mudar direção de flex/grid

## 11. Variáveis CSS

```css
:root {
  --cor-primaria: #007bff;
}

.btn {
  background-color: var(--cor-primaria);
}
```

## 12. Animações e transições

```css
.btn {
  transition: all 0.3s ease-in-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
```

## 13. Boas práticas

- CSS externo
- Classe com nomes semânticos e em kebab-case: `.user-card`
- Evitar `!important`
- Comentar blocos grandes
- Separar layout (flex/grid) de estilo (cor/tipo)

## 14. Reset/Normalize

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

## 15. Exemplo base

```css
body {
  font-family: "Arial", sans-serif;
  color: #e0e0e0;
  background-color: #121212;
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: inherit;
}

.btn {
  background: #3b82f6;
  color: white;
  padding: 10px 20px;
  border-radius: 8px;
  transition: background 0.3s;
}

.btn:hover {
  background: #2563eb;
}
```

## 16. Paleta Graphite Blue

```css
:root {
  --bg-main: #121212;
  --bg-card: #1e1e2f;
  --border-soft: #2a2a3c;
  --text-main: #e0e0e0;
  --text-secondary: #a0a0b0;
  --btn-primary: #3b82f6;
  --btn-hover: #2563eb;
  --neutral-icon: #606078;
}
```

## 17. Extras

- Sass/SCSS (variáveis, mixins, nesting)
- BEM (block-element-modifier)
- CSS Modules (em React)
- Tailwind CSS (estilização utilitária)
- Animações com `transform`, `scale`, `translate`, `opacity`
