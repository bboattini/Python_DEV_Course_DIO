# Notas
Notas relativas a tópicos novos que aprendi nesse curso
## Curso: Conhecendo a Linguagem de Programação Python

### Modo Iterativo:
* **python3 -i <file_name.py>:** facilita o teste de uma função ou classe dentro do arquivo
* **dir():** sem argumentos retorna o escopo local de atributos do arquivo, incluindo modulos e biblios importadas
  * Com uma argumento retorna todos os metodos associados a classe do argumento
* **help():** permite buscas no modo iterativo
  * Com um argumento retorna um resumo do objeto e dos métodos associados a classe do objeto

### Variáveis e Constantes:
* Em Python não possui definição de uma constante, mas usa-se a convenção de **CapsLk** na definição valores que não devem ser alterados
  * ex: CONSTANTE = 10
* Como boa prática variaveis devem ter nomes sugestivos e e em snake case
  * ex: usuarios_conta_corrente = ["João", "Maria"]
  * ex: BRAZILIAN_STATES = ["RS", "SP", "RJ"]

### Funções de Entrada e Saída:
* **print():** pode receber dois argumentos **sep: str** e **end: str** que podem ser usados para modificar a separação entre variaves e o final do output, respectivamente
* **fstring:**
  * ex: print(f"Retorna {val_1} e {val_2}")

## Curso: Tipos de Operadores com Python

### Operadores de Identidade
* Verifica se 2 objetos ocupam a mesma região de memoria
* **is:** quando entre 2 variaveis retorna **True** se elas ocuparem a mesma região de memoria, vice-versa
* **is not:** quando entre 2 variaveis retorna **True** se elas não ocuparem a mesma região de memoria, vice-versa

### Operadores de Associação
* Identifica se um objeto esta presente em uma sequência
* **in:** quando entre 2 variaveis retorna **True** se a primeira estiver contida na segunda
* **not in:** quando entre 2 variaveis retorna **True** se a primeira não estiver contida na segunda

## Curso: Estruturas Condicionais e de Repetição

### Estruturas Condicionais
* **if ternário:** permite escrever uma instrução em apenas uma linha

  _exemplo:_
  ```
  copo = "cheio" if ("agua" in copo) else "vazio"
  ```
### Estruturas de Repetição
* **break:** para sair do loop de execução
* **continue:** para pular um dos loops dentro da execução

## Curso: Dominando Strings e Fatiamento

### Conhecendo Métodos Úteis
* **upper:** coverte todos os caracteres para maiúsculo
* **lower:** coverte todos os caracteres para minusculo
* **title:** converte todos os caracteres para minusculo exeto o primeiro que é convertido para maiusculo
* **strip:** elimita espaços em branco nas extreidades do string
  * **lstrip:** elimina espaços à esquerda
  * **rstrip:** elimina espaços à direita
* **center:** bom para fazer bons menus em interfácie programável
```
<string_variable>.center(char_len, filling_char)
```
_exemplo_
```
curso = "Python"
n = len(curso)
print(curso.center(n+4, "#"))
>> ##Python##
```
* **join:** adiciona variaveis entre caracteres do iteravel

_exemplo_
```
curso = "Python"
n = len(curso)
print(".".join(curso))
>> ##Python##
```
### Interpolação de Variaveis string
* **format:** pode ser usado com dicionário
  _exemplo_
  ```
  dados = ["pi": 3.1415, "nome": "Bernardo"]
  print(f"Hello! My name is {nome}, and you can assume PI as {pi:.2}.".format(**dados))
  >> Hello! My name is Bernardo, and you can assume PI as 3.14.
  ```
* **f-string:** melhor forma de formatar string

  _exemplo_
  ```
  price = 45,52
  nome = "Bernardo"
  discovery = 2100
  print(f"Hello! My name is {nome}, the course price is {price:2.}.")
  >> Hello! My name is Bernardo, the couse price is 45.
  ```
### Fatiamento de string
```
<string_variable>[begin:end:interval]
```
