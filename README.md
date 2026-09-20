# Event Correlation & Root Cause Analysis (RCA)

Mini projeto de Machine Learning para identificação de possíveis causas-raiz
em eventos de ambientes distribuídos.

## Objetivo

Desenvolver um protótipo de Root Cause Analysis (RCA) capaz de analisar
eventos operacionais e sugerir possíveis causas-raiz.

O projeto foi desenvolvido em Python utilizando Google Colab e dados
sintéticos.

## Pipeline

Eventos → Feature Engineering → Random Forest → Predição da Causa-Raiz

## Dados

Foi criado um conjunto de dados sintético simulando incidentes em diferentes
componentes de um ambiente distribuído, como:

- API
- Database
- Network
- Authentication
- Cache
- Payment

Cada incidente possui uma causa-raiz conhecida e uma sequência de eventos
associados.

## Feature Engineering

Foram consideradas características relacionadas a:

- coocorrência de eventos;
- janela temporal entre eventos;
- severidade dos eventos.

## Modelo

Foi utilizado o algoritmo Random Forest para classificação da causa-raiz.

Os dados foram divididos em conjuntos de treinamento (80%) e teste (20%).

## Resultado

O modelo obteve 100% de acurácia no conjunto de teste sintético.

Esse resultado deve ser interpretado considerando que os dados simulados
possuem padrões bem definidos entre as classes. Portanto, não representa
o desempenho esperado em um ambiente real.

## Próximos passos

Como evolução do protótipo, podem ser considerados:

- introdução de ruído e sobreposição entre eventos;
- análise de recorrência;
- dependências entre serviços;
- ranking Top-1 e Top-3 de possíveis causas;
- métodos de inferência causal;
- avaliação utilizando dados reais.

## Tecnologias

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab

## Notebook

O notebook completo está disponível na pasta:

`notebooks/RCA_Event_Correlation.ipynb`
