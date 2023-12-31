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
