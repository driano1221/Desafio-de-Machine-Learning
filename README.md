<a href="https://colab.research.google.com/github/driano1221/ControleEst/blob/main/Plastic_ML.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

# Combate à Poluição Plástica nos Oceanos e Praias: Um Desafio de Machine Learning

## Alunos:

### Bruno Tanaui Zanocco 85770
### Caio Silva Alves 85350
### Murilo José Cressoni 95267

### Introdução

O dataset intitulado "Concentrations of Plastic Additives in the Ocean" contém informações detalhadas sobre aditivos plásticos presentes em diversos compartimentos ambientais, como plásticos, água, sedimentos e biota. Os dados foram coletados a partir de literatura revisada por pares e incluem estudos que mencionam aditivos químicos como componentes plásticos. Este dataset é valioso para pesquisas sobre poluição plástica nos oceanos e os efeitos desses aditivos químicos no meio ambiente marinho. A atualização mais recente dos dados foi em 11 de abril de 2024.

Referência: https://catalog.data.gov/dataset/dataset-of-published-concentrations-of-plastic-additives-in-the-ocean

### Variáveis do Dataset

A planilha "Compiled Data" deste dataset contém 46 variáveis. Aqui está a explicação de cada uma delas:

1. **Referência**: Referência abreviada do artigo no formato APA.
2. **Título do Artigo**: Título do artigo publicado na revista.
3. **Ano da Referência**: Ano em que o artigo foi publicado.
4. **Compartimento**: Tipo de amostra analisada no artigo (plástico, água, sedimento ou biota).
5. **Tamanho da Amostra**: Número de amostras analisadas.
6. **ID da Amostra**: Número de identificação individual da amostra.
7. **Método de Coleta de Campo da Amostra**: Como a amostra foi inicialmente coletada/obtida.
8. **Ano de Coleta da Amostra**: Data(s) em que as amostras foram coletadas do ambiente.
9. **Local de Coleta da Amostra - Corpo de Água**: Corpo de água de onde as amostras foram coletadas ou corpo de água associado próximo ao local de coleta (N/A = não aplicável).
10. **Local de Coleta da Amostra - Massa de Terra de Referência**: Massa de terra associada (por exemplo, país, cidade, etc.) próxima ao local de coleta das amostras (N/A = não aplicável).
11. **Local de Amostragem - Continente de Referência**: Área geográfica associada à coleta das amostras.
12. **Técnica de Separação da Matriz Original**: Método utilizado para separar o plástico da matriz original (por exemplo, sedimento, biota, etc.; N/A = não aplicável).
13. **Identificação do Polímero Realizada?**: Indica se os polímeros plásticos foram identificados (sim ou não).
14. **Método de Identificação do Polímero**: Instrumento ou método laboratorial utilizado para identificar o polímero plástico (N/A = não aplicável).
15. **Composição do Polímero**: Tipo de polímero (por exemplo, polipropileno, polietileno, etc.; N/A = não aplicável).
16. **Categoria de Tamanho do Plástico**: Tamanho ou intervalo de tamanho das partículas de plástico analisadas.
17. **Profundidade Abaixo da Superfície da Água Amostrada**: Ponto na coluna d'água em que a água foi coletada/profundidade abaixo da superfície da água em que o sedimento foi coletado.
18. **Unidades da Profundidade Abaixo da Superfície da Água Amostrada**: Unidades da profundidade abaixo da superfície da água amostrada (por exemplo, metros, centímetros, pés; N/A = não aplicável).
19. **Categoria da Distância da Amostra de Água em Relação à Costa**: Área onde a amostra de água foi coletada para avaliar a distância da linha costeira mais próxima (por exemplo, marina, baía, pelágico).
20. **Volume de Água por Amostra (L)**: Quantidade de água coletada para cada amostra em litros.
21. **Tipo de Sedimento**: Área de onde o sedimento foi coletado (por exemplo, estuarino, praia, marinho).
22. **Profundidade de Amostragem Abaixo da Superfície do Sedimento**: Profundidade abaixo da superfície do sedimento amostrada ou intervalo de profundidade do sedimento amostrado.
23. **Unidades da Profundidade de Amostragem Abaixo da Superfície do Sedimento**: Unidades da profundidade de amostragem abaixo da superfície do sedimento (por exemplo, metros, centímetros, pés; N/A = não aplicável).
24. **Nome Científico**: Nomenclatura binomial (gênero e espécie) da biota amostrada.
25. **Nome Comum**: Nome coloquial da espécie conhecido pelo público em geral.
26. **Táxon**: Grupo biológico de espécies amostradas.
27. **Tipo de Amostragem de Biota**: Método pelo qual o tecido da biota foi separado e preparado para análise.
28. **Tecido da Biota**: Parte da biota amostrada e analisada para aditivos plásticos.
29. **Produto Químico de Extração**: Produto químico utilizado para extrair aditivos plásticos das amostras.
30. **Método de Extração**: Método laboratorial utilizado para facilitar a extração de aditivos plásticos das amostras.
31. **Notas sobre o Método de Extração**: Informações adicionais sobre produtos químicos/métodos de extração.
32. **Método Analítico Geral**: Instrumento utilizado para detectar, identificar e quantificar aditivos plásticos.
33. **Método Analítico Específico**: Propriedades específicas (por exemplo, modo) do instrumento analítico.
34. **Notas sobre o Método Analítico**: Informações adicionais sobre métodos analíticos.
35. **Função Primária do Aditivo**: Uso do composto como aditivo plástico.
36. **Função Secundária do Aditivo**: Se houver múltiplos usos para este composto, o uso secundário foi registrado aqui.
37. **Classe Química**: Tipo específico de composto dentro da função primária e/ou secundária.
38. **Nome Completo do Composto**: Nome químico do aditivo plástico conforme relatado no artigo.
39. **Abreviação do Composto**: Abreviação comum dos compostos (se aplicável).
40. **Número CAS**: Número de identificação único do registro CAS do composto.
41. **Estatística Resumida**: Valor estatístico específico reportado (por exemplo, média, desvio padrão).
42. **Concentração**: Quantidade do composto medida na amostra.
43. **Unidades de Concentração**: Unidade de concentração específica reportada para o composto.
44. **% Detectado**: Percentual do composto detectado na amostra.
45. **Notas Gerais**: Informações adicionais sobre as publicações incorporadas neste banco de dados consideradas relevantes pelos autores.
46. **Notas de QA/QC**: Informações adicionais sobre o controle de qualidade e garantia de qualidade dos métodos da publicação.



Para reduzir o número de variáveis do dataset e focar nas informações mais relevantes, especialmente relacionadas ao plástico, foram selecionadas as 10 variáveis que são consideradas mais importantes para o trabalho. Aqui estão elas:

1. **Reference**: Para identificar a fonte dos dados.
2. **Reference Year**: Para saber o ano em que os dados foram publicados.
3. **Compartment**: Para entender o tipo de amostra analisada (plástico, água, sedimento ou biota).
4. **Polymer ID Performed?**: Para saber se os polímeros plásticos foram identificados.
5. **Polymer Composition**: Para obter informações sobre o tipo de polímero (por exemplo, polipropileno, polietileno, etc.).
6. **Plastic Size Category**: Para conhecer a categoria de tamanho das partículas de plástico analisadas.
7. **Sample Collection Location - Water Body**: Para identificar o corpo de água de onde as amostras foram coletadas.
8. **Concentration**: Para medir a quantidade de composto na amostra.
9. **Concentration Units**: Para saber as unidades da concentração reportada.
10. **% Detected**: Para entender o percentual de detecção do composto na amostra.

Essas variáveis proporcionarão uma visão abrangente e focada no plástico, permitindo uma análise mais direcionada e eficiente, iremos trabalhar em cima delas para criar um modelo final de **Machine Learning**

Por fim, escolhemos essas 4 variáveis com as seguintes informações:

1. **Reference Year**: Para saber o ano em que os dados foram publicados.
2. **Compartment**: Para entender o tipo de amostra analisada (plástico, água, sedimento ou biota).
3. **Concentration**: Para medir a quantidade de composto na amostra.
4. **% Detected**: Para entender o percentual de detecção do composto na amostra.


Vamos agora começar a chegar possíveis valores sem sentido, outliers ou fora do padrão:


Os box plots para as variáveis numéricas "Concentration" e "% Detected" indicam a presença de possíveis outliers. Vamos analisar essas variáveis mais detalhadamente para identificar e lidar com esses valores, vale destacar que estamos usando a conversão logaritma para uma melhor visualização

### Análise de Outliers

1. **Concentration**: A distribuição da concentração de compostos pode ter valores extremamente altos que são considerados outliers.
2. **% Detected**: A porcentagem detectada também apresenta alguns valores que se destacam como possíveis outliers.

#### Próximos Passos

- Calcular os limites para outliers usando o método do IQR (Interquartile Range).
- Identificar e decidir como lidar com os outliers (remoção, transformação, etc.).

Vamos começar calculando os limites do IQR para identificar os outliers.

A análise revelou que aproximadamente 0,11% dos dados são outliers, com valores extremamente altos em "Concentration". Alguns exemplos de outliers incluem concentrações de 518,000, 214,000, e até 37,000,000.

### Abordagem para Lidar com Outliers

1. **Remoção de Outliers**: Remover os outliers pode ser uma abordagem se esses valores forem considerados ruído.
2. **Transformação de Dados**: Aplicar uma transformação, como logaritmo, pode ajudar a reduzir a influência dos outliers.
3. **Manter os Outliers**: Dependendo da natureza do estudo, pode ser necessário manter esses valores para análise mais detalhada.
### Sumário Estatístico das Variáveis

|                   | Reference Year | Compartment | Concentration        | % Detected        |
|-------------------|----------------|-------------|----------------------|-------------------|
| **Count**         | 11624.0        | 11624       | 11624                | 11624             |
| **Unique**        | 33.0           | 4           | -                    | -                 |
| **Top**           | 2021.0         | Plastic     | -                    | -                 |
| **Freq**          | 2725.0         | 4465        | -                    | -                 |
| **Mean**          | -              | -           | 65492.18             | 63.27             |
| **Std**           | -              | -           | 4465940.00           | 88.81             |
| **Min**           | -              | -           | 0.00                 | 0.00              |
| **25%**           | -              | -           | 1.70                 | 60.00             |
| **50%**           | -              | -           | 32.60                | 63.27             |
| **75%**           | -              | -           | 65492.18             | 100.00            |
| **Max**           | -              | -           | 480000000.00         | 8871.00           |


### Box Plots com Transformação Logarítmica após Remoção dos Outliers

Os gráficos acima mostram a distribuição das variáveis "Concentration" e "% Detected" após a aplicação da transformação logarítmica e a remoção dos outliers.


### Sumário Estatístico das Variáveis após Remoção dos Outliers

|                   | Reference Year | Compartment | Concentration        | % Detected        |
|-------------------|----------------|-------------|----------------------|-------------------|
| **Count**         | 11611.0        | 11611       | 11611                | 11611             |
| **Unique**        | 33.0           | 4           | -                    | -                 |
| **Top**           | 2021.0         | Plastic     | -                    | -                 |
| **Freq**          | 2723.0         | 4455        | -                    | -                 |
| **Mean**          | -              | -           | 19556.54             | 62.50             |
| **Std**           | -              | -           | 29751.91             | 34.82             |
| **Min**           | -              | -           | 0.00                 | 0.00              |
| **25%**           | -              | -           | 1.70                 | 60.00             |
| **50%**           | -              | -           | 32.30                | 63.27             |
| **75%**           | -              | -           | 65492.18             | 100.00            |
| **Max**           | -              | -           | 84595.90             | 100.00            |

Os outliers foram removidos e os dados foram transformados logaritmicamente, resultando em uma distribuição mais uniforme.


## Estatística Descritiva


### Visualizações e Análises

### Matriz de Correlação das Variáveis Transformadas Logaritmicamente

A matriz de correlação acima exibe as correlações entre as variáveis do dataset após a transformação logarítmica e a conversão das colunas categóricas para numéricas.

#### Pairplot das Variáveis Transformadas Logaritmicamente
O gráfico de pares mostra a relação entre as variáveis "Reference Year", "Compartment", "Concentration" e "% Detected" após a transformação logarítmica e remoção de outliers.



### Sumário Estatístico das Variáveis após Remoção dos Outliers e Transformação Logarítmica

|                   | Reference Year | Compartment | Concentration        | % Detected        |
|-------------------|----------------|-------------|----------------------|-------------------|
| **Count**         | 11611.0        | 11611       | 11611                | 11611             |
| **Unique**        | 33.0           | 4           | -                    | -                 |
| **Top**           | 2021.0         | Plastic     | -                    | -                 |
| **Freq**          | 2723.0         | 4455        | -                    | -                 |
| **Mean**          | -              | -           | 5.02                 | 3.58              |
| **Std**           | -              | -           | 4.38                 | 1.59              |
| **Min**           | -              | -           | 0.00                 | 0.00              |
| **25%**           | -              | -           | 0.99                 | 4.11              |
| **50%**           | -              | -           | 3.51                 | 4.16              |
| **75%**           | -              | -           | 11.09                | 4.62              |
| **Max**           | -              | -           | 11.35                | 4.62              |

### Análise


1. **Análise da Matriz de Correlação**

  - **Concentration e % Detected**: Existe uma correlação positiva entre a concentração dos compostos e a porcentagem detectada, indicando que essas duas variáveis tendem a aumentar juntas.
  - **Reference Year**: Não há correlações fortes entre o ano de referência e as outras variáveis, sugerindo que a concentração e a detecção dos compostos não variam significativamente ao longo dos anos.
  - **Compartment**: A variável "Compartment" apresenta correlações mais fracas com as variáveis numéricas, indicando que a distribuição de concentração e detecção pode variar entre diferentes compartimentos.


2. **Distribuição por "Compartment"**:
   - O box plot de "Concentration" através das categorias de "Compartment" mostra que há variação significativa nas concentrações entre diferentes compartimentos, com plásticos e biota apresentando diferentes níveis de concentração.

3. **Dados Estatísticos**:
   - A média logarítmica de "Concentration" e "% Detected" ajuda a normalizar os dados, mostrando uma distribuição mais uniforme e facilitando a análise de tendências.


##  feature engineering

Para melhorar o nosso dataset, podemos considerar a criação de novas variáveis com base nas existentes, que podem fornecer informações adicionais ou insights que não são imediatamente aparentes nas variáveis originais. Aqui estão algumas sugestões de feature engineering que podemos realizar:

1. **Categoria de Concentração**: Podemos criar uma variável categórica baseada na "Concentration" para agrupar os dados em diferentes faixas de concentração (baixa, média, alta).

2. **Detecção Binária**: Podemos criar uma variável binária para indicar se um composto foi detectado ou não, com base na variável "% Detected".

3. **Ano Agrupado**: Agrupar os anos de referência em períodos (por exemplo, década) pode ajudar a analisar tendências temporais.

### Implementação das Novas Variáveis

Vamos criar essas novas variáveis e verificar como elas melhoram o nosso dataset.

#### 1. Categoria de Concentração
- Baixa: Concentração < 25%
- Média: Concentração entre 25% e 75%
- Alta: Concentração > 75%

#### 2. Detecção Binária
- Detectado: % Detected > 0
- Não Detectado: % Detected == 0

#### 3. Ano Agrupado
- Agrupar os anos em períodos de 5 anos.




### Novas Variáveis Criadas

1. **Concentration Category**:
   - **Low**: Concentração < Percentil 25
   - **Medium**: Concentração entre Percentil 25 e 75
   - **High**: Concentração > Percentil 75

2. **Detection Binary**:
   - **1**: Detecção ( % Detected > 0 )
   - **0**: Não Detecção ( % Detected == 0 )

3. **Year Group**:
   - Agrupamento de anos em períodos de 5 anos (1970-1974, 1975-1979, ..., 2015-2019, 2020-2024)

Essas novas variáveis fornecem uma categorização mais granular e podem ajudar a identificar padrões ou tendências ocultas nos dados.

### Análise das Novas Variáveis

#### Distribuição das Categorias de Concentração
Será criados gráficos para visualizar a distribuição dessas novas variáveis e como elas interagem com outras variáveis do dataset.





### Análise das Novas Variáveis

#### Distribuição das Categorias de Concentração
O gráfico de barras mostra que há uma distribuição razoavelmente equilibrada entre as categorias de concentração "Low", "Medium" e "High", com "Medium" sendo ligeiramente mais frequente.

#### Distribuição da Detecção Binária
A maioria das amostras possui detecção, como indicado pela predominância da categoria "1" (Detectado).

#### Distribuição dos Grupos de Anos
A distribuição dos grupos de anos mostra uma maior quantidade de dados coletados nos anos mais recentes, especialmente no período de 2015-2019.

#### Box Plot de Concentração por Categoria de Concentração
O box plot confirma a categorização de concentração, mostrando claramente as faixas de concentração "Low", "Medium" e "High".

#### Box Plot de Concentração por Grupos de Anos
O box plot mostra a variação da concentração ao longo dos diferentes grupos de anos, indicando que não há uma tendência clara de aumento ou diminuição ao longo do tempo.


As novas variáveis adicionadas permitem uma análise mais detalhada e granular dos dados, facilitando a identificação de padrões e tendências que não eram evidentes nas variáveis originais. Essas visualizações fornecem uma base sólida para futuras análises e insights sobre a concentração de compostos plásticos e sua detecção em diferentes contextos e períodos.



### Verificação de Multicolinearidade

A Tabela de Fatores de Inflação da Variância (VIF) é apresentada abaixo:

| Variable         | VIF       |
|------------------|-----------|
| const            | 28.662874 |
| Reference Year   | 1.015784  |
| Concentration    | 1.336250  |
| % Detected       | 1.340471  |



- **Reference Year, Concentration, e % Detected** têm VIFs muito baixos (próximos de 1), indicando que não há problemas significativos de multicolinearidade entre essas variáveis.
- **Const** (constante adicionada) tem um VIF alto, mas isso é esperado e não é uma preocupação.



As variáveis no dataset não apresentam multicolinearidade significativa, o que é positivo para a criação de modelos futuros. Você pode prosseguir com a criação do modelo sem a preocupação de multicolinearidade entre essas variáveis.



# Aplicação Machine Learning

Para aplicar técnicas de Machine Learning ao nosso dataset, considerarei duas abordagens diferentes: Regressão e Classificação. Vamos definir os problemas que vamos abordar:

1. **Regressão**: Prever a concentração de compostos plásticos ("Concentration") com base nas outras variáveis do dataset.
2. **Classificação**: Classificar se a concentração é "Alta" ou não com base nas outras variáveis do dataset.

### Passos para a Análise

1. **Preparação dos Dados**:
   - Separar os dados em conjuntos de treino e teste.
   - Normalizar os dados.
   - Converter variáveis categóricas em variáveis dummy (one-hot encoding).

2. **Aplicação das Técnicas**:
   - Regressão Linear.
   - Regressão com Árvores de Decisão.
   - Classificação com Regressão Logística.
   - Classificação com Random Forest.

3. **Avaliação das Métricas**:
   - Para Regressão: Mean Absolute Error (MAE), Mean Squared Error (MSE), R².
   - Para Classificação: Acurácia, Precision, Recall, F1-Score, AUC-ROC.





### Análise das Técnicas de Machine Learning

#### Regressão

1. **Regressão Linear**:
   - **MAE**: 2.95
   - **MSE**: 13.64
   - **R²**: 0.26

2. **Regressão com Árvores de Decisão**:
   - **MAE**: 1.89
   - **MSE**: 7.96
   - **R²**: 0.57

#### Classificação

1. **Regressão Logística**:
   - **Acurácia**: 0.84
   - **Precisão**: 0.87
   - **Recall**: 0.48
   - **F1-Score**: 0.62
   - **AUC-ROC**: 0.73

2. **Random Forest**:
   - **Acurácia**: 0.90
   - **Precisão**: 0.81
   - **Recall**: 0.83
   - **F1-Score**: 0.82
   - **AUC-ROC**: 0.88

**Abaixo conseguimos visualizar a comparação dos modelos**

### Conclusão do Trabalho

Neste trabalho, realizamos uma série de análises e transformações de dados, culminando na aplicação de técnicas de Machine Learning para prever e classificar a concentração de compostos plásticos no oceano. Aqui estão os passos detalhados e as conclusões de cada etapa do nosso trabalho:

#### Preparação dos Dados

1. **Limpeza e Transformação dos Dados**:
   - Remoção de outliers e transformação logarítmica dos dados para normalizar a distribuição.
   - Criação de novas variáveis para enriquecer o dataset: "Concentration Category", "Detection Binary", e "Year Group".

2. **Verificação de Multicolinearidade**:
   - Utilizamos o Variance Inflation Factor (VIF) para garantir que não havia multicolinearidade significativa entre as variáveis, confirmando que as variáveis selecionadas eram adequadas para modelagem.

#### Aplicação de Técnicas de Machine Learning

1. **Regressão**:
   - **Regressão Linear** e **Árvore de Decisão** foram usadas para prever a concentração dos compostos plásticos.
   - **Árvore de Decisão** teve um desempenho significativamente melhor, com menor MAE e MSE, e um R² maior, indicando maior precisão na previsão.

2. **Classificação**:
   - **Regressão Logística** e **Random Forest** foram usadas para classificar se a concentração de compostos plásticos era alta ou não.
   - **Random Forest** apresentou melhor desempenho em todas as métricas de classificação (Acurácia, Precisão, Recall, F1-Score, e AUC-ROC), mostrando-se superior na tarefa de classificação.

#### Resultados

##### Métricas de Regressão

| Model              | MAE   | MSE   | R2    |
|--------------------|-------|-------|-------|
| Linear Regression  | 2.95  | 13.64 | 0.26  |
| Decision Tree      | 1.89  | 7.96  | 0.57  |

A Árvore de Decisão superou a Regressão Linear em todas as métricas, mostrando-se mais eficaz para prever a concentração dos compostos plásticos.

##### Métricas de Classificação

| Model              | Accuracy | Precision | Recall | F1-Score | ROC AUC |
|--------------------|----------|-----------|--------|----------|---------|
| Logistic Regression| 0.84     | 0.87      | 0.48   | 0.62     | 0.73    |
| Random Forest      | 0.90     | 0.81      | 0.83   | 0.82     | 0.88    |

O modelo Random Forest apresentou melhor desempenho do que a Regressão Logística, especialmente em termos de Recall e AUC-ROC, sendo o modelo preferido para a tarefa de classificação.

### Conclusão Final

A análise revelou que, para a previsão de concentração dos compostos plásticos, a Árvore de Decisão é a melhor escolha devido à sua maior precisão. Para a tarefa de classificação, o modelo Random Forest mostrou-se superior, fornecendo alta acurácia e precisão. Estes resultados indicam que técnicas de Machine Learning podem ser eficazmente aplicadas para analisar a poluição plástica no oceano, auxiliando em estudos ambientais e na formulação de políticas de mitigação.



Este trabalho demonstra a eficácia do uso de Machine Learning para entender e prever a poluição plástica, fornecendo uma base sólida para análises futuras e ações mitigadoras.
