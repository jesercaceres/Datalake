 <h1 align ="center">Geração de Dados e Análise através de Data Lake</h1>

<p align="center">
  <img src="https://i.imgur.com/z61i01Z.jpeg" alt="DataLake image">
</p>

<p align="justify">
Este repositório contém um projeto de criação de um ambiente de Data Lake, onde são gerados dados simulados, armazenados em arquivos CSV e posteriormente integrados e analisados utilizando um banco de dados SQLite.

O projeto é dividido em três partes:

1. **Geração de Dados:** Nesta etapa, dados simulados são gerados para representar vendas de produtos. São criados múltiplos arquivos CSV, cada um contendo informações sobre vendas de produtos, como `quantidade`, `valor` e `categoria`.

2. **Armazenamento dos Dados:** Os dados gerados na etapa anterior são armazenados em um banco de dados `SQLite`. Cada arquivo CSV é lido em um DataFrame e posteriormente escrito em uma tabela correspondente no banco de dados.

3. **Análise Exploratória:** Por fim, é realizada uma análise exploratória dos dados armazenados no banco de dados SQLite. São gerados gráficos e estatísticas descritivas para entender melhor os padrões e tendências nos dados de vendas.

Resumidamente, as três partes visam gerar dados simulados, armazená-los em um banco de dados SQLite e realizar análises exploratórias sobre esses dados. Abaixo estão detalhadas as etapas de cada parte do projeto, juntamente com os resultados obtidos.

## Parte 1: Geração de Dados

![Print Google Colab](https://github.com/jesercaceres/Datalake/assets/97481583/3942e8b4-e0f8-475b-b51a-ec5900a6e850)


Nesta parte, dados simulados foram gerados para simular vendas de produtos. Foram criados `10 arquivos CSV`, cada um contendo 1000 linhas de dados. Os dados incluem três colunas: `coluna1`, `coluna2` e `coluna3`. A `coluna1` contém números inteiros aleatórios entre 0 e 100, a `coluna2` contém números aleatórios seguindo uma distribuição normal e a `coluna3` contém valores aleatórios escolhidos entre 'A', 'B' e 'C'. Os dados foram armazenados na pasta 'data_lake'.

## Parte 2: Armazenamento dos Dados no Banco de Dados SQLite

![Print Google Colab](https://i.imgur.com/PGEX6HG.png)

Na segunda parte do projeto, os dados gerados na Parte 1 foram armazenados em um banco de dados SQLite. Cada arquivo CSV foi lido em um DataFrame e em seguida escrito em uma tabela correspondente no banco de dados. Caso a tabela já existisse, os dados foram substituídos. O banco de dados foi criado na pasta `'data_lake.db'`.

## Parte 3: Análise Exploratória dos Dados

![Print Google Colab](https://i.imgur.com/dv8y40A.png)

Na última parte do projeto, foi realizada uma análise exploratória dos dados armazenados no banco de dados SQLite. Um DataFrame foi criado a partir dos dados da tabela 'dados_1' e foram realizadas as seguintes análises:

1. **Impressão** das primeiras linhas do DataFrame.
2. **Impressão de informações sobre o DataFrame** (tipo de dado, número de entradas não nulas).
3. **Impressão de um resumo estatístico do DataFrame** (média, desvio padrão, mínimo, máximo, quartis).
4. **Plotagem de um gráfico de dispersão** entre as colunas 'coluna1' e 'coluna2'.
5.**Plotagem de um histograma** da coluna 'coluna1'.
6. **Plotagem de um boxplot** da coluna 'coluna1' em relação à coluna 'coluna3'.

## Resultados

Os resultados das análises realizadas estão disponíveis no arquivo [DataLake](https://github.com/jesercaceres/Datalake/blob/main/datalake.ipynb). 

## Acesso ao Google Colab

O código utilizado para este projeto está disponível em meu [Google Colab](https://colab.research.google.com/drive/10_GeIfdEeq-RMBtkfJYrbvMv7ipIp_J9?usp=sharing). 

Você pode acessar e executar diretamente em seu navegador.

</p>
