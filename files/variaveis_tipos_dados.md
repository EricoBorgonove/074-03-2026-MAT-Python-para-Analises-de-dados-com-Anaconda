# 📝 Tipos de Dados e Variáveis em Python

Neste documento, abordaremos os tipos de dados disponíveis em Python e como utilizar variáveis de forma eficiente.

---

## 📌 O que são Variáveis?

Variáveis são espaços na memória onde armazenamos valores que podem ser utilizados e manipulados ao longo do programa.

### 🛠 Declaração de Variáveis

Em Python, não precisamos especificar o tipo da variável. O interpretador infere o tipo automaticamente:
```python
nome = "Alice"  # String
idade = 25  # Inteiro
altura = 1.68  # Float
estudante = True  # Booleano
```

**Regras para nomeação de variáveis:**
- Devem começar com uma letra ou underscore (`_`), mas não com um número.
- Não podem conter espaços nem caracteres especiais (exceto `_`).
- Python diferencia maiúsculas de minúsculas (`Nome` e `nome` são diferentes).
- Evite palavras reservadas da linguagem (`def`, `class`, `if`, etc.).

---

## 📌 Tipos de Dados em Python

Python possui vários tipos de dados embutidos que podem ser classificados em diferentes categorias.

### 🔹 Tipos Numéricos

1. **Inteiro (`int`)**: Números inteiros positivos ou negativos.
   ```python
   idade = 30
   ano = 2024
   numero_negativo = -15
   ```

2. **Ponto Flutuante (`float`)**: Números decimais.
   ```python
   pi = 3.1415
   altura = 1.75
   ```

3. **Números Complexos (`complex`)**: Usados para operações matemáticas avançadas.
   ```python
   numero_complexo = 2 + 3j
   ```

### 🔹 Tipo Booleano (`bool`)

Os valores booleanos representam **Verdadeiro (`True`)** ou **Falso (`False`)**.
```python
ativo = True
concluido = False
```

### 🔹 Tipo String (`str`)

As strings representam textos e podem ser declaradas com aspas simples (`'`) ou duplas (`"`).
```python
mensagem = "Olá, mundo!"
nome = 'Python'
```

Podemos concatenar strings:
```python
frase = "Bem-vindo ao " + "Python!"
```

E acessar caracteres individualmente:
```python
texto = "Python"
print(texto[0])  # P
print(texto[-1])  # n
```

### 🔹 Estruturas de Dados

Python oferece estruturas para armazenar coleções de valores.

#### 📌 Listas (`list`)
Listas armazenam múltiplos valores e podem conter diferentes tipos de dados.
```python
numeros = [1, 2, 3, 4, 5]
mistos = [10, "Python", True, 3.14]
```

Podemos acessar elementos pelo índice:
```python
print(numeros[0])  # 1
print(mistos[-1])  # 3.14
```

E modificar elementos:
```python
numeros[2] = 100
```

#### 📌 Tuplas (`tuple`)
Tuplas são similares às listas, mas são **imutáveis** (não podem ser alteradas após a criação).
```python
coordenadas = (10, 20)
```

#### 📌 Conjuntos (`set`)
Os conjuntos armazenam valores **únicos e desordenados**.
```python
cores = {"vermelho", "azul", "verde"}
```

#### 📌 Dicionários (`dict`)
Dicionários armazenam **pares chave-valor**.
```python
aluno = {"nome": "Carlos", "idade": 21, "curso": "Computação"}
```

Acessamos os valores pelas chaves:
```python
print(aluno["nome"])  # Carlos
```

---

## 📌 Conversão de Tipos

Podemos converter tipos usando funções como `int()`, `float()`, `str()`, etc.
```python
numero = "25"
print(int(numero) + 5)  # 30
```

---

## 🎯 Exercícios

1. **Criação de Variáveis**
   - Declare variáveis para armazenar seu nome, idade, altura e se é estudante.

2. **Manipulação de Strings**
   - Peça ao usuário para inserir seu nome e exiba a primeira e última letra.

3. **Listas e Dicionários**
   - Crie uma lista com cinco números e um dicionário com informações de uma pessoa.

4. **Conversão de Tipos**
   - Converta uma string em número e realize uma soma.

5. **Operações com Conjuntos**
   - Crie dois conjuntos com cores e exiba a interseção entre eles.

---

💡 _Compreender os tipos de dados e variáveis é essencial para dominar Python! 🚀_
