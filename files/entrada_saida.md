# 📌 Comandos de Entrada e Saída em Python

Os comandos de entrada e saída em Python são essenciais para interagir com o usuário, permitindo que o programa receba dados e exiba informações.

---

## 🚀 Entrada de Dados (`input`)

O comando `input()` permite que o usuário insira dados durante a execução do programa. O valor inserido sempre será do tipo `str` (string), então é necessário convertê-lo para outros tipos, se necessário.

### 📌 Sintaxe Básica
```python
entrada = input("Digite algo: ")
print("Você digitou:", entrada)
```

### 🛠 Conversão de Tipos
Se precisar de um número inteiro (`int`) ou decimal (`float`), use a conversão:
```python
idade = int(input("Digite sua idade: "))
altura = float(input("Digite sua altura: "))
print(f"Você tem {idade} anos e {altura}m de altura.")
```

---

## 🚀 Saída de Dados (`print`)

O comando `print()` exibe informações na tela. Ele pode imprimir strings, números e variáveis.

### 📌 Sintaxe Básica
```python
print("Olá, mundo!")
nome = "Alice"
print("Olá,", nome)
```

### 🛠 Concatenação de Strings
```python
nome = "Carlos"
idade = 25
print("Nome: " + nome + ", Idade: " + str(idade))
```

### 🛠 Interpolação (`f-strings`)
Uma maneira mais moderna de formatar strings:
```python
nome = "Mariana"
idade = 30
print(f"Meu nome é {nome} e tenho {idade} anos.")
```

### 🛠 Sep e End no `print()`
Podemos modificar a saída do `print()` utilizando `sep` e `end`:
```python
print("Python", "é", "incrível", sep=" - ")  # Saída: Python - é - incrível
print("Linha 1", end=" ")
print("continua na mesma linha.")
```

---

## 🎯 Exercícios

1. **Solicitar Nome e Idade**
   - Peça ao usuário para digitar seu nome e idade e exiba uma mensagem formatada.

2. **Soma de Dois Números**
   - Solicite dois números ao usuário, some-os e exiba o resultado.

3. **Formatação de Saída**
   - Peça o nome de um produto, o preço e exiba no formato: `Produto: [nome], Preço: R$ [preço]`.

4. **Cálculo de Média**
   - Solicite três notas ao usuário, calcule a média e exiba o resultado formatado.

5. **Personalizando Print**
   - Exiba três palavras separadas por `***` e finalize a linha com `!` ao invés da quebra padrão.

---

💡 _Com esses conceitos, você já pode criar programas interativos! 🚀_
