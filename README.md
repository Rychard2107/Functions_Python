# Funções Úteis do Python para Iniciantes
Aqui estão algumas das funções mais úteis do Python para quem está começando. Essas funções ajudam a manipular dados, trabalhar com strings, listas, dicionários e muito mais!

## 1. Funções para Manipulação de Dados
### `len()`
Retorna o tamanho de um objeto (lista, string, dicionário, etc.).

```
lista = [1, 2, 3, 4]
print(len(lista))  # Saída: 4
```
### `sum()`
Retorna a soma dos elementos de uma lista ou tupla.

```
numeros = [10, 20, 30]
print(sum(numeros))  # Saída: 60
```
### `min()` e `max()`
Retornam o menor e o maior valor de uma sequência, respectivamente.

```
valores = [5, 3, 9, 1]
print(min(valores))  # Saída: 1
print(max(valores))  # Saída: 9
```
### `sorted()`
Retorna uma nova lista com os elementos ordenados.

```
numeros = [3, 1, 4, 2]
print(sorted(numeros))  # Saída: [1, 2, 3, 4]
```
## 2. Funções para Trabalhar com Strings
### `str()`
Converte um objeto em uma string.

```
numero = 42
print(str(numero) + " é a resposta")  # Saída: 42 é a resposta
```
### `upper()` e `lower()`
Convertem uma string para maiúsculas ou minúsculas.

```
texto = "Olá, Mundo!"
print(texto.upper())  # Saída: OLÁ, MUNDO!
print(texto.lower())  # Saída: olá, mundo!
```
### `strip()`
Remove espaços em branco no início e no final de uma string.

```
texto = "   Python é incrível!   "
print(texto.strip())  # Saída: "Python é incrível!"
```
### `split()`
Divide uma string em uma lista com base em um separador.

```
frase = "Python é divertido"
print(frase.split(" "))  # Saída: ['Python', 'é', 'divertido']
```
## 3. Funções para Listas e Iteráveis
### `append()`
Adiciona um elemento ao final de uma lista.

```
lista = [1, 2, 3]
lista.append(4)
print(lista)  # Saída: [1, 2, 3, 4]
```
### `extend()`
Adiciona vários elementos a uma lista.

```
lista = [1, 2, 3]
lista.extend([4, 5])
print(lista)  # Saída: [1, 2, 3, 4, 5]
```
### `map()`
Aplica uma função a todos os elementos de uma lista.

```
def dobrar(x):
    return x * 2

numeros = [1, 2, 3]
resultado = list(map(dobrar, numeros))
print(resultado)  # Saída: [2, 4, 6]
```
### `filter()`
Filtra elementos de uma lista com base em uma condição.

```
def eh_par(x):
    return x % 2 == 0

numeros = [1, 2, 3, 4, 5]
resultado = list(filter(eh_par, numeros))
print(resultado)  # Saída: [2, 4]
```
## 4. Funções para Dicionários
### `keys()` e `values()`
Retornam as chaves e os valores de um dicionário, respectivamente.

```
dados = {"nome": "Afonso", "idade": 20}
print(dados.keys())  # Saída: dict_keys(['nome', 'idade'])
print(dados.values())  # Saída: dict_values(['Afonso', 20])
```
### `items()`
Retorna uma lista de tuplas com as chaves e valores de um dicionário.

```
dados = {"nome": "Afonso", "idade": 20}
print(dados.items())  # Saída: dict_items([('nome', 'Afonso'), ('idade', 20)])
```
## 5. Funções para Trabalhar com Arquivos
### `open()`
Abre um arquivo para leitura ou escrita.

```
# Lendo um arquivo
with open("arquivo.txt", "r") as arquivo:
    conteudo = arquivo.read()
    print(conteudo)
```
```
# Escrevendo em um arquivo
with open("arquivo.txt", "w") as arquivo:
    arquivo.write("Olá, mundo!")
```
## 6. Funções Úteis Gerais
### `type()`
Retorna o tipo de um objeto.

```
print(type(42))  # Saída: <class 'int'>
print(type("Olá"))  # Saída: <class 'str'>
```
### `isinstance()`
Verifica se um objeto é uma instância de uma classe.

```
numero = 42
print(isinstance(numero, int))  # Saída: True
```
### `range()`
Gera uma sequência de números.

```
for i in range(5):
    print(i)  # Saída: 0, 1, 2, 3, 4
```
### `enumarate()`
Retorna o índice e o valor de cada item em uma lista.

```
frutas = ["maçã", "banana", "laranja"]
for indice, fruta in enumerate(frutas):
    print(f"{indice}: {fruta}")

# Saída:
# 0: maçã
# 1: banana
# 2: laranja
```
## 7. Funções Avançadas (mas Úteis!)
### `zip()`
Combina duas ou mais listas em uma lista de tuplas.

```
nomes = ["Afonso", "Maria", "João"]
idades = [20, 25, 30]
print(list(zip(nomes, idades)))  # Saída: [('Afonso', 20), ('Maria', 25), ('João', 30)]
```
### `lambda`
Cria funções anônimas (pequenas e sem nome).

```
dobrar = lambda x: x * 2
print(dobrar(5))  # Saída: 10
```