## Atividade – Prompt Mestre em Programação de Computadores  
### Tema: Funções em Python

---

### Prompt Mestre Inicial

**Prompt:**  
Escreva uma função em Python que receba dois números e retorne a soma deles.

---

### Variação 1

**Prompt:**  
Escreva a função em Python e explique passo a passo como funciona.

**Resposta do LLM:**
```python
soma = 0

for numero in range(1, 101):
    if numero % 2 == 0:
        soma += numero

print("A soma dos números pares de 1 a 100 é:", soma)
```

**Explicação:**  
**1.** 
`soma = 0`
Criamos uma variável chamada `soma`
Ela começa com valor 0, pois ainda não somamos nada

 **2.** 
`for numero in range(1, 101):`
O `range(1, 101)` gera números de **1 até 100**.
O `for` percorre cada número, um por vez.
A variável `numero` vai assumir valores: 1, 2, 3, ..., 100

**3.**  `if numero % 2 == 0:`
Aqui verificamos se o número é par
O operador `%` é o módulo (resto da divisão).

Exemplo:
`4 % 2 = 0` → par ✅

`5 % 2 = 1` → ímpar ❌

Então, só entra no if se o número for par.

**4.** 
`soma += numero`
Isso é o mesmo que: `soma = soma + numero`
Vai acumulando os números pares
Exemplo do que acontece:
soma = 0
soma = 0 + 2 → 2
soma = 2 + 4 → 6
soma = 6 + 6 → 12
...

**5.** 
`print(...)`
Mostra o resultado final na tela

---

### Variação 2

**Prompt:**  
otimizando o programa em python, usando compreensao em listas

**Resposta do LLM :**
```python
soma = sum([numero for numero in range(1, 101) if numero % 2 == 0])
print("A soma dos números pares de 1 a 100 é:", soma)
```

---

### Variação 3
**Prompt:**  
otimizando o programa em python, usando compreensao em listas

**Resposta do LLM :**

🪜 Passo a passo simples

**1.** `range(1, 101)`

Pense nisso como:
“me dê os números de 1 até 100”

**2.** `for numero in range(...)`

Aqui é como se o programa dissesse:
“vou olhar um número de cada vez”

Tipo:

pega o 1
depois o 2
depois o 3
... até o 100

**3.** `if numero % 2 == 0`

Isso verifica se o número é par

💡 Regra simples:

Se dá resto 0, é par
Se dá resto 1, é ímpar

Exemplo:

4 ÷ 2 → resto 0 ✅
5 ÷ 2 → resto 1 ❌

**4.**  `numero for numero ... if ...`

Aqui acontece:

“pegue só os números que passaram no teste (os pares)”

Então o programa basicamente cria isso:

`2, 4, 6, 8, ..., 100`

**5.** `sum(...)`

Agora ele faz:

“some todos esses números”

**6.** `print(...)`

Mostra o resultado na tela

🧠 Explicação em uma frase

👉 O programa:

“olha todos os números de 1 a 100, pega só os pares e soma tudo”

---

### Reflexão

Ao modificar os prompts, é possível perceber que pequenas mudanças nas instruções influenciam diretamente nas respostas geradas.  

A versão com explicação foi a mais útil para o aprendizado, pois facilitou o entendimento do funcionamento da função.  
Já a versão com validação mostrou uma aplicação mais prática e segura do código.  Isso demonstra que a engenharia de prompt pode ser usada para obter respostas mais completas,
adaptadas ao nível de conhecimento e à necessidade do programador.
