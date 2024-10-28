# Função `funq4`

## Descrição

A função `funq4` é uma implementação em Haskell que gera uma lista de pares de strings. Cada par contém a linha e uma cor que alterna entre "white" e "gray". A regra pra mostrar a cor é com base na imparidade do número associado.

## Implementação

```haskell
funq4 :: Int -> [(String, String)]
funq4 n = [fun (i, j) | (i, j) <- take n $ zip [10, 11..] [1, 2..]]
  where
    fun (i, j) = ("line" ++ show i, color j)
    color k = if odd k then "white" else "gray"

Funcionamento
1. Geração dos Pares: A expressão zip [10, 11..] [1, 2..] combina duas listas.
2. "Take n" : usa o argumento para limite dos pares.
3. List Comprehension: Para cada par (i, j).
4. Função color 


##Possíveis Erros ⚠️

Confundir o parâmetro n, tratando-o como um valor a ser somado aos índices gerados.Resulta em pares começando por "line14" em vez de "line10". Foi o que eu fiz na prova...😓

##Diferenças entre Paradigmas: Haskell vs. C 🔍

A confusão em relação ao uso do parâmetro n pode ser atribuída às diferenças entre os paradigmas de programação:

- **Em C (Paradigma Imperativo)**: Parâmetros são frequentemente manipulados diretamente e podem ser usados para modificar estados. Programadores podem esperar que um parâmetro seja um valor a ser adicionado.

- **Em Haskell (Paradigma Funcional)**: Os parâmetros servem como limites ou critérios, e não são utilizados para manipulação direta de valores. A função é definida para retornar um resultado baseado em condições sem modificar estados externos.

## Conclusão 🎯:

Com funq4, abordamos os seguintes conceitos:

**List Comprehension**
**Funções High-Order**: Zip
**Where**
**Condições**: lógica condicional com base na imparidade. 





