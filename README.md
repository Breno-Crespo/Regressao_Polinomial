Projeto de Regressão Polinomial
Este projeto utiliza regressão polinomial para prever valores com base em um conjunto de dados. Ele inclui etapas de pré-processamento e validação cruzada (k-fold) para avaliar a performance do modelo, bem como o cálculo de métricas como o RMSE (Root Mean Squared Error) e o R² Score.

Estrutura do Projeto
O projeto está estruturado em torno de um pipeline de pré-processamento e treinamento, com a seguinte ordem:

# Pré-processamento de dados numéricos: 
padronização das variáveis tempo_na_empresa e nivel_na_empresa usando StandardScaler.

# Treinamento do Modelo:
 usando a técnica de Regressão Linear.
# Validação Cruzada (K-Fold): 
o conjunto de dados é dividido em várias partes (folds), e o modelo é treinado/testado em cada parte para obter uma avaliação mais robusta.

# Cálculo de métricas:
 durante cada iteração de validação cruzada, as métricas como RMSE e R² são calculadas para os conjuntos de treino e teste.
Requisitos


# Pipeline de Pré-processamento:

O pipeline padroniza as variáveis numéricas, removendo a média e escalando para unidade de variância.

# Modelo de Regressão:
Após o pré-processamento, o modelo de regressão linear é treinado.

K-Fold Cross Validation:
A validação cruzada divide os dados em diferentes conjuntos de treino e teste (usando kf.split(X)), treinando o modelo em cada conjunto e armazenando as métricas.

#Cálculo de Métricas:

Em cada iteração do K-Fold, o RMSE (Raiz do Erro Quadrático Médio) e o R² Score são calculados tanto para os conjuntos de treino quanto de teste.
As previsões e os resíduos (diferença entre valores observados e preditos) são armazenados.

As seguintes métricas são calculadas durante o treinamento e teste do modelo:

  RMSE (Root Mean Squared Error): Calcula o erro médio das previsões. Um valor menor indica um melhor ajuste.
  R² Score: Representa a proporção de variância explicada pelo modelo. Um valor mais próximo de 1 indica um melhor ajuste.
  Resíduos: Diferença entre os valores reais e os valores preditos pelo modelo.
