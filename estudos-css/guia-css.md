# Guia Completo de CSS para Desenvolvedor

> Versão profissional e aplicada — do básico ao avançado

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
```

## 3. Sintaxe

```css
seletor {
  propriedade: valor;
}
```

## 4. Seletores

```css
p {}
.titulo {}
#menu {}
nav ul {}
section > h2 {}
*
a:hover {}
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
  from { opacity: 0; }
  to { opacity: 1; }
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
  background: #3B82F6;
  color: white;
  padding: 10px 20px;
  border-radius: 8px;
  transition: background 0.3s;
}

.btn:hover {
  background: #2563EB;
}
```

## 16. Paleta Graphite Blue

```css
:root {
  --bg-main: #121212;
  --bg-card: #1E1E2F;
  --border-soft: #2A2A3C;
  --text-main: #E0E0E0;
  --text-secondary: #A0A0B0;
  --btn-primary: #3B82F6;
  --btn-hover: #2563EB;
  --neutral-icon: #606078;
}
```

## 17. Extras

- Sass/SCSS (variáveis, mixins, nesting)
- BEM (block-element-modifier)
- CSS Modules (em React)
- Tailwind CSS (estilização utilitária)
- Animações com `transform`, `scale`, `translate`, `opacity`
