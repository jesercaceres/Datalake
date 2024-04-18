# Projeto de Geração de Dados e Análise

Este projeto consiste em três partes que visam gerar dados simulados, armazená-los em um banco de dados SQLite e realizar análises exploratórias sobre esses dados. Abaixo estão detalhadas as etapas de cada parte do projeto, juntamente com os resultados obtidos.

## Parte 1: Geração de Dados

Nesta parte, dados simulados foram gerados para simular vendas de produtos. Foram criados 10 arquivos CSV, cada um contendo 1000 linhas de dados. Os dados incluem três colunas: `coluna1`, `coluna2` e `coluna3`. A `coluna1` contém números inteiros aleatórios entre 0 e 100, a `coluna2` contém números aleatórios seguindo uma distribuição normal e a `coluna3` contém valores aleatórios escolhidos entre 'A', 'B' e 'C'. Os dados foram armazenados na pasta 'data_lake'.

[Link para o código no Google Colab](link_para_o_colab)

## Parte 2: Armazenamento dos Dados no Banco de Dados SQLite

Na segunda parte do projeto, os dados gerados na Parte 1 foram armazenados em um banco de dados SQLite. Cada arquivo CSV foi lido em um DataFrame e em seguida escrito em uma tabela correspondente no banco de dados. Caso a tabela já existisse, os dados foram substituídos. O banco de dados foi criado na pasta 'data_lake.db'.

[Link para o código no Google Colab](link_para_o_colab)

## Parte 3: Análise Exploratória dos Dados

Na última parte do projeto, foi realizada uma análise exploratória dos dados armazenados no banco de dados SQLite. Um DataFrame foi criado a partir dos dados da tabela 'dados_1' e foram realizadas as seguintes análises:

- Impressão das primeiras linhas do DataFrame.
- Impressão de informações sobre o DataFrame (tipo de dado, número de entradas não nulas).
- Impressão de um resumo estatístico do DataFrame (média, desvio padrão, mínimo, máximo, quartis).
- Plotagem de um gráfico de dispersão entre as colunas 'coluna1' e 'coluna2'.
- Plotagem de um histograma da coluna 'coluna1'.
- Plotagem de um boxplot da coluna 'coluna1' em relação à coluna 'coluna3'.

[Link para o código no Google Colab](link_para_o_colab)

## Resultados

Os resultados das análises realizadas estão disponíveis nos respectivos códigos executados no Google Colab. Os dados gerados e armazenados podem ser encontrados na pasta 'data_lake' e o banco de dados SQLite 'data_lake.db'.
