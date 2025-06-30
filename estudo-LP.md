# Guia Completo de Lógica de Programação

1. O que é lógica de programação

É a capacidade de pensar em soluções passo a passo para resolver um problema, estruturando instruções de forma lógica e eficiente.

2. Elementos fundamentais

# Variáveis

Armazenam valores que podem mudar.

```c
int idade = 16;
Constantes
Valores fixos que não mudam.
```

```c
Copiar
Editar
const float PI = 3.14;
Tipos de dados
Inteiros: 1, 100, -5

Reais: 3.14, -0.99

Caractere: 'A', 'z'

Lógico/Booleano: verdadeiro/falso

Operadores
Aritméticos: +, -, *, /, %

Relacionais: ==, !=, >, <, >=, <=

Lógicos: && (e), || (ou), ! (negação)
```

3. Estruturas de controle

# Condicional

```c
Copiar
Editar
if (nota >= 7) {
// aprovado
} else {
// reprovado
}
Switch
```

```c
Copiar
Editar
switch (opcao) {
case 1:
// ação
break;
default:
// outra ação
}
```

4. Repetição (laços)

# For

```c
Copiar
Editar
for (int i = 0; i < 5; i++) {
// repete 5 vezes
}
While
```

```c
Copiar
Editar
while (condicao) {
// repete enquanto condição for verdadeira
}
Do While
```

```c
Copiar
Editar
do {
// executa pelo menos uma vez
} while (condicao);
```

5. Estrutura Sequencial

# Executa instruções em sequência:

```c
Copiar
Editar
int a = 5;
int b = 10;
int soma = a + b; 6. Estrutura Condicional
Executa apenas se uma condição for verdadeira.
```

7. Estrutura de Repetição

# Usada para repetir ações com base em condições.

8. Vetores e Matrizes

# Vetores (arrays)

```c
Copiar
Editar
int notas[5] = {7, 8, 5, 10, 6};
Matrizes (arrays 2D)
```

```c
Copiar
Editar
int tabela[2][3] = {{1, 2, 3}, {4, 5, 6}};
```

9. Funções

# Permitem dividir o código em blocos reutilizáveis.

```c
Copiar
Editar
int soma(int a, int b) {
return a + b;
} 10.
```

Algoritmos clássicos para treinar
Trocar valores de duas variáveis

Verificar se número é par ou ímpar

Calcular fatorial

Verificar se número é primo

Calcular média de alunos

Buscar o maior/menor valor em vetor

Contar elementos positivos/negativos

Ordenar vetores (ex: bubble sort)

11. Pseudocódigo

# Forma intermediária de escrever algoritmos (tipo português estruturado):

pseudo
Copiar
Editar
INÍCIO
LEIA A, B
SOMA ← A + B
ESCREVA SOMA
FIM 12. Fluxogramas
Diagramas visuais que mostram o fluxo de um algoritmo (usado no planejamento com símbolos).

Extras pra dominar depois
Recursão

Estruturas de dados (listas, filas, pilhas)

Análise de algoritmos (complexidade)

Modularização e boas práticas

Refatoração de lógica
