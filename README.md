# **DBSCAN** - *Density-based spatial clustering of applications with noise*


## Definição
- É um algoritmo de agrupamento por densidade, onde não é necessário informar o nº de grupos

## Aplicação
- Detecção de fraudes, detecção de *outliers* etc.

## Implementação
Dados:
- a) um conjunto de dados X;
- b) o raio de uma vizinhança eps e
- c) o número mínimo de pontos minPts:

1. Para cada ponto do dataset X, encontre os pontos que estão dentro do raio da vizinhança eps;
2. Identifique os corePoints, isto é, os pontos que têm ao menos minPts vizinhos;
3. Encontre todos os Componentes Conectados de cada corePoint. Este agrupamento de pontos conectados por densidade constitui um cluster;
4. Cada borderPoint pertence a um cluster se este cluster é alcançável por densidade, senão o borderPoint é considerado ruído.   

Obs. Dado ponto pode inicialmente ser considerado ruído e depois revisto para pertencer a um cluster, mas uma vez pertencente a um cluster nunca será desassociado deste.

## Fonte de dados
- IRIS Dataset: https://archive.ics.uci.edu/ml/datasets/iris


## Referências
- https://medium.com/analytics-vidhya/dbscan-from-scratch-almost-b02096600c14
- https://towardsdatascience.com/understanding-dbscan-algorithm-and-implementation-from-scratch-c256289479c5
- Material da disciplina MATE33 UFBA
---

