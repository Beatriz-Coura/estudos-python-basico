### Código de Estrutura Sequencial

```python
# Solicita entrada do usuário
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

# Calcula a soma
soma = num1 + num2

# Exibe o resultado
print("A soma dos números é:", soma)
```

🔹 **Exemplo:**

1. **Entrada de dados** → O usuário digita dois números.
2. **Processamento** → A soma dos dois números é calculada.
3. **Saída de dados** → O resultado é exibido na tela.

### **Introdução ao Python**

Python é uma **linguagem de programação de alto nível, interpretada e multiparadigma** (suporta programação procedural, orientada a objetos e funcional). Sua sintaxe simples e legível a torna uma das linguagens mais populares no mundo da tecnologia.

---

### **Características principais**

**Fácil de aprender** → Sintaxe simples e intuitiva.

**Portável** → Funciona em diferentes sistemas operacionais.

**Interpretada** → Executada linha por linha, sem necessidade de compilação.

**Multiparadigma** → Suporta diferentes estilos de programação.

**Bibliotecas poderosas** → Diversas bibliotecas para ciência de dados, web, automação, IA, etc.

---

### **Estruturas básicas**

### **Variáveis e Tipos de Dados**

Python não exige declaração de tipos:

```python
nome = "Alice"  # String
idade = 25      # Inteiro
altura = 1.75   # Float
ligado = True   # Booleano

```

### **Entrada e Saída de Dados**

```python
nome = input("Digite seu nome: ")  # Entrada
print("Olá,", nome)  # Saída

```

### **Operadores Matemáticos**

```python
soma = 5 + 3     # Adição
subtracao = 5 - 2  # Subtração
multiplicacao = 4 * 3  # Multiplicação
divisao = 10 / 2  # Divisão (float)
modulo = 10 % 3   # Resto da divisão

```

### **Estruturas Condicionais (if-else)**

```python
idade = int(input("Digite sua idade: "))

if idade >= 18:
    print("Você é maior de idade!")
else:
    print("Você é menor de idade.")

```

### **Estruturas de Repetição (for e while)**

```python
# For - Percorrendo uma lista
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4

# While - Executa enquanto a condição for verdadeira
contador = 0
while contador < 5:
    print(contador)
    contador += 1

```

### **Listas, Tuplas e Dicionários**

```python
# Lista (mutável)
frutas = ["maçã", "banana", "uva"]
frutas.append("laranja")  # Adiciona um elemento

# Tupla (imutável)
cores = ("azul", "vermelho", "verde")

# Dicionário (chave-valor)
pessoa = {"nome": "Carlos", "idade": 30, "cidade": "São Paulo"}
print(pessoa["nome"])  # Acessando valor pela chave

```

### **Funções**

```python
def saudacao(nome):
    return "Olá, " + nome + "!"

print(saudacao("Lucas"))

```

---

### **Conclusão**

Python é uma linguagem versátil, usada em diversas áreas como **desenvolvimento web, automação, ciência de dados, inteligência artificial e segurança da informação**. Sua sintaxe simples facilita o aprendizado, tornando-se uma ótima escolha tanto para iniciantes quanto para programadores experientes.
