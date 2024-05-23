## **Empregos e salários em Ciência de Dados 🔍**

Esse projeto tem como objetivo realizar uma análise exploratória de um conjunto de dados disponibilizado no Kaggle. Quais informações relevantes é possível extrair e como criar visualizações gráficas interessantes?

Link do Dataset: [Jobs and Salaries in Data Science](https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data)

### Introdução e primeiros passos do projeto:

Realizei todo o processo de carregamento, limpeza e preparação dos dados utilizando a biblioteca Pandas. Defini tipos de dados adequados para cada coluna, o que permitiu trabalhar eficientemente com dados categóricos.

Para começar a entender melhor as informações do conjunto de dados, criei um novo DataFrame contendo a contagem do número de valores com uma nova coluna em porcentagem e as primeiras conclusões que conseguimos identificar:

A maior parte dos empregos está distribuída nas áreas de **Data Science and Research**, **Data Engineering**, **Machine Learning and AI** e **Data Analysis**. Correspondendo a aproximadamente **85%** do conjunto de dados.

| **Categoria**                      |   **Quantidade** |   **Porcentagem (%)** |
|:-----------------------------------|-----------------:|----------------------:|
| Data Science and Research          |              1655|                30.9867|
| Data Engineering                   |              1160|                21.7188|
| Machine Learning and AI            |               917|                17.1691|
| Data Analysis                      |               809|                15.147 |
| Leadership and Management          |               351|                 6.5718|
| BI and Visualization               |               188|                 3.51994|
| Data Architecture and Modeling     |               162|                 3.03314|
| Data Management and Strategy       |                49|                 0.917431|
| Data Quality and Operations        |                45|                 0.842539|
| Cloud and Database                 |                 5|                 0.093615|

### Distribuição Temporal das Categorias:

Os dados foram coletados entre 2020 e 2023. 

Visualizando o DataFrame anterior com um contexto temporal, é possível entender melhor o conjunto de dados e tirar algumas conclusões:

- Crescimento significativo nos anos de 2022 e 2023 em quase todas as categorias. Isso indica uma demanda crescente por profissionais de Ciência de Dados.

- Pelo menos seis categorias não existiam em 2020. Isso mostra a evolução e diversificação das funções e especializações das áreas de atuação.

- A alta demanda em Machine Learning and AI, Data Engineering e Data Science and Research pode estar ligada ao crescente avanço em Inteligência Artificial.


| Ano de Pesquisa                | 2020 | 2021 | 2022 | 2023 |
|--------------------------------|------|------|------|------|
| **Categoria**                  |      |      |      |      |
| BI and Visualization           | 0    | 0    | 8    | 180  |
| Cloud and Database             | 0    | 0    | 2    | 3    |
| Data Analysis                  | 15   | 28   | 185  | 581  |
| Data Architecture and Modeling | 0    | 5    | 30   | 127  |
| Data Engineering               | 17   | 44   | 286  | 813  |
| Data Management and Strategy   | 0    | 1    | 10   | 38   |
| Data Quality and Operations    | 0    | 0    | 8    | 37   |
| Data Science and Research      | 29   | 71   | 338  | 1217 |
| Leadership and Management      | 0    | 9    | 71   | 271  |
| Machine Learning and AI        | 10   | 37   | 157  | 713  |

### Distribuição das Categorias pelo Nível de Experiência:

Cada categoria de atuação em Ciência de Dados exige um nível de experiência diferente e isso pode ser visualizado de forma prática com um mapa de calor do Seaborn. Transformei a visualização em percentual de modo que possa visualização a distribuição de cada categoria e suas respectivas vagas pelo nível de experiência.

![heatmap](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/heatmap.png)