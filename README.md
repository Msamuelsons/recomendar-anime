# Projeto de Recomendação de Animes usando a Biblioteca Surprise

![Poster animes](https://storage.googleapis.com/kaggle-datasets-images/571/1094/c633ae058ddaa59f43649caac1748cf4/dataset-cover.png)

Este projeto implementa um modelo de recomendação de animes com base nas preferências e histórico de visualização do usuário. A biblioteca Surprise, amplamente utilizada para sistemas de recomendação, é usada aqui, e diversos algoritmos de filtragem colaborativa são implementados para gerar recomendações personalizadas.

## Visão Geral

Este documento descreve a implementação e uso do modelo de recomendação de animes construído com a biblioteca Surprise. O modelo é projetado para sugerir animes com base nas preferências e histórico de visualização do usuário. O Surprise é uma biblioteca Python amplamente utilizada para sistemas de recomendação e tem uma variedade de algoritmos de filtragem colaborativa implementados para gerar recomendações personalizadas.

Para saber mais sobre o Surprise, acesse [Surprise](https://surpriselib.com/).

## Pré-requisitos

- Python
- Jupyter Notebook
- Biblioteca scikit-surprise
- Conjunto de dados de animes
  ou
- [Google Colab](https://colab.research.google.com/).

## Carregamento dos Dados

Os dados de avaliações de animes são carregados a partir de um arquivo CSV, e os dados de labels dos animes também são carregados a partir de um arquivo CSV. Os conjuntos de dados utilizados são do Kaggle.

## Análise Exploratória

Uma análise exploratória dos dados é realizada, incluindo estatísticas descritivas das avaliações, visualização da distribuição das notas e informações sobre a quantidade de animes, usuários e amostras no conjunto de dados.

## Preparando o Dataset

O dataset é preparado especificando o intervalo de valores esperados para as avaliações. Isso é importante para informar ao Surprise qual é o intervalo de classificação dos dados.

## Treinando o Modelo

O modelo de recomendação é treinado com os dados de treinamento usando o algoritmo SVDpp. Também é possível ajustar os parâmetros do modelo para obter melhores resultados.

## Predições

As previsões são feitas com o conjunto de teste e os resultados são exibidos.

## Encontrando Animes Recomendados

O modelo é usado para encontrar os 10 melhores animes recomendados para um usuário específico com base em suas preferências.

## Encontrando Animes Semelhantes

Além das recomendações para usuários, o modelo também encontra animes semelhantes a um anime específico usando o algoritmo KNN.

## Resultado

O resultado do modelo é avaliado usando a métrica RMSE (Root Mean Square Error) para medir o erro médio das previsões em relação aos valores reais.
