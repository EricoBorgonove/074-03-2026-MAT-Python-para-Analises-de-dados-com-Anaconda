# 🔍 Funções em Python

As funções são blocos de código reutilizáveis que ajudam a organizar e modularizar programas. Elas permitem a execução de tarefas específicas e evitam repetição de código.

---

## 📌 O que são Funções?

Uma função é um conjunto de instruções que recebe entradas, executa cálculos ou operações e retorna um resultado.

### 🎯 Benefícios do Uso de Funções:
- **Reutilização de código** → Evita repetição.
- **Modularidade** → Código mais organizado e fácil de manter.
- **Facilidade de depuração** → Testes e correções mais simples.
- **Legibilidade** → Código mais claro e compreensível.

---

## 🚀 Criando Funções em Python

### 🔹 Sintaxe Básica
```python
def nome_da_funcao(parametros):
    # Bloco de código
    return resultado
```

### 🔹 Exemplo Simples
```python
def saudacao():
    print("Olá, seja bem-vindo!")

saudacao()  # Chamada da função
```

---

## 🚀 Funções com Parâmetros

Podemos passar valores para as funções através de parâmetros.

```python
def soma(a, b):
    return a + b

resultado = soma(5, 3)
print("Resultado:", resultado)  # 8
```

Se um parâmetro tiver um valor padrão, ele se torna opcional na chamada:
```python
def cumprimentar(nome="Visitante"):
    print(f"Olá, {nome}!")

cumprimentar("Alice")  # Olá, Alice!
cumprimentar()  # Olá, Visitante!
```

---

## 🚀 Retorno de Valores (`return`)

A palavra-chave `return` permite que a função devolva um resultado para quem a chamou.

```python
def multiplicacao(x, y):
    return x * y

print(multiplicacao(4, 5))  # 20
```

Uma função pode retornar múltiplos valores usando tuplas:
```python
def operacoes(a, b):
    return a + b, a - b, a * b, a / b

soma, subtracao, multiplicacao, divisao = operacoes(10, 2)
print(soma, subtracao, multiplicacao, divisao)
```

---

## 🚀 Argumentos Variáveis (`*args` e `**kwargs`)

O Python permite funções com número variável de argumentos.

### 🔹 `*args` (Argumentos Posicionais)
Permite passar múltiplos valores sem definir um número fixo de parâmetros.

```python
def somar(*numeros):
    return sum(numeros)

print(somar(1, 2, 3, 4, 5))  # 15
```

### 🔹 `**kwargs` (Argumentos Nomeados)
Permite passar argumentos com chave-valor.

```python
def exibir_info(**dados):
    for chave, valor in dados.items():
        print(f"{chave}: {valor}")

exibir_info(nome="Carlos", idade=30, cidade="São Paulo")
```

---

## 🚀 Funções Recursivas

Uma função pode chamar a si mesma, facilitando operações como cálculo de fatorial e Fibonacci.

### 🔹 Exemplo: Cálculo do Fatorial
```python
def fatorial(n):
    if n == 0:
        return 1
    return n * fatorial(n - 1)

print(fatorial(5))  # 120
```

### 🔹 Exemplo: Fibonacci
```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(6))  # 8
```

---

## 🚀 Funções `lambda` (Funções Anônimas)

As funções `lambda` são funções curtas que podem ser escritas em uma única linha.

```python
quadrado = lambda x: x ** 2
print(quadrado(5))  # 25
```

Podemos usar `lambda` dentro de funções como `map()`, `filter()` e `sorted()`:

```python
numeros = [1, 2, 3, 4, 5]
dobro = list(map(lambda x: x * 2, numeros))
print(dobro)  # [2, 4, 6, 8, 10]
```

---

## 🎯 Exercícios

1. **Criação de Funções**
   - Crie uma função que receba dois números e retorne a soma deles.

2. **Função com Parâmetro Padrão**
   - Escreva uma função que receba um nome e exiba "Olá, [nome]!". Se nenhum nome for passado, exiba "Olá, Visitante!".

3. **Uso de `*args`**
   - Faça uma função que receba múltiplos números e retorne a soma deles.

4. **Função Recursiva**
   - Implemente uma função recursiva para calcular o fatorial de um número.

5. **Uso de `lambda`**
   - Crie uma função lambda que receba um número e retorne seu triplo.

---

💡 _Dominar funções é essencial para escrever código eficiente e modular! 🚀_