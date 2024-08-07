# Resumo do Projeto: Analise e Previsao de Abandono de Colaboradores

O projeto tem como objetivo analisar um conjunto de dados de colaboradores de uma empresa para prever o abandono dos mesmos. Seguindo uma abordagem metódica e estruturada, o projeto é dividido em seis passos principais. Abaixo, descrevemos cada fase do projeto:

* **Passo 1: Análise e Tratamento dos Dados**
* 
*1. Carregamento e Análise Inicial:*
* Utilizamos a biblioteca Pandas para carregar a base de dados HR_Abandono.csv. Realizamos uma inspeção inicial dos dados para identificar características como valores nulos, duplicatas e inconsistências.
*2. Tratamento de Dados:*
* Valores Nulos e Duplicados: Identificamos e tratamos valores nulos e registros duplicados para garantir a integridade dos dados.
* Transformação de Tipos de Dados: Corrigimos o tipo de dados das variáveis para refletir corretamente a natureza dos dados, como conversão de variáveis categóricas para numéricas (one-hot encoding) e ajuste de variáveis numéricas.
* Identificação e Tratamento de Outliers: Utilizamos métodos estatísticos e gráficos para identificar outliers e aplicamos as devidas transformações para minimizar seu impacto.
*3. Análise Estatística Descritiva:*
* Realizamos uma análise detalhada das variáveis, calculando médias, medianas e distribuições para variáveis qualitativas e quantitativas. Essa etapa fornece uma compreensão inicial do comportamento dos dados.

* **Passo 2: Análise Exploratório dos Dados**
*1. Visualização de Dados:*
* Utilizamos as bibliotecas Matplotlib e Seaborn para criar gráficos que exploram a distribuição e as relações entre variáveis. Incluímos histogramas, boxplots e gráficos de dispersão para visualizar dados qualitativos e quantitativos.
*2. Storytelling com Dados:*
* Realizamos uma análise narrativa, respondendo a perguntas como:
**Qual é a relação entre o nível de satisfação e o abandono de colaboradores?
**Como o tempo de empresa e o número de acidentes afetam a decisão de sair da empresa?
*Cada gráfico e visualização foram explicados com inferências sobre os possíveis motivos e padrões observados.

* **Passo 3: Formulação e Teste de Hipóteses
*1. Formulação da Hipótese:*
*Baseados na análise exploratória, formulamos hipóteses para testar se variáveis como satisfação e salário têm impacto significativo na decisão de abandonar a empresa.
*2. Teste Estatístico:*
* Utilizamos testes estatísticos como o teste t para comparar grupos e validar as hipóteses. Os resultados foram interpretados para aceitar ou rejeitar as hipóteses com base no valor-p obtido e no nível de significância definido (α = 0.05).

* **Passo 4: Identificação do Tipo de Problema
*1. Tipo de Problema:*
*O problema foi identificado como um problema supervisionado, uma vez que temos rótulos (variável target) e queremos prever a saída dos colaboradores com base em características fornecidas.
*2. Variável Target:*
* A variável target definida é left (se o colaborador deixou a empresa ou não). As variáveis independentes são as características do colaborador que usamos para prever essa variável target.

* **Passo 5: Construção do Modelo Preditivo
*1. Escolha do Algoritmo:*
* Optamos por utilizar o K-Nearest Neighbors (KNN) para a construção do modelo preditivo, um algoritmo adequado para problemas de classificação baseado na proximidade entre amostras.
*2. Treinamento e Ajuste do Modelo:*
* Dividimos os dados em conjuntos de treino e teste e aplicamos escalonamento para normalizar as características. Treinamos o modelo KNN e ajustamos o hiperparâmetro n_neighbors usando validação cruzada (GridSearchCV) para encontrar o melhor valor.

* **Passo 6: Validação do Modelo
*1. Avaliação do Modelo:*
* Avaliamos o modelo utilizando métricas de desempenho como acurácia, precisão, recall e F1-score. Utilizamos a matriz de confusão para examinar o desempenho detalhado em cada classe.
*2. Validação Cruzada:*
* Realizamos validação cruzada para garantir a robustez do modelo e calcular a precisão média, o que fornece uma estimativa confiável da capacidade do modelo de generalizar para novos dados.
