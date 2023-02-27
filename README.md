# ETL_PowerBI_Python
Exercício do curso de Data Engineer - Azure da Gama Academy, com o objetivo de importar dados no formato CSV para o Power Bi, utilizando um script Python, realizando a transformação dos dados.

# Executar o código no Script Python do Power BI
import pandas as pd
import matplotlib as plt

df = pd.read_csv('dados.csv')

df['UF'] = df['UF'].replace(11, 'Rondônia')
df['UF'] = df['UF'].replace(12, 'Acre')
df['UF'] = df['UF'].replace(13, 'Amazonas')
df['UF'] = df['UF'].replace(14, 'Roraima')
df['UF'] = df['UF'].replace(15, 'Pará')
df['UF'] = df['UF'].replace(16, 'Amapá')
df['UF'] = df['UF'].replace(17, 'Tocantins')
df['UF'] = df['UF'].replace(21, 'Maranhão')
df['UF'] = df['UF'].replace(22, 'Piauí')
df['UF'] = df['UF'].replace(23, 'Ceará')
df['UF'] = df['UF'].replace(24, 'Rio Grande do Norte')
df['UF'] = df['UF'].replace(25, 'Paraíba')
df['UF'] = df['UF'].replace(26, 'Pernambuco')
df['UF'] = df['UF'].replace(27, 'Alagoas')
df['UF'] = df['UF'].replace(28, 'Sergipe')
df['UF'] = df['UF'].replace(29, 'Bahia')
df['UF'] = df['UF'].replace(31, 'Minas Gerais')
df['UF'] = df['UF'].replace(32, 'Espírito Santo')
df['UF'] = df['UF'].replace(33, 'Rio de Janeiro')
df['UF'] = df['UF'].replace(35, 'São Paulo')
df['UF'] = df['UF'].replace(41, 'Paraná')
df['UF'] = df['UF'].replace(42, 'Santa Catarina')
df['UF'] = df['UF'].replace(43, 'Rio Grande do Sul')
df['UF'] = df['UF'].replace(50, 'Mato Grosso do Sul')
df['UF'] = df['UF'].replace(51, 'Mato Grosso')
df['UF'] = df['UF'].replace(52, 'Goiás')
df['UF'] = df['UF'].replace(53, 'Distrito Federal')
df['Sexo'] = df['Sexo'].replace([0, 1],['Masculino', 'Feminino'])
df['Anos de Estudo'] = df['Anos de Estudo'].replace([1, 16, 17],['Sem instrução ou até 1 ano', 'Mais de 15 anos', 'Não determinado'])
df['Cor'] = df['Cor'].replace([0, 2, 4, 6, 8, 9],['Indígena', 'Branca', 'Preta', 'Amarela', 'Parda', 'Sem declaração'])


print(df)

# Print do código inserido no Script Python
![Script1](https://user-images.githubusercontent.com/121309155/221641723-9f5945c6-15f7-407d-8d6f-c7d14811235b.jpg)
