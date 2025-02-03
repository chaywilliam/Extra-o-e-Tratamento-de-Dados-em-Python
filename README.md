# Análise de Dados de Vendas e Segmentação RFM

Este repositório contém um script Python que realiza uma análise de dados de vendas, incluindo limpeza, pré-processamento, visualização e segmentação RFM (Recência, Frequência, Monetário). O código utiliza as bibliotecas Pandas, Plotly e outras ferramentas para fornecer insights valiosos sobre o comportamento dos clientes e as vendas.

## Arquivos

*   `Dados.csv`: Conjunto de dados contendo informações sobre vendas.
*   `analise_vendas.ipynb`: Notebook Jupyter com o código Python comentado.
*   `README.md`: Este arquivo.

## Dependências

Para executar o código, você precisa ter as seguintes bibliotecas instaladas:

*   `pandas`
*   `plotly`

Você pode instalá-las usando o pip:

pip install pandas plotly

Markdown

# Análise de Dados de Vendas e Segmentação RFM

Este repositório contém um script Python que realiza uma análise de dados de vendas, incluindo limpeza, pré-processamento, visualização e segmentação RFM (Recência, Frequência, Monetário). O código utiliza as bibliotecas Pandas, Plotly e outras ferramentas para fornecer insights valiosos sobre o comportamento dos clientes e as vendas.

## Arquivos

*   `Dados.csv`: Conjunto de dados contendo informações sobre vendas.
*   `analise_vendas.ipynb`: Notebook Jupyter com o código Python comentado.
*   `README.md`: Este arquivo.

## Dependências

Para executar o código, você precisa ter as seguintes bibliotecas instaladas:

*   `pandas`
*   `plotly`

Você pode instalá-las usando o pip:

```bash
pip install pandas plotly

#Como usar
## 1.Clone este repositório:
git clone https://[endereço-do-repositório].git

## 2.Abra o notebook Jupyter analise_vendas.ipynb em seu ambiente local.
Certifique-se de que o arquivo Dados.csv esteja no mesmo diretório que o notebook.

## 3.Execute as células do notebook para realizar a análise.

# Descrição do código
O código realiza as seguintes etapas:

## 1.Carregamento e exploração inicial dos dados:
Lê o dataset Dados.csv usando pd.read_csv().
Exibe os primeiros registros usando df.head().
Exibe um resumo estatístico das variáveis numéricas usando df.describe().
Verifica os tipos de dados usando df.dtypes.

## 2.Limpeza e pré-processamento dos dados:
Verifica e remove valores nulos na coluna 'CustomerID'.
Verifica e remove preços e quantidades menores ou iguais a 0.
Verifica e remove registros duplicados.
Ajusta o tipo de 'CustomerID' para inteiro e converte 'InvoiceDate' para datetime.
Remove outliers de quantidade e preço unitário.

## 3.Engenharia de Features:
Cria a coluna 'TotalPrice' (preço total) multiplicando 'Quantity' por 'UnitPrice'.

## 4.Análise de vendas e visualização:
Identifica a última data de compra no dataset.
### Top 10 países com maior valor em vendas:
Agrupa os dados por país e calcula o valor total de vendas.
Cria um gráfico de barras interativo com Plotly para mostrar os 10 países com maior valor de vendas.

###Top 10 produtos mais vendidos:
Agrupa os dados por produto (Description) e calcula a quantidade total vendida.
Cria um gráfico de barras interativo com Plotly para mostrar os 10 produtos mais vendidos.

### Valor de venda total por mês:
Cria uma coluna com o ano e mês da compra.
Agrupa os dados por mês e calcula o valor total de vendas.
Cria um gráfico de linha interativo com Plotly para mostrar a evolução das vendas ao longo do tempo.

### Valor de venda total por mês e por país (Top 10 países):
Filtra os dados para os 10 países com maior valor de vendas.
Agrupa os dados por mês e país, e calcula o valor total de vendas.
Cria um gráfico de linha interativo com Plotly para mostrar a evolução das vendas por país ao longo do tempo.

## 5.Segmentação RFM:
Agrupa os dados por cliente e fatura para obter a data da compra e o preço total por pedido.
Calcula a última data disponível no dataset.
Agrupa os dados por cliente para calcular a Recência (R), Frequência (F) e o valor Monetário (M).
Renomeia as colunas para R, F e M.

# Resultados
O código gera insights valiosos sobre os dados de vendas, incluindo:

Ranking dos países com maior valor de vendas.
Ranking dos produtos mais vendidos.
Evolução das vendas ao longo do tempo (mensal e por país).
Segmentação de clientes por RFM (Recência, Frequência, Monetário).

# Observações
O código foi desenvolvido em Python 3.
O arquivo Dados.csv deve conter as colunas necessárias para a análise (CustomerID, InvoiceNo, InvoiceDate, Quantity, UnitPrice, Country, Description).
A segmentação RFM é uma técnica poderosa para entender o comportamento dos clientes e direcionar estratégias de marketing.

# Contato
Se tiver alguma dúvida ou sugestão, entre em contato:

# Charles William
c_wasouza@outlook.com
