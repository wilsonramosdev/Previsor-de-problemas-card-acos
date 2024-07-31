# Previsor-de-problemas-card-acos
Inteligência artificial previsora de pacientes com probabilidades a ter problemas cardíacos .

O objetivo do programa é prever a probabilidade de um paciente ter problemas cardíacos com base em variáveis clínicas e demográficas. Para isso, é utilizado um modelo de classificação treinado com dados históricos de pacientes.

Bibliotecas Utilizadas
Scikit-learn (sklearn): Uma biblioteca abrangente de machine learning em Python, que fornece ferramentas para a criação e avaliação de modelos de aprendizado supervisionado e não supervisionado.
XGBoost (xgboost): Uma biblioteca otimizada de boosting de gradiente para Python, que oferece alto desempenho e precisão em problemas de classificação e regressão.
Estrutura do Programa

Coleta e Pré-processamento de Dados:

Carregamento dos Dados: Os dados dos pacientes são carregados de um arquivo CSV ou banco de dados.
Tratamento de Valores Ausentes: Imputação ou exclusão de dados faltantes.
Codificação de Variáveis Categóricas: Conversão de variáveis categóricas em numéricas (por exemplo, usando OneHotEncoder ou LabelEncoder do Scikit-learn).
Normalização/Escalonamento: Ajuste dos dados para uma escala uniforme, utilizando técnicas como MinMaxScaler ou StandardScaler.

Divisão dos Dados:

Separação dos dados em conjuntos de treino e teste, usando uma proporção de 70/30.

Treinamento do Modelo:

Modelos Utilizados: São treinados dois modelos principais:
Random Forest (usando RandomForestClassifier do Scikit-learn): Um conjunto de árvores de decisão treinadas com diferentes subconjuntos de dados.
XGBoost (usando XGBClassifier): Um modelo baseado em boosting de gradiente, que combina várias árvores de decisão fracas para formar um modelo forte.

Avaliação do Modelo:

Métricas: As principais métricas de avaliação incluem acurácia, precisão, recall, F1-score e área sob a curva ROC (AUC-ROC).
Validação Cruzada: Uso de validação cruzada para garantir que o modelo seja generalizável e não esteja superajustado aos dados de treinamento.

Previsão e Interpretação:

O modelo treinado é utilizado para prever a probabilidade de problemas cardíacos em novos pacientes.
As previsões podem ser interpretadas e visualizadas para fornecer insights clínicos.

Implementação:

O modelo pode ser implementado em um ambiente de produção para fornecer previsões em tempo real, auxiliando médicos e profissionais de saúde na tomada de decisões.
