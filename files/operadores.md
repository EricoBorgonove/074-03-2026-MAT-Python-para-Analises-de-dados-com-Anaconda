# ⚡ Operadores em Python

Os operadores em Python são símbolos especiais que realizam operações sobre valores e variáveis. Eles podem ser classificados em diferentes categorias.

---

## 📌 Tipos de Operadores

Python possui os seguintes tipos de operadores:

1. **Aritméticos**
2. **De Atribuição**
3. **Comparação (Relacionais)**
4. **Lógicos**
5. **Bitwise (Bit a Bit)**
6. **Identidade**
7. **Pertinência (Membership)**

Cada um deles desempenha um papel específico dentro das expressões e cálculos.

---

## 🔢 1. Operadores Aritméticos

Os operadores aritméticos são usados para realizar operações matemáticas entre variáveis e valores.

| Operador | Descrição          | Exemplo (`a = 10`, `b = 3`) |
|----------|-------------------|----------------------------|
| `+`      | Adição            | `a + b` → `13`             |
| `-`      | Subtração         | `a - b` → `7`              |
| `*`      | Multiplicação     | `a * b` → `30`             |
| `/`      | Divisão           | `a / b` → `3.3333`         |
| `//`     | Divisão Inteira   | `a // b` → `3`             |
| `%`      | Módulo (Resto)    | `a % b` → `1`              |
| `**`     | Exponenciação     | `a ** b` → `1000`          |

Exemplo:
```python
a = 10
b = 3
print(a + b)  # 13
print(a ** b)  # 1000
```

---

## 🎯 2. Operadores de Atribuição

Usados para atribuir valores às variáveis.

| Operador | Exemplo  | Equivalente a |
|----------|---------|---------------|
| `=`      | `a = 5` | `a = 5`       |
| `+=`     | `a += 2` | `a = a + 2`   |
| `-=`     | `a -= 3` | `a = a - 3`   |
| `*=`     | `a *= 4` | `a = a * 4`   |
| `/=`     | `a /= 2` | `a = a / 2`   |
| `//=`    | `a //= 3` | `a = a // 3` |
| `%=`     | `a %= 2` | `a = a % 2`   |
| `**=`    | `a **= 2` | `a = a ** 2` |

Exemplo:
```python
a = 5
a += 3  # Agora a é 8
a **= 2  # Agora a é 64
```

---

## 🔍 3. Operadores de Comparação (Relacionais)

Comparam valores e retornam `True` ou `False`.

| Operador | Descrição          | Exemplo (`a = 10`, `b = 5`) |
|----------|-------------------|----------------------------|
| `==`     | Igualdade         | `a == b` → `False`        |
| `!=`     | Diferente         | `a != b` → `True`         |
| `>`      | Maior que         | `a > b` → `True`          |
| `<`      | Menor que         | `a < b` → `False`         |
| `>=`     | Maior ou igual    | `a >= b` → `True`         |
| `<=`     | Menor ou igual    | `a <= b` → `False`        |

Exemplo:
```python
a = 10
b = 5
print(a > b)  # True
print(a == b)  # False
```

---

## 🧠 4. Operadores Lógicos

Utilizados para combinar expressões booleanas.

| Operador | Descrição                           | Exemplo (`a = True`, `b = False`) |
|----------|-----------------------------------|----------------------------|
| `and`    | Retorna `True` se ambos forem `True` | `a and b` → `False`        |
| `or`     | Retorna `True` se pelo menos um for `True` | `a or b` → `True` |
| `not`    | Inverte o valor booleano         | `not a` → `False`        |

Exemplo:
```python
x = 10
y = 5
if x > 5 and y < 10:
    print("Condição satisfeita")
```

---

## 🖥 5. Operadores Bitwise (Bit a Bit)

Realizam operações diretamente nos bits dos números inteiros.

| Operador | Descrição            | Exemplo (`a = 5`, `b = 3`) |
|----------|---------------------|----------------------------|
| `&`      | AND bit a bit       | `a & b` → `1`             |
| `|`      | OR bit a bit        | `a | b` → `7`             |
| `^`      | XOR bit a bit       | `a ^ b` → `6`             |
| `~`      | NOT bit a bit       | `~a` → `-6`              |
| `<<`     | Deslocamento à esquerda | `a << 1` → `10`        |
| `>>`     | Deslocamento à direita | `a >> 1` → `2`        |

Exemplo:
```python
a = 5  # 101 em binário
b = 3  # 011 em binário
print(a & b)  # 1 (001)
```

---

## 🆔 6. Operadores de Identidade

Verificam se duas variáveis referem-se ao mesmo objeto na memória.

| Operador | Descrição        | Exemplo (`a = 10`, `b = 10`) |
|----------|----------------|----------------------------|
| `is`     | Retorna `True` se for o mesmo objeto | `a is b` → `True`  |
| `is not` | Retorna `True` se não for o mesmo objeto | `a is not b` → `False` |

---

## 🔍 7. Operadores de Pertinência (Membership)

Verificam se um valor está presente em uma sequência (listas, strings, tuplas, etc.).

| Operador | Descrição         | Exemplo (`x = [1, 2, 3]`) |
|----------|----------------|-------------------------|
| `in`     | Retorna `True` se o valor estiver na sequência | `2 in x` → `True` |
| `not in` | Retorna `True` se o valor **não** estiver na sequência | `5 not in x` → `True` |

Exemplo:
```python
frutas = ["maçã", "banana", "laranja"]
print("banana" in frutas)  # True
```

---

💡 _Dominar os operadores é essencial para escrever código eficiente e expressivo! 🚀_
