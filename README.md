# Roteamento de Veiculos - Pesquisa Operacional


## Modelo Matemático

        O modelo matemático apresentado para o PRV, tem como objetivo a minimização 
    do custo para constatar o movimento do cliente i para o cliente j, vezes a variável de decisão i j, se 
    realmente houver o movimento do cliente i para o cliente j, sendo assim faremos um somatório para todos 
    os arcos possíveis sujeito as seguintes restrições.
    
        Primeira restrição é que para todo cliente i temos que ter um arco saindo deste cliente.
    
        Para todo cliente j temos que ter exatamente um arco entrando nesse cliente.
    
        Para o deposito x0 encontraremos exatamente k arcos saindo desse deposito, 
        sendo que K é o numero de rotas ou número de veículos.
    
        A última restrição diz respeito a eliminação de subciclos veremos que para todo subconjunto S dos clientes
        o numero de arestas que saem desse subconjunto que tem origem dentro desse conjunto  e destino 
        fora desse subconjunto deve ser maior ou igual ao R de S, onde esse r de s significa o número 
        mínimo de rotas necessárias para servir os clientes que estão dentro desse subconjunto, e a ultima 
        restrição é a definição da variável x i j como sendo variável binária ou seja apenas admite valores 0 ou 1.

## Estudo de caso

### Algoritmo Gillett e Miller 
        Gillett e Miller (1974) é uma heurística baseada na noção de economias, que dividem o problema em partes 
        para resolvê-lo como estratégia, como ilustra a Figura 1. Onde na primeira etapa dessa heurística, 
        os vértices (pontos de demandas) são agrupados segundo algum critério de proximidade.
![Untitled(1)](https://user-images.githubusercontent.com/83835393/205767474-56472a49-abd7-43be-9814-b49d0c8a0986.png)

### Algoritmo Hill-climbing
        o Algoritmo Descida de Encosta é uma técnica de busca local, baseada em profundidade,
    sua heurística de busca local ajusta a posição de uma solução candidata (vizinha) somente se a nova 
    posição for melhor que a posição prévia.
        A otimização deste algoritmo ocorre por meio da avaliação de soluções vizinhas de uma
    solução ou estado atual. O algoritmo avalia as soluções vizinhas com base na função de
    avaliação (fitness). A cada etapa do algoritmo, a solução gerada pelo estado corrente é
    substituída pela solução representada pelo melhor vizinho. O algoritmo encerra quando
    alcança um pico ou seja quando não encontra vizinho melhor que o estado atual

![Untitled](https://user-images.githubusercontent.com/83835393/205768025-dc96527a-1f8a-49bf-b2e3-74f3a381c39b.png)

## Estratégia Proposta para Solução do problema de roteamento de veiculos

        A representação do cromossomo de um algoritmo genético é gerada baseada em uma matriz binaria. 
    Com o objetivo de resolver o problema de roteamento de veículos, temos o exemplo de 7 clientes e 2 veículos, 
    assim as 7 primeiras colunas representam os clientes a serem atendidos pelos veículos, e as 6 ultimas são espaço 
    para permutações da matriz que representam a ordem dos clientes por veículo. A matriz por completo 
    é denominada matriz de permutação
