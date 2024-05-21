## **Empregos e salários em Ciência de Dados 🔍**

Esse projeto tem como objetivo realizar uma análise exploratória de um conjunto de dados disponibilizado no kaggle. Quais informações relevantes é possível extrair e como criar visualizações gráficas interessantes?

Link do Dataset: [Jobs and Salaries in Data Science](https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data)

### Introdução e primeiros passos do projeto:

Realizei todo o processo de carregamento, limpeza e preparação dos dados utilizando a biblioteca [Pandas](https://pandas.pydata.org/). Defini tipos de dados adequados para cada coluna, o que permitiu trabalhar eficientemente com dados categóricos.

Para começar entender melhor as informações do conjunto de dados, criei um novo DataFrame contendo a contagem do número de valores com uma nova coluna em porcentagem e as primeiras conclusões que conseguimos identificar:

 A maior parte dos empregos está distribuido nas áreas de **Data Science and Research**, **Data Engineering**, **Machine Learning and AI** e **Data Analysis**. Correspondendo a aproximadamente **85%** do conjunto de dados.

| Categoria                      |   Quantidade |   Porcentagem (%) |
|:-------------------------------|-------------:|------------------:|
| Data Science and Research      |         1655 |          30.9867  |
| Data Engineering               |         1160 |          21.7188  |
| Machine Learning and AI        |          917 |          17.1691  |
| Data Analysis                  |          809 |          15.147   |
| Leadership and Management      |          351 |           6.5718  |
| BI and Visualization           |          188 |           3.51994 |
| Data Architecture and Modeling |          162 |           3.03314 |
| Data Management and Strategy   |           49 |           0.917431|
| Data Quality and Operations    |           45 |           0.842539|
| Cloud and Database             |            5 |           0.093615|

Essa é a proporção da quantidade de vagas pelo nível de experiência exigido:

| Experiência  | Quantidade  | Porcentagem (%) |
|--------------|-------------|-----------------|
| Senior       | 3444        | 64.482307       |
| Mid-level    | 1274        | 23.853211       |
| Entry-level  | 400         | 7.489234        |
| Executive    | 223         | 4.175248        |

Transformando esses resultados em subplots com o [Matplotlib](https://matplotlib.org/):

![subplot1](https://github.com/ryanrodr/eda-jobs-in-data/blob/main/imagens/subplots1.png)

Analisando dessa forma é correto identificar que existe uma predominância por profissionais de um nível mais Sênior. Somando os dois principais níveis de experiências conseguimos observar que aproximadamente **88%** das vagas está destinada aos níveis **Senior** e **Mid-level**.