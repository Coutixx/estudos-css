# Guia Completo da Linguagem C

## 1. Estrutura básica de um programa em C
```c
#include <stdio.h>

int main() {
    // código aqui
    return 0;
}
```

- `#include <stdio.h>`: importa funções de entrada/saída
- `int main()`: função principal obrigatória
- `return 0;`: indica que o programa terminou com sucesso

## 2. Tipos de dados
- `int`: números inteiros (4 bytes)
- `float`: números decimais com precisão simples (4 bytes)
- `double`: decimais com precisão dupla (8 bytes)
- `char`: caractere (1 byte)
- `void`: ausência de tipo (funções sem retorno)

## 3. Variáveis e constantes
```c
int idade = 16;
float peso = 60.5;
const float PI = 3.14;
```

## 4. Operadores
- Aritméticos: `+`, `-`, `*`, `/`, `%`
- Relacionais: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Lógicos: `&&`, `||`, `!`
- Atribuição: `=`, `+=`, `-=`, `*=`, `/=`, `%=`

## 5. Entrada e saída
```c
// entrada
scanf("%d", &idade);

// saída
printf("Idade: %d\n", idade);
```

### Especificadores de formato:
- `%d`: int
- `%f`: float
- `%lf`: double
- `%c`: char
- `%s`: string

## 6. Estruturas de controle

### Condicional
```c
if (idade >= 18) {
    printf("Maior de idade");
} else {
    printf("Menor de idade");
}
```

### Switch
```c
switch (opcao) {
    case 1: printf("Opção 1"); break;
    default: printf("Outra");
}
```

### Laços
```c
for (int i = 0; i < 10; i++) {
    printf("%d ", i);
}

while (condicao) {
    // código
}

do {
    // código
} while (condicao);
```

## 7. Funções
```c
int soma(int a, int b) {
    return a + b;
}
```

## 8. Vetores e strings

### Vetores
```c
int numeros[5] = {1, 2, 3, 4, 5};
```

### Strings
```c
char nome[20];
scanf("%s", nome);
printf("Olá, %s", nome);
```

## 9. Ponteiros
```c
int x = 10;
int *ptr = &x;

printf("%d", *ptr); // acessa valor de x
```

## 10. Estruturas
```c
struct Pessoa {
    char nome[50];
    int idade;
};

struct Pessoa p1 = {"Henrique", 16};
```

## 11. Arquivos
```c
FILE *arq = fopen("dados.txt", "r");

if (arq != NULL) {
    // leitura ou escrita
    fclose(arq);
}
```

## 12. Boas práticas
- Sempre inicialize variáveis
- Use nomes claros e em inglês
- Comente partes importantes
- Evite funções muito longas
- Separe lógica em funções pequenas
- Nunca esqueça de liberar memória se usar `malloc`

## 13. Compilação
Para compilar no terminal:
```bash
gcc programa.c -o programa
./programa
```

---

## Extras para dominar depois
- Alocação dinâmica: `malloc`, `calloc`, `free`
- Recursão
- Estruturas de dados: listas, pilhas, filas
- Manipulação avançada de strings
- Modularização com múltiplos arquivos
- Criação de bibliotecas
