### O que são listas?

A **`lista`** em Python é uma estrutura de dados que permite armazenar múltiplos valores em uma única variável. Elas são **mutáveis**, ou seja, podem ser alteradas após a criação.

---

### **Criando Listas**

```python
numeros = [1, 2, 3, 4, 5]  # Lista de números
nomes = ["Ana", "Bruno", "Carlos"]  # Lista de strings
mista = [10, "Python", True, 3.14]  # Lista com diferentes tipos de dados
vazia = []  # Lista vazia

```

- As listas são definidas com **colchetes `[ ]`**.
- Podem conter **diferentes tipos de dados**.
- Também podem ser **criadas vazias** e preenchidas depois.

---

### **Acessando Elementos**

```python
frutas = ["Maçã", "Banana", "Uva", "Morango"]
print(frutas[0])   # Maçã (primeiro elemento)
print(frutas[-1])  # Morango (último elemento)

```

- Os **índices começam em 0**.
- Índices **negativos** acessam elementos de trás para frente.

---

### **Modificando Listas**

```python
frutas[1] = "Pera"  # Substitui "Banana" por "Pera"
print(frutas)  # ['Maçã', 'Pera', 'Uva', 'Morango']

```

- As listas **podem ser alteradas** após a criação.

---

### **Fatiamento (`Slicing`)**

```python
numeros = [10, 20, 30, 40, 50, 60]
print(numeros[1:4])   # [20, 30, 40] (índice 1 até 3)
print(numeros[:3])    # [10, 20, 30] (do início até índice 2)
print(numeros[3:])    # [40, 50, 60] (do índice 3 até o final)
print(numeros[::2])   # [10, 30, 50] (pula de 2 em 2)

```

- `lista[início:fim]` retorna uma **parte** da lista.
- O índice **final não é incluído**.
- `lista[::passo]` define um intervalo entre os elementos.

---

### **Adicionando e Removendo Elementos**

```python
numeros = [1, 2, 3]

numeros.append(4)     # Adiciona 4 ao final
numeros.insert(1, 10) # Insere 10 na posição 1
print(numeros)        # [1, 10, 2, 3, 4]

numeros.remove(2)     # Remove o valor 2
ultimo = numeros.pop() # Remove o último elemento (4)
print(numeros)        # [1, 10, 3]

```

- **`append(valor)`** adiciona ao final.
- **`insert(índice, valor)`** insere na posição desejada.
- **`remove(valor)`** remove o primeiro valor encontrado.
- **`pop()`** remove e retorna o último elemento.

---

### **Verificando e Ordenando**

```python
cores = ["vermelho", "azul", "verde"]

print("azul" in cores)  # True (verifica se "azul" está na lista)

cores.sort()  # Ordena em ordem alfabética
print(cores)  # ['azul', 'verde', 'vermelho']

numeros = [3, 1, 4, 2]
numeros.sort(reverse=True)  # Ordena em ordem decrescente
print(numeros)  # [4, 3, 2, 1]

```

- **`in`** verifica se um elemento está na lista.
- **`sort()`** ordena em ordem crescente/alfabética.
- **`sort(reverse=True)`** ordena em ordem decrescente.

---

### **Percorrendo Listas (`for` e `while`)**

```python
frutas = ["Maçã", "Banana", "Uva"]

for fruta in frutas:
    print(fruta)  # Imprime cada fruta

# Usando índice
for i in range(len(frutas)):
    print(frutas[i])  # Acessando via índice

```

- O **`for` percorre** os elementos diretamente.
- O **`range(len(lista))`** permite usar índices.

---

### **Compreensão de Listas (`List Comprehension`)**

```python
numeros = [1, 2, 3, 4, 5]
quadrados = [x ** 2 for x in numeros]  # [1, 4, 9, 16, 25]
pares = [x for x in numeros if x % 2 == 0]  # [2, 4]

```

- Uma forma **mais compacta** de criar listas.
- Permite aplicar **operações e filtros** diretamente.

---

### **Resumo**

**Listas são mutáveis** e podem conter **diferentes tipos de dados**.

Podem ser **acessadas via índice** e **modificadas**.

Permitem **fatiamento (`slicing`)** e **ordenamento (`sort()`)**.

Métodos como `append()`, `insert()`, `remove()` e `pop()` facilitam manipulação.

**Compreensão de listas** (`List Comprehension`) cria listas de forma eficiente.
