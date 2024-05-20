### **Empregos e salários em Ciência de Dados 🔍**

Esse projeto tem como objetivo realizar uma análise exploratória de um conjunto de dados disponibilizado no kaggle. Quais informações relevantes é possível extrair e como criar visualizações interessantes com o matplotlib?

Link do Dataset: [Jobs and Salaries in Data Science](https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data)

Realizei todo o processo de carregamento, limpeza e preparação dos dados utilizando o Pandas. Defini tipos de dados adequados para cada coluna, o que permitiu trabalhar eficientemente com dados categóricos.

Para começar entender melhor as informações do conjunto de dados, criei um novo DataFrame contendo a contagem do número de valores com uma nova coluna em porcentagem:


```python
quantidade_categoria = df['job_category'].value_counts()
percentual_categoria = df['job_category'].value_counts(normalize=True) * 100

tabela_categoria = pd.DataFrame({'Quantidade': quantidade_categoria,
                                 'Porcentagem (%)': percentual_categoria})

tabela_categoria = tabela_categoria.reset_index().rename(columns={'job_category': 'Categoria'})
```
As primeiras conclusões que conseguimos identificar é que a maior parte dos empregos está distribuido nas áreas de **Data Science and Research**, **Data Engineering**, **Machine Learning and AI** e **Data Analysis**. Correspondendo a aproximadamente **85%** do conjunto de dados.

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

