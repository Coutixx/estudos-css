# Guia Completo de JavaScript para Desenvolvedor

## 1. Introdução
JavaScript é a linguagem de programação que dá interatividade, lógica e dinâmica ao site. Roda no navegador (client-side) e também no servidor (com Node.js).

## 2. Inclusão no HTML
```html
<script src="js/script.js"></script>
```

## 3. Sintaxe básica

### Declaração de variáveis
```js
let nome = "Chef";
const idade = 16;
var antigo = "evitar usar";
```

### Tipos de dados
- String: `"texto"`
- Number: `10`, `3.14`
- Boolean: `true`, `false`
- Array: `["HTML", "CSS", "JS"]`
- Object: `{ nome: "Chef", idade: 16 }`
- Null: `null`
- Undefined: `undefined`

### Operadores
- Aritméticos: `+`, `-`, `*`, `/`, `%`
- Comparação: `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=`
- Lógicos: `&&`, `||`, `!`

## 4. Controle de fluxo

### Condicional
```js
if (idade >= 18) {
  console.log("Maior de idade");
} else {
  console.log("Menor de idade");
}
```

### Switch
```js
switch (dia) {
  case "segunda": console.log("Início da semana"); break;
  default: console.log("Outro dia");
}
```

### Loop
```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}

while (condicao) {
  // executa enquanto verdadeiro
}
```

## 5. Funções
```js
function saudacao(nome) {
  return `Olá, ${nome}!`;
}

const somar = (a, b) => a + b;
```

## 6. Manipulação do DOM
```js
const titulo = document.querySelector("h1");
titulo.textContent = "Novo título";
titulo.style.color = "blue";
```

### Eventos
```js
botao.addEventListener("click", function () {
  alert("Clicou!");
});
```

## 7. Arrays e Objetos

### Array
```js
const lista = ["HTML", "CSS", "JS"];
lista.push("React");
console.log(lista[0]);
```

### Object
```js
const user = { nome: "Chef", idade: 16 };
console.log(user.nome);
```

## 8. Métodos úteis

### Strings
- `length`, `toUpperCase()`, `toLowerCase()`, `includes()`, `replace()`, `split()`

### Arrays
- `push()`, `pop()`, `shift()`, `unshift()`, `map()`, `filter()`, `reduce()`, `forEach()`

## 9. JSON
```js
const json = '{"nome":"Chef","idade":16}';
const obj = JSON.parse(json);
const novoJSON = JSON.stringify(obj);
```

## 10. Funções assíncronas
```js
async function pegarDados() {
  const resposta = await fetch("https://api.exemplo.com");
  const dados = await resposta.json();
  console.log(dados);
}
```

## 11. Boas práticas
- Usar `const` sempre que possível
- Evitar `var`
- Nomear funções e variáveis com clareza (camelCase)
- Comentar partes complexas
- Dividir código em funções reutilizáveis
- Validar dados e tratar erros com `try/catch`

## 12. Exemplo de interatividade
```html
<button id="btn">Clique</button>
<script>
  const btn = document.getElementById("btn");
  btn.addEventListener("click", () => {
    alert("Você clicou!");
  });
</script>
```

---

## Extras para dominar depois
- Promises e async/await avançado
- Manipulação de datas com Date
- LocalStorage e SessionStorage
- Módulos ES6 (`import`, `export`)
- Fetch API / Axios
- Frameworks: React, Vue, Angular
- Node.js (JS no backend)
- Testes automatizados (Jest)
