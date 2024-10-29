## Função funq4 


## Descrição
A função `funq4` é uma implementação em Haskell que gera uma lista de pares de strings. Cada par contém a linha e uma cor que alterna entre "white" e "gray". A regra pra mostrar a cor é com base na imparidade do número associado.


   ## Implementação
   
![funq4](https://github.com/user-attachments/assets/d95dd096-6a1c-4359-8455-490286b03a19)

   
## Funcionamento
1. Geração dos Pares: A expressão zip [10, 11..] [1, 2..] combina duas listas.
2. "Take n" : usa o argumento para limite dos pares.
3. List Comprehension: Para cada par (i, j).
4. Função color

## Possiveis Erros ⚠️
Confundir o parâmetro n, tratando-o como um valor a ser somado aos índices gerados.Resulta em pares começando por "line14" em vez de "line10". Foi o que eu fiz na prova...😓

## Diferenças entre Paradigmas: Haskell vs. C 🔍

A confusão em relação ao uso do parâmetro n pode ser atribuída às diferenças entre os paradigmas de programação:

- **Em C (Paradigma Imperativo)**: Parâmetros são frequentemente manipulados diretamente e podem ser usados para modificar estados. Programadores podem esperar que um parâmetro seja um valor a ser adicionado.

- **Em Haskell (Paradigma Funcional)**: Os parâmetros servem como limites ou critérios, e não são utilizados para manipulação direta de valores. A função é definida para retornar um resultado baseado em condições sem modificar estados externos.


## Conclusão 🎯


https://github.com/user-attachments/assets/36b29a0a-4f71-4e8b-924e-6b719db929c4


Com funq4, abordamos os seguintes conceitos:

- **List Comprehension**
- **Funções High-Order**: Zip
- **Where**
- **Condições**: lógica condicional
