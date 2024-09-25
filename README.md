# grafico.py
import pandas as pd
import matplotlib.pyplot as plt

#para carregar os dados de um arquivo cvs(externo)
#df = pd.read_csv('dados.cvs')
#ou criando um dataframe manual

dados = {'ano':[2018,2019,2020,2021,2022], 'vendas':[200,250,300,280,320]}
df = pd.DataFrame(dados)

#grafico de linha

df.plot(x='ano', y='vendas', kind='line')
plt.title('vendas ao longo dos Anos')
plt.xlabel('ano')
plt.ylabel('vendas')
plt.grid('True')
plt.show()

#grafico barras

df.plot(x='ano', y='vendas', kind='bar', color='orange')
plt.title('vendas ao longo dos Anos')
plt.xlabel('ano')
plt.ylabel('vendas')
plt.grid(axis='y')
plt.show()

#grafico pizza
