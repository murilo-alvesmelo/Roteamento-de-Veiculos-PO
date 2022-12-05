
# Roteamento de Veiculos - Pesquisa Operacional


## Modelo Matemático

        O modelo matemático apresentado para o PRV, tem como objetivo a minimização 
    do custo para constatar o movimento do cliente i para o cliente j, vezes a variável de decisão i j, se 
    realmente houver o movimento do cliente i para o cliente j, sendo assim faremos um somatório para todos os arcos possíveis sujeito as seguintes restrições.
    
        Primeira restrição é que para todo cliente i temos que ter um arco saindo deste cliente.
    
        Para todo cliente j temos que ter exatamente um arco entrando nesse cliente.
    
        Para o deposito x0 encontraremos exatamente k arcos saindo desse deposito, sendo que K é o numero de rotas ou número de veículos.
    
        A última restrição diz respeito a eliminação de subciclos veremos que para todo subconjunto S dos clientes o numero de arestas que saem desse subconjunto que tem origem dentro desse conjunto  e destino fora desse subconjunto deve ser maior ou igual ao R de S, onde esse r de s significa o número mínimo de rotas necessárias para servir os clientes que estão dentro desse subconjunto, e a ultima restrição é a definição da variável x i j como sendo variável binária ou seja apenas admite valores 0 ou 1.
