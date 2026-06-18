# TripleTen Sprint 11: Machine Learning para Retenção de Clientes (Previsão de Churn) 🤖🏋️‍♀️

Este repositório contém o projeto final da décima primeira sprint do curso de Análise de Dados da TripleTen. O foco deste projeto foi a aplicação de algoritmos de **Machine Learning** para resolver um problema crítico de negócios: prever e reduzir o cancelamento de matrículas (Churn) em uma rede de academias chamada Model Fitness.

## 📋 Contexto do Negócio
A Model Fitness identificou que a perda de clientes (churn) é um dos maiores desafios para a lucratividade. O objetivo deste projeto foi analisar perfis de clientes, construir um modelo preditivo para identificar a probabilidade de cancelamento no próximo mês e agrupar os clientes em clusters para criar estratégias de retenção direcionadas.

## 🛠️ Tecnologias e Ferramentas
*   **Python 3.x**
*   **Scikit-Learn:** Criação, treinamento e avaliação de modelos de Machine Learning (Regressão Logística, Random Forest e K-Means).
*   **SciPy:** Criação de dendrogramas para clustering hierárquico.
*   **Pandas & NumPy:** Limpeza, pré-processamento e padronização de dados.
*   **Seaborn & Matplotlib:** Visualização de distribuições, matrizes de correlação e perfis de clusters.

## 🚀 Desafios Técnicos Superados
Este projeto marcou a transição da análise descritiva para a análise preditiva:
*   **Pré-processamento para ML:**
    *   Padronização de variáveis contínuas usando `StandardScaler` para garantir que os algoritmos de distância funcionassem corretamente.
    *   Análise de correlação para evitar multicolinearidade (identificando que "mês de contrato" e "meses restantes" eram altamente correlacionados).
*   **Modelagem Preditiva (Classificação):**
    *   Treinamento e comparação de dois algoritmos: **Regressão Logística** e **Random Forest Classifier**.
    *   Avaliação de desempenho usando métricas de negócio: **Acurácia, Precisão e Recall**.
    *   Conclusão de que a Regressão Logística teve um desempenho ligeiramente superior nos dados padronizados.
*   **Clusterização (Aprendizado Não Supervisionado):**
    *   Construção de um dendrograma para estimar o número ideal de clusters (5).
    *   Aplicação do algoritmo **K-Means** para segmentar a base de clientes em grupos com comportamentos distintos.

## 📊 Principais Insights
*   **Previsão de Churn:** Clientes com contratos curtos (1 mês), que não participam de aulas em grupo e que moram longe da academia têm a maior probabilidade de cancelar.
*   **Segmentação:** Foram identificados 5 perfis claros de clientes. O Cluster 0 (clientes fiéis de longo prazo) tem uma taxa de churn de apenas 2.7%, enquanto o Cluster 3 (clientes de curto prazo sem engajamento) tem uma taxa alarmante de 51%.
*   **Estratégia de Negócio:** Recomendações focadas em incentivar planos de longo prazo, promover aulas em grupo nos primeiros meses e focar o marketing em residentes próximos às unidades.

## 📁 Estrutura do Repositório
*   `notebook.ipynb`: O notebook Jupyter contendo a Análise Exploratória (EDA), treinamento dos modelos de classificação e a clusterização.
*   `README.md`: Este arquivo com a apresentação do projeto.

---
*Este projeto faz parte da minha formação como Analista de Dados na TripleTen Brasil.*
