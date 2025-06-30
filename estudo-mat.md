# Criando um arquivo Markdown com as fórmulas dos tópicos solicitados

formulas_md = """

# 📚 Fórmulas de Matemática – Chef

## 🔺 Trigonometria

### Lei dos Senos

\\[
\\frac{a}{\\sen A} = \\frac{b}{\\sen B} = \\frac{c}{\\sen C}
\\]

### Lei dos Cossenos

\\[
a^2 = b^2 + c^2 - 2bc \\cdot \\cos A
\\]
\\[
b^2 = a^2 + c^2 - 2ac \\cdot \\cos B
\\]
\\[
c^2 = a^2 + b^2 - 2ab \\cdot \\cos C
\\]

---

## 🧮 Conjuntos

- União: \\( A \\cup B \\)
- Interseção: \\( A \\cap B \\)
- Diferença: \\( A - B \\)
- Complementar: \\( A^c \\)
- Pertence: \\( x \\in A \\)
- Não pertence: \\( x \\notin A \\)

Conjuntos usuais:

- \\( \\mathbb{N} \\): naturais
- \\( \\mathbb{Z} \\): inteiros
- \\( \\mathbb{Q} \\): racionais
- \\( \\mathbb{R} \\): reais
- \\( \\mathbb{I} \\): irracionais

---

## ➗ Fração Geratriz

### Decimal exato

\\[
0{,}ab = \\frac{ab}{10^n}
\\]

### Periódico simples (ex: 0{,}777...)

\\[
x = 0{,}\\overline{a} \\\\
10x = a{,}\\overline{a} \\\\
10x - x = 9x = a \\\\
x = \\frac{a}{9}
\\]

### Periódico composto (ex: 0{,}58383...)

\\[
x = 0{,}n\\overline{p} \\\\
Multiplica por potências de 10 para eliminar as casas decimais e resolver: \\\\
10^k x - 10^m x = número \\\\
x = \\frac{número}{10^k - 10^m}
\\]

---

## 📈 Função

Função geral:
\\[
f(x) = \\text{expressão algébrica}
\\]

Domínio: todos os valores de \\( x \\) que não anulam denominadores nem causam raiz par de número negativo.

---

## 📉 Função Afim

Forma geral:
\\[
f(x) = ax + b
\\]

- Raiz: \\( f(x) = 0 \\Rightarrow x = -\\frac{b}{a} \\)
- Interseção com y: \\( f(0) = b \\)
- Coeficiente angular (a): indica a inclinação da reta
  """

# Salvando no arquivo .md

file_path = "/mnt/data/formulas_chef.md"
with open(file_path, "w") as f:
f.write(formulas_md)

file_path
