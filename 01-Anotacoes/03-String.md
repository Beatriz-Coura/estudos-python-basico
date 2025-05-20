### O que são Strings?

A **`string`** em Python é uma sequência de caracteres usada para armazenar textos. Ela pode ser definida com **aspas simples (`'`)**, **aspas duplas (`"`)**, ou **aspas triplas (`''' """`)** para textos longos.

---

### **Criando Strings**

```python
texto1 = 'Olá, mundo!'
texto2 = "Python é incrível!"
texto3 = '''Este é um texto
com várias linhas.'''

```

- **Aspas simples** e **duplas** podem ser usadas indistintamente.
- **Aspas triplas** permitem **múltiplas linhas**.

---

### **Acessando Caracteres**

```python
palavra = "Python"
print(palavra[0])  # P (primeiro caractere)
print(palavra[-1]) # n (último caractere)

```

- Os **índices começam em 0**.
- Use **índices negativos** para contar de trás para frente.

---

### **Fatiamento (`Slicing`)**

```python
frase = "Aprendendo Python"
print(frase[0:10])  # Aprendendo
print(frase[:8])    # Aprenden (do início até índice 7)
print(frase[3:])    # endendo Python (do índice 3 até o final)

```

- `string[início:fim]` → Retorna parte da string.
- O **"fim"** não é incluído no resultado.

---

### **Métodos Úteis**

```python
texto = "  Olá, Python!  "
print(texto.lower())     # "  olá, python!  " (tudo minúsculo)
print(texto.upper())     # "  OLÁ, PYTHON!  " (tudo maiúsculo)
print(texto.strip())     # "Olá, Python!" (remove espaços extras)
print(texto.replace("Python", "Mundo"))  # "  Olá, Mundo!  "
print(texto.split())     # ['Olá,', 'Python!'] (separa por espaços)

```

- **`lower()`** → Transforma tudo em minúsculo.
- **`upper()`** → Transforma tudo em maiúsculo.
- **`strip()`** → Remove espaços extras no início e no fim.
- **`replace(a, b)`** → Substitui `a` por `b`.
- **`split()`** → Divide a string em uma lista de palavras.

---

### **Concatenação e Repetição**

```python
a = "Olá"
b = "Mundo"
print(a + " " + b)  # "Olá Mundo" (concatenação)
print(a * 3)  # "OláOláOlá" (repetição)

```

- **`+`** une strings.
- **`*`** repete a string `n` vezes.

---

### **Verificando Substrings**

```python
frase = "Aprender Python é divertido"
print("Python" in frase)   # True (existe na string)
print("Java" not in frase) # True (não existe na string)

```

- **`in`** verifica se um texto está dentro de outro.
- **`not in`** verifica se um texto NÃO está dentro de outro.

---

### **Formatando Strings**

```python
nome = "Beatriz"
idade = 19
print(f"Meu nome é {nome} e tenho {idade} anos.")  # Usando f-strings
print("Meu nome é {} e tenho {} anos.".format(nome, idade))  # Usando format()

```

- **F-strings (`f"..."`)** são a forma mais moderna e recomendada.
- **`format()`** também funciona, mas é mais verboso.

---

### **Resumo**

Strings são sequências de caracteres.

Pode-se acessar caracteres por índice.

Fatiamento (`slicing`) permite pegar partes da string.

Métodos como `lower()`, `upper()`, `strip()`, `replace()`, `split()` ajudam no processamento.

`+` concatena e `*` repete strings.

F-strings (`f"..."`) facilitam a formatação.