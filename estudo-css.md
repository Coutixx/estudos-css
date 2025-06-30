# Guia Completo de CSS para Desenvolvedor

# Paleta “Graphite Blue”

- `Fundo principal (body): #121212 (preto carvão)`

- `Card/Formulário: #1E1E2F (grafite azulado)`

- `Bordas e sombras suaves: #2A2A3C`

- `Texto principal: #E0E0E0 (cinza claro quase branco)`

- `Texto secundário/placeholder: #A0A0B0`

- `Botão primário: #3B82F6 (azul profissional)`

- `Botão hover: #2563EB`

- `Detalhes/ícones neutros: #606078`

## 1. Conceito

CSS (Cascading Style Sheets) é usado para estilizar elementos HTML. Controla layout, cores, tamanhos, posicionamento, responsividade e animações.

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

- `elemento` → `p`, `h1`, `footer`
- `.classe` → `.btn-primary`
- `#id` → `#menu-lateral`
- `elemento elemento` → `nav ul`
- `elemento > filho` → `section > h2`
- `*` → `todos os elementos`

- `elemento:hover` → estado ao passar o mouse

## 5. Tipos de unidades

- Absolutas: `px`, `cm`, `in`
- Relativas: `em`, `rem`, `%`, `vw`, `vh`

## 6. Propriedades mais usadas

### Texto

- `color`
- `font-family`
- `font-size`
- `font-weight`
- `text-align`
- `text-transform`
- `line-height`
- `letter-spacing`

### Espaçamento

- `margin`: espaço externo
- `padding`: espaço interno

### Tamanho e layout

- `width`, `height`
- `max-width`, `min-height`
- `display`: `block`, `inline`, `inline-block`, `flex`, `grid`, `none`
- `position`: `static`, `relative`, `absolute`, `fixed`, `sticky`
- `top`, `bottom`, `left`, `right`
- `z-index`

### Borda e fundo

- `border`: `1px solid #000`
- `border-radius`
- `background-color`
- `background-image`
- `background-size`: `cover`, `contain`
- `box-shadow`

### Flexbox

```css
display: flex;
flex-direction: row | column;
justify-content: center | space-between | space-around;
align-items: center | stretch;
gap: 10px;
```

### Grid (CSS Grid Layout)

```css
display: grid;
grid-template-columns: repeat(3, 1fr);
grid-gap: 10px;
```

## 7. Responsividade

### Media Queries

```css
@media (max-width: 768px) {
  body {
    font-size: 14px;
  }
}
```

## 8. Variáveis CSS

```css
:root {
  --cor-primaria: #007bff;
}

.btn {
  background-color: var(--cor-primaria);
}
```

## 9. Animações e transições

```css
transition: all 0.3s ease-in-out;
animation: fadeIn 1s ease;

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
```

## 10. Boas práticas

- Nomear classes em inglês, kebab-case: `.product-card`
- Usar CSS externo sempre
- Evitar !important (último recurso)
- Separar layout (grid/flex) de estilo (cores/tipografia)
- Organizar o CSS por seções
- Comentar blocos quando necessário

## 11. Reset ou Normalize

Use reset para remover estilos padrão dos navegadores:

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

## 12. Exemplo base de CSS

```css
body {
  font-family: "Arial", sans-serif;
  color: #333;
  background-color: #f9f9f9;
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: inherit;
}

.btn-primary {
  background: #007bff;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
}
```

---

## Extras pra estudar depois

- Sass/SCSS (pré-processadores)
- BEM (metodologia de nomeação de classe)
- CSS Modules (em React)
- Tailwind CSS (utilitário moderno)
- Animações complexas e transformações
