# 🔀 Estruturas Condicionais em Python

As estruturas condicionais são fundamentais para a lógica de um programa, permitindo a tomada de decisões com base em condições.

---

## 📌 O que são Estruturas Condicionais?

As estruturas condicionais permitem que um programa execute diferentes blocos de código dependendo do resultado de uma expressão lógica.

Em Python, utilizamos os comandos `if`, `elif` e `else` para definir condições.

---

## 🚀 Sintaxe Básica do `if` e `else`

```python
idade = int(input("Digite sua idade: "))

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

- Se a condição dentro do `if` for verdadeira, o bloco de código será executado.
- Caso contrário, o bloco do `else` será executado.

---

## 🚀 Usando `elif` para Múltiplas Condições

O `elif` (abreviação de "else if") permite testar múltiplas condições sequencialmente.

```python
nota = float(input("Digite sua nota: "))

if nota >= 9:
    print("Ótimo desempenho! Nota A.")
elif nota >= 7:
    print("Bom desempenho! Nota B.")
elif nota >= 5:
    print("Regular! Nota C.")
else:
    print("Reprovado! Nota D.")
```

### 🛠 Regras:
1. O `if` sempre é testado primeiro.
2. O `elif` é testado caso a condição do `if` seja falsa.
3. O `else` é executado apenas se todas as condições anteriores forem falsas.

---

## 🚀 Expressões Lógicas e Operadores Comparativos

Python permite o uso de operadores para comparar valores dentro das condições.

| Operador  | Significado  | Exemplo (`a = 10`, `b = 5`) |
|-----------|-------------|-----------------|
| `==`      | Igual       | `a == b` → `False` |
| `!=`      | Diferente   | `a != b` → `True` |
| `>`       | Maior       | `a > b` → `True` |
| `<`       | Menor       | `a < b` → `False` |
| `>=`      | Maior ou igual | `a >= b` → `True` |
| `<=`      | Menor ou igual | `a <= b` → `False` |

Exemplo:
```python
numero = int(input("Digite um número: "))
if numero > 0:
    print("Número positivo")
elif numero < 0:
    print("Número negativo")
else:
    print("O número é zero")
```

---

## 🚀 Operadores Lógicos (`and`, `or`, `not`)

| Operador | Descrição | Exemplo (`a = True`, `b = False`) |
|----------|-----------|----------------|
| `and`    | Retorna `True` se **ambas** as condições forem verdadeiras | `a and b` → `False` |
| `or`     | Retorna `True` se **pelo menos uma** das condições for verdadeira | `a or b` → `True` |
| `not`    | Inverte o valor lógico | `not a` → `False` |

Exemplo:
```python
idade = int(input("Digite sua idade: "))
ingressos = int(input("Quantos ingressos você tem? "))

if idade >= 18 and ingressos > 0:
    print("Você pode entrar no evento.")
else:
    print("Entrada negada.")
```

---

## 🚀 Condições em Uma Única Linha (`Ternário`)

Python permite simplificar condições com expressões condicionais em uma única linha:

```python
idade = int(input("Digite sua idade: "))
status = "Maior de idade" if idade >= 18 else "Menor de idade"
print(status)
```

---

## 🚀 Uso de `match-case` (Python 3.10+)

A estrutura `match-case` funciona de forma similar ao `switch-case` de outras linguagens, facilitando comparações diretas.

```python
opcao = input("Escolha uma opção (A, B ou C): ")

match opcao:
    case "A":
        print("Você escolheu A")
    case "B":
        print("Você escolheu B")
    case "C":
        print("Você escolheu C")
    case _:
        print("Opção inválida")
```

---

## 🎯 Exercícios

1. **Verificação de Número Par ou Ímpar**
   - Peça ao usuário um número inteiro e informe se ele é par ou ímpar.

2. **Classificação de Idade**
   - Peça a idade do usuário e classifique-o como criança (0-12), adolescente (13-17), adulto (18-59) ou idoso (60+).

3. **Sistema de Login Simples**
   - Peça um nome de usuário e uma senha. Se forem "admin" e "1234", exiba "Acesso permitido"; caso contrário, "Acesso negado".

4. **Calculadora de Descontos**
   - Peça o valor da compra e aplique um desconto de 10% se for acima de R$100.

5. **Menu de Opções**
   - Exiba um menu de opções (1. Ver saldo, 2. Depositar, 3. Sacar) e execute a ação correspondente.

---

💡 _Dominar estruturas condicionais é essencial para criar lógica eficiente nos seus programas! 🚀_
