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

| Ano de Pesquisa                   | 2020 | 2021 | 2022 | 2023 | Total |
|-----------------------------------|------|------|------|------|-------|
| Categoria                         |      |      |      |      |       |
| Data Science and Research         | 29   | 71   | 338  | 1217 | 1655  |
| Data Engineering                  | 17   | 44   | 286  | 813  | 1160  |
| Machine Learning and AI           | 10   | 37   | 157  | 713  | 917   |
| Data Analysis                     | 15   | 28   | 185  | 581  | 809   |
| Leadership and Management         | 0    | 9    | 71   | 271  | 351   |
| BI and Visualization              | 0    | 0    | 8    | 180  | 188   |
| Data Architecture and Modeling    | 0    | 5    | 30   | 127  | 162   |
| Data Management and Strategy      | 0    | 1    | 10   | 38   | 49    |
| Data Quality and Operations       | 0    | 0    | 8    | 37   | 45    |
| Cloud and Database                | 0    | 0    | 2    | 3    | 5     |

### Distribuição das Categorias pelo Nível de Experiência:

Existem diferentes níveis de experiência para cada área de atuação.

| Experiência   | Quantidade | Porcentagem (%) |
|---------------|------------|-----------------|
| Senior        | 3444       | 64.482307       |
| Mid-level     | 1274       | 23.853211       |
| Entry-level   | 400        | 7.489234        |
| Executive     | 223        | 4.175248        |

Criando uma visualização com subplots da biblioteca matplotlib.

![subplots](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/subplots.png)

Conseguimos concluir que mais da metade do conjunto de dados está destinado a vagas de nível Senior, mas como seria essa distribuição entre as categorias de atuação em Ciência de Dados? Com a biblioteca Seaborn, é possível gerar um heatmap com esses dados, transformando os valores em porcentagens pelo eixo das linhas, o que facilita a visualização da distribuição de vagas pelo seu nível de experiência.

- É evidente a proporção da quantidade de vagas de nível **Senior**.
- **Cloud and Database** tem preferência por profissionais apenas de nível Senior.
- **Data Analysis** e **Data Management and Strategy** tendem a ter mais oportunidades de entrada.

![heatmap1](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/heatmap.png)
