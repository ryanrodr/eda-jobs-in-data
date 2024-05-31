## **Empregos e salários em Ciência de Dados 🔍**

Esse projeto tem como objetivo realizar uma análise exploratória de um conjunto de dados disponibilizado no Kaggle. Quais informações relevantes é possível extrair e como criar visualizações gráficas interessantes?

Link do Dataset: [Jobs and Salaries in Data Science](https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data)

### Introdução

O conjunto de dados foi carregado, limpo e preparado utilizando a biblioteca Pandas. Tipos de dados adequados foram definidos para cada coluna, o que permitiu trabalhar eficientemente com dados categóricos. Para começar a entender melhor as informações do conjunto de dados podemos começar com uma tabela de frequência.

### Tabela de Frequência

| Categoria                     | Frequência | Frequência Relativa (%) | Frequência Relativa Acumulada (%) |
|-------------------------------|------------|-------------------------|-----------------------------------|
| Data Science and Research     | 4675       | 32.924854               | 32.924854                         |
| Data Engineering              | 3157       | 22.233960               | 55.158814                         |
| Data Analysis                 | 2204       | 15.522220               | 70.681034                         |
| Machine Learning and AI       | 2148       | 15.127826               | 85.808860                         |
| Leadership and Management     | 791        | 5.570815                | 91.379675                         |
| BI and Visualization          | 600        | 4.225650                | 95.605324                         |
| Data Architecture and Modeling| 419        | 2.950912                | 98.556236                         |
| Data Management and Strategy  | 115        | 0.809916                | 99.366153                         |
| Data Quality and Operations   | 79         | 0.556377                | 99.922530                         |
| Cloud and Database            | 11         | 0.077470                | 100.000000                        |

### Distribuição de Pareto
A maior parte dos empregos está distribuída nas áreas de **Data Science and Research**, **Data Engineering**, **Data Analysis** e **Machine Learning and AI**. Correspondendo a aproximadamente **85%** do conjunto de dados.

![pareto](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/distribuicao_pareto.png)

### Nível de Experiência

Existem diferentes níveis de experiência para cada área de atuação.

| Experiência  | Quantidade | Porcentagem (%) |
|--------------|------------|-----------------|
| Senior       | 9381       | 66.068033       |
| Mid-level    | 3339       | 23.515741       |
| Entry-level  | 1063       | 7.486443        |
| Executive    | 416        | 2.929784        |

Conseguimos concluir que mais da metade do conjunto de dados está destinado a vagas de nível Senior, mas como seria essa distribuição entre as categorias de atuação em Ciência de Dados? Com a biblioteca Seaborn, é possível gerar um heatmap com esses dados, transformando os valores em porcentagens pelo eixo das linhas, o que facilita a visualização da distribuição de vagas pelo seu nível de experiência.

### Nível de Experiência com HeatMap
![heatmap](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/heatmap.png)

- É evidente a proporção da quantidade de vagas de nível **Senior**.
- **Cloud and Database** tem preferência por profissionais apenas de nível Senior.
- **Data Analysis** e **Data Management and Strategy** tendem a ter mais oportunidades de entrada.
