# 🔄 Estruturas de Repetição em Python

As estruturas de repetição permitem que um bloco de código seja executado várias vezes enquanto uma condição for verdadeira. Em Python, existem dois principais tipos de laços de repetição: `for` e `while`.

---

## 📌 Tipos de Estruturas de Repetição

1. **`for`** - Utilizado quando sabemos o número de repetições ou queremos iterar sobre elementos de uma sequência (listas, tuplas, strings, etc.).
2. **`while`** - Utilizado quando não sabemos o número exato de repetições e a execução depende de uma condição booleana.

---

## 🚀 Laço `for`

O `for` é ideal para iterar sobre elementos de uma sequência.

### 🔹 Sintaxe Básica
```python
for variavel in sequencia:
    # Bloco de código a ser repetido
```

### 🔹 Exemplo com Listas
```python
numeros = [1, 2, 3, 4, 5]
for numero in numeros:
    print(numero)
```

### 🔹 Iterando sobre Strings
```python
palavra = "Python"
for letra in palavra:
    print(letra)
```

### 🔹 Usando `range()`
A função `range()` gera uma sequência de números.
```python
for i in range(5):  # Gera valores de 0 a 4
    print(i)
```

Podemos especificar um intervalo e um passo:
```python
for i in range(1, 10, 2):  # Inicia em 1, vai até 9, incrementando de 2 em 2
    print(i)
```

---

## 🚀 Laço `while`

O `while` executa um bloco de código enquanto uma condição for verdadeira.

### 🔹 Sintaxe Básica
```python
while condicao:
    # Bloco de código a ser repetido
```

### 🔹 Exemplo Simples
```python
contador = 0
while contador < 5:
    print(contador)
    contador += 1  # Incremento necessário para evitar loop infinito
```

---

## 🚀 Controle de Fluxo em Laços

Python permite modificar o comportamento dos loops com as palavras-chave `break`, `continue` e `else`.

### 🔹 `break`
Interrompe a execução do laço antes que a condição seja falsa.
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### 🔹 `continue`
Pula a iteração atual e segue para a próxima.
```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

### 🔹 `else` em Loops
O bloco `else` em loops é executado **após o término normal do loop**, ou seja, se ele não for interrompido por um `break`.
```python
for i in range(3):
    print(i)
else:
    print("Loop concluído com sucesso!")
```

---

## 🎯 Exercícios

1. **Imprimir Números de 1 a 10**
   - Use `for` e `while` para imprimir os números de 1 a 10.

2. **Tabuada de um Número**
   - Solicite um número ao usuário e imprima sua tabuada até o 10.

3. **Soma dos Números de 1 a N**
   - Peça um número `n` e calcule a soma de `1` até `n`.

4. **Adivinhe o Número**
   - Gere um número aleatório entre `1 e 100` e peça para o usuário adivinhar até acertar.

5. **Fatorial de um Número**
   - Peça um número e calcule seu fatorial usando `while` e `for`.

6. **Contagem Regressiva**
   - Solicite um número e faça uma contagem regressiva até 0.

7. **Números Primos**
   - Peça um número ao usuário e verifique se ele é primo.

---

💡 _Com essas estruturas, você pode automatizar tarefas e criar programas mais dinâmicos! 🚀_
