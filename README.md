# Classificação de Cogumelos

Machine Learning – Identificação de cogumelos comestíveis e venenosos

Este projeto utiliza o famoso dataset Mushroom Dataset (UCI Machine Learning Repository) para treinar um modelo capaz de prever se um cogumelo é comestível ou venenoso, com base em atributos físicos como formato do chapéu, cor das brânquias, odor, textura, entre outros.

# Objetivo

Construir um modelo supervisionado de classificação usando Decision Tree, incluindo:

Exploração inicial do dataset

Pré-processamento das variáveis categóricas

Treinamento de modelo

Avaliação de desempenho

Extração das features mais importantes

 # Dataset

O conjunto de dados contém atributos como:

```cap-shape```, ```cap-surface```, ```cap-color```

```bruises```, ```odor```, ```gill-size```, ```gill-color```

```stalk-shape```, ```stalk-root```, ```habitat```, etc.

Cada amostra é classificada como:

e — edible (comestível)

p — poisonous (venenoso)

O objetivo é prever essa variável alvo.

# Tecnologias utilizadas

Python

Pandas

Scikit-learn

DecisionTreeClassifier

Jupyter Notebook

# Pipeline do Projeto
1. Carregamento dos Dados

Leitura do dataset e visualização inicial dos atributos.

2. Pré-processamento

Como os atributos são categóricos, foram aplicadas técnicas de:

Label Encoding

Separação entre ```X_train```, ```X_test```, ```y_train```, ```y_test```

3. Treinamento do Modelo

O algoritmo utilizado foi:
```bash
DecisionTreeClassifier(random_state=0)
```
4. Avaliação

Foram avaliadas métricas como:

Acurácia

Importância das features

5. Features Mais Importantes

Uma função retorna as 5 variáveis mais relevantes para a árvore de decisão.

# Resultados

O modelo apresentou alta acurácia (como é comum nesse dataset).

A análise de importância dos atributos mostrou que características como odor, spore-print-color e gill-size são fatores decisivos para identificar cogumelos venenosos.
