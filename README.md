## **Empregos e salários em Ciência de Dados 🔍**

Esse projeto tem como objetivo realizar uma análise exploratória de um conjunto de dados disponibilizado no Kaggle. Quais informações relevantes é possível extrair e como criar visualizações gráficas interessantes?

Link do Dataset: [Jobs and Salaries in Data Science](https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data)

### Introdução

O conjunto de dados foi carregado, limpo e preparado utilizando a biblioteca Pandas. Tipos de dados adequados foram definidos para cada coluna, o que permitiu trabalhar eficientemente com dados categóricos. Para começar a entender melhor as informações do conjunto de dados podemos começar com uma tabela de frequência.

### Tabela de Frequência

| Categoria                         | Frequência | Frequência Relativa (%) | Frequência Acumulada | Frequência Relativa Acumulada (%) |
|-----------------------------------|------------|--------------------------|----------------------|------------------------------------|
| Data Science and Research         | 3014       | 32.218065                | 3014                 | 32.218065                          |
| Data Engineering                  | 2260       | 24.158204                | 5274                 | 56.376269                          |
| Data Analysis                     | 1457       | 15.574559                | 6731                 | 71.950828                          |
| Machine Learning and AI           | 1428       | 15.264564                | 8159                 | 87.215393                          |
| Leadership and Management         | 503        | 5.376804                 | 8662                 | 92.592197                          |
| BI and Visualization              | 313        | 3.345804                 | 8975                 | 95.938001                          |
| Data Architecture and Modeling    | 259        | 2.768573                 | 9234                 | 98.706574                          |
| Data Management and Strategy      | 61         | 0.652058                 | 9295                 | 99.358632                          |
| Data Quality and Operations       | 55         | 0.587921                 | 9350                 | 99.946553                          |
| Cloud and Database                | 5          | 0.053447                 | 9355                 | 100.000000                         |

### Distribuição de Pareto
A maior parte dos empregos está distribuída nas áreas de **Data Science and Research**, **Data Engineering**, **Data Analysis** e **Machine Learning and AI**. Correspondendo a aproximadamente **87%** do conjunto de dados.

![pareto](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/distribuicao_pareto.png)

### Distribuição Temporal
Os dados foram coletados entre 2020 e 2023. 

Visualizando o DataFrame anterior com um contexto temporal, é possível entender melhor o conjunto de dados e tirar algumas conclusões:

- Crescimento significativo nos anos de 2022 e 2023 em quase todas as categorias. Isso indica uma demanda crescente por profissionais de Ciência de Dados.

- Pelo menos seis categorias não existiam em 2020. Isso mostra a evolução e diversificação das funções e especializações das áreas de atuação.

- A alta demanda em Machine Learning and AI, Data Engineering e Data Science and Research pode estar ligada ao crescente avanço em Inteligência Artificial.

| Categoria                       | 2020 | 2021 | 2022 | 2023 | Total |
|---------------------------------|------|------|------|------|-------|
| Data Science and Research       | 29   | 72   | 500  | 2413 | 3014  |
| Data Engineering                | 17   | 45   | 499  | 1699 | 2260  |
| Data Analysis                   | 15   | 28   | 289  | 1125 | 1457  |
| Machine Learning and AI         | 10   | 37   | 186  | 1195 | 1428  |
| Leadership and Management       | 0    | 9    | 80   | 414  | 503   |
| BI and Visualization            | 0    | 0    | 8    | 305  | 313   |
| Data Architecture and Modeling  | 0    | 5    | 46   | 208  | 259   |
| Data Management and Strategy    | 0    | 1    | 12   | 48   | 61    |
| Data Quality and Operations     | 0    | 0    | 12   | 43   | 55    |
| Cloud and Database              | 0    | 0    | 2    | 3    | 5     |

### Distribuição das Categorias pelo Nível de Experiência:

Existem diferentes níveis de experiência para cada área de atuação.

| Experiência    | Quantidade | Porcentagem (%) |
|----------------|------------|-----------------|
| Senior         | 6709       | 71.715660       |
| Mid-level      | 1869       | 19.978621       |
| Entry-level    | 496        | 5.301978        |
| Executive      | 281        | 3.003741        |

Criando uma visualização com subplots da biblioteca matplotlib.

![subplots](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/subplots.png)

Conseguimos concluir que mais da metade do conjunto de dados está destinado a vagas de nível Senior, mas como seria essa distribuição entre as categorias de atuação em Ciência de Dados? Com a biblioteca Seaborn, é possível gerar um heatmap com esses dados, transformando os valores em porcentagens pelo eixo das linhas, o que facilita a visualização da distribuição de vagas pelo seu nível de experiência.

- É evidente a proporção da quantidade de vagas de nível **Senior**.
- **Cloud and Database** tem preferência por profissionais apenas de nível Senior.
- **Data Analysis** e **Data Management and Strategy** tendem a ter mais oportunidades de entrada.

![heatmap1](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/heatmap.png)
