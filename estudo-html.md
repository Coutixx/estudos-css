# Guia Completo de HTML para Desenvolvedor

## 1. Estrutura básica do HTML

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Título da Página</title>
  </head>
  <body>
    <!-- Conteúdo aqui -->
  </body>
</html>
```

- `<!DOCTYPE html>`: define HTML5, padrão atual obrigatório
- `<html lang="pt-BR">`: idioma da página para acessibilidade e SEO
- `<head>`: metadados, título, links, scripts
- `<meta charset="UTF-8" />`: codificação de caracteres (acentos etc)
- `<meta name="viewport">`: responsividade para dispositivos móveis
- `<title>`: título que aparece na aba do navegador
- `<body>`: conteúdo visível da página

## 2. Tags mais usadas e suas funções

### Semânticas:

- `<header>`: topo da página ou seção
- `<nav>`: menu de navegação
- `<main>`: conteúdo principal (só um por página)
- `<section>`: seção genérica, agrupamento de conteúdo
- `<article>`: conteúdo independente (ex: post, notícia)
- `<aside>`: conteúdo complementar (ex: barra lateral)
- `<footer>`: rodapé da página ou seção

### Texto:

- `<h1>` a `<h6>`: títulos, h1 o mais importante
- `<p>`: parágrafo
- `<strong>`: texto importante (negrito semântica)
- `<em>`: texto enfatizado (itálico semântica)
- `<br>`: quebra de linha
- `<hr>`: linha horizontal para separação

### Links e mídias:

- `<a href="url">`: link
- `<img src="url" alt="descrição">`: imagem, alt obrigatório
- `<video>`, `<audio>`: mídia embutida

### Listas:

- `<ul>`: lista não ordenada (bolinhas)
- `<ol>`: lista ordenada (números)
- `<li>`: item de lista (sempre dentro de ul ou ol)

### Formulários:

- `<form>`: formulário
- `<input>`: campo de entrada
- `<label>`: rótulo para inputs
- `<textarea>`: área de texto
- `<button>`: botão
- `<select>`, `<option>`: lista suspensa
- `type` no input: text, password, email, number, submit, etc.

## 3. Atributos importantes

- `id`: identificador único no documento
- `class`: identifica grupos para estilo/JS
- `href`: endereço do link (âncora)
- `src`: fonte da imagem ou mídia
- `alt`: texto alternativo da imagem (acessibilidade)
- `name`: nome do campo em formulário (para backend)
- `placeholder`: texto guia em input
- `required`: campo obrigatório
- `disabled`: desabilita o campo
- `maxlength`, `minlength`: limites de tamanho
- `pattern`: regex para validar entrada

## 4. Boas práticas

- Sempre usar `alt` nas imagens
- Usar tags semânticas para SEO e acessibilidade
- Validar formulários no front e backend
- Usar `label` associado a cada `input` com `for="id-do-input"`
- Manter indentação e organização do código
- Evitar uso de inline styles ou javascript no HTML
- Usar nomes de classes em inglês, sem acento, kebab-case
- Evitar `id` repetidos no documento
- Sempre fechar tags que não são void (exceto tags como `<br>`, `<img>`, etc)

## 5. SEO e acessibilidade

- Usar `lang` correto na tag `<html>`
- Textos alternativos descritivos nas imagens
- Usar `<nav>` para menus
- Estruturar conteúdo com títulos hierárquicos (`<h1>` a `<h6>`)
- Usar atributos ARIA quando necessário (ex: `aria-label`)
- Evitar elementos que atrapalhem a navegação por teclado

## 6. Comentários

- Sintaxe: `<!-- Comentário aqui -->`
- Usar para documentar seções complexas
- Não deixa código comentado em produção

## 7. Exemplos comuns

### Link externo com target para abrir em nova aba

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer"
  >Link externo</a
>
```

### Formulário simples

```html
<form action="/submit" method="POST">
  <label for="email">Email:</label>
  <input
    type="email"
    id="email"
    name="email"
    required
    placeholder="seu@email.com"
  />
  <button type="submit">Enviar</button>
</form>
```

---

# Extras que você deve dominar depois

- HTML5 APIs (Storage, Canvas, Geolocation)
- Microdata e Schema para SEO avançado
- Técnicas de otimização e performance
- Entender o DOM e manipulação via JS
