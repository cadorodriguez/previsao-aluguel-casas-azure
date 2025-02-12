Projeto de Previsão de Aluguel de Casas com Azure ML
Este projeto demonstra a criação de um modelo de previsão de aluguel de casas utilizando o Azure Machine Learning, com foco em regressão. O objetivo é prever o preço de aluguel mensal para casas de até 3 quartos, com base em dados demográficos e características das casas.

1. Objetivo
Prever o preço de aluguel mensal para casas de até 3 quartos, utilizando dados demográficos e características das casas.

2. Dados
Fonte de dados: Os dados utilizados neste projeto foram coletados do Kaggle, em um conjunto de dados público sobre aluguel de imóveis na cidade de São Paulo. O conjunto de dados pode ser encontrado em [https://www.kaggle.com/datasets/gabrielabastos/housing-prices-in-sao-paulo](https://www.google.com/search?q=https://www.kaggle.com/datasets/gabrielabastos/housing-prices-in-sao-paulo).
Descrição dos dados: Os dados incluem informações sobre características das casas (ex: tamanho em metros quadrados, número de quartos, número de banheiros, vagas de garagem, se aceita animais, se é mobiliado, valor do condomínio, IPTU) e dados demográficos da região (ex: renda média, população).
Armazenamento dos dados: Os dados foram armazenados no Azure Blob Storage para garantir segurança e escalabilidade.
3. Metodologia
Preparação dos dados:
Os dados foram explorados e limpos utilizando o Azure Databricks.
Foram tratadas informações faltantes, valores discrepantes e erros nos dados.
Os dados foram transformados para melhorar o desempenho do modelo (ex: normalização, padronização).
Criação e treinamento do modelo:
O modelo foi criado e treinado utilizando o Azure Machine Learning Studio.
Foi utilizado um algoritmo de regressão linear.
Os hiperparâmetros do modelo foram ajustados para otimizar seu desempenho.
Avaliação do modelo:
O desempenho do modelo foi avaliado utilizando as métricas de erro quadrático médio (RMSE).
O modelo foi validado em dados não vistos para garantir sua generalização.
4. Resultados
O modelo de regressão linear obteve um erro quadrático médio (RMSE) de R$ 750. Este resultado indica que o modelo é capaz de prever o preço de aluguel de casas com uma precisão de, em média, R$ 750 para mais ou para menos. Em outras palavras, o modelo estima o aluguel com uma margem de erro de R$ 750.

Além da previsão do valor médio do aluguel, a análise exploratória dos dados revelou que o aluguel mais baixo encontrado na amostra foi de R$ 1.500 e o aluguel mais alto foi de R$ 15.000.
