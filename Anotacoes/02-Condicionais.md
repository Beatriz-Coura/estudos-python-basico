### **O que é if e else em Python?**

O `if` e `else` são estruturas condicionais em Python que permitem tomar decisões no código.

---

### **if (Se)**

Usado para verificar uma condição. Se a condição for verdadeira (`True`), o bloco de código indentado será executado.

🔹 **Exemplo:**

```python
idade = 18

if idade >= 18:  # Se a idade for maior ou igual a 18
    print("Você é maior de idade!")  # Executa essa linha

```

✔ Se `idade = 20`, a mensagem será exibida.

❌ Se `idade = 15`, nada acontece (porque a condição é falsa).

---

### **else (Senão)**

Usado para definir o que acontece se a condição do `if` for falsa (`False`).

🔹 **Exemplo:**

```python
idade = 16

if idade >= 18:
    print("Você pode entrar na festa!")
else:
    print("Entrada negada, menor de idade.")

```

✔ Se `idade = 16`, o `else` será executado, exibindo **"Entrada negada, menor de idade."**.

---

### **elif (Else If)**

Usado quando há mais de uma condição a ser verificada.

🔹 **Exemplo:**

```python
nota = 75

if nota >= 90:
    print("Aprovado com excelência!")
elif nota >= 60:
    print("Aprovado")
else:
    print("Reprovado")

```

✔ Se `nota = 75`, imprime **"Aprovado"**.

✔ Se `nota = 95`, imprime **"Aprovado com excelência!"**.

✔ Se `nota = 50`, imprime **"Reprovado"**.

---

### **Resumo**

**`if`** → Executa se a condição for verdadeira.

**`else`** → Executa se a condição do `if` for falsa.

**`elif`** → Adiciona mais condições antes do `else`.

### Extra

### **Condições Múltiplas com `and` e `or`**

```python
idade = 20
renda = 2500

# Ambas as condições devem ser verdadeiras
if idade >= 18 and renda >= 2000:
    print("Aprovado para o crédito")

# Pelo menos uma das condições precisa ser verdadeira
if idade >= 18 or renda >= 2000:
    print("Pode solicitar crédito")

```

🔹 **`and` → Todas as condições precisam ser `True`**.

🔹 **`or` → Pelo menos uma condição precisa ser `True`**.

---

### **Condições Aninhadas**

```python
idade = 20
tem_ingresso = True

if idade >= 18:
    if tem_ingresso:
        print("Entrada permitida!")
    else:
        print("Você precisa de um ingresso.")
else:
    print("Entrada negada, menor de idade.")

```

🔹 **Um `if` dentro de outro `if`** permite verificações mais detalhadas.

---

### **Operador Ternário (`if` em uma linha)**

```python
idade = 18
status = "Maior de idade" if idade >= 18 else "Menor de idade"
print(status)

```

🔹 **Forma compacta do `if-else`** para expressões curtas.

---

### **Comparação com `in`**

```python
vogais = "aeiou"
letra = input("Digite uma letra: ").lower()

if letra in vogais:
    print("É uma vogal!")
else:
    print("É uma consoante!")

```

🔹 **`in` verifica se um valor está dentro de uma lista, string ou tupla**.

---

### **`if` com Números e Strings**

```python
# Números: 0 é considerado False, qualquer outro número é True
if 0:
    print("Isso nunca será impresso")
if -5:
    print("Isso será impresso")

# Strings: String vazia é False, qualquer outra string é True
if "":
    print("Não imprime")
if "Python":
    print("Python é verdadeiro!")

```

🔹 **Valores "falsy" (considerados `False`) em Python**: `0`, `""`, `None`, `False`, `[]`, `{}`, `set()`.

🔹 **Valores "truthy" (considerados `True`)**: Qualquer valor diferente dos acima.

---

### **Dicas Importantes**

**Sempre use indentação correta** (4 espaços por nível).

**Evite aninhar muitos `if`s**, prefira `elif`.

**Cuidado com `or` e `and`**, para evitar erros lógicos.

**O operador ternário (`if` inline) é útil, mas não exagere para não prejudicar a legibilidade do código.**
