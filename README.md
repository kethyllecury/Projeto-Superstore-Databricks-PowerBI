# Projeto Superstore - Databricks + Power BI

Este repositório contém um projeto completo de análise de dados utilizando a base **Superstore**, com processamento e modelagem feitos integralmente no **Databricks** com **PySpark** e **SQL**, e visualização dos dados no **Power BI**.

## Tecnologias Utilizadas

- [Databricks](https://www.databricks.com/)
- [Apache Spark](https://spark.apache.org/)
- [Delta Lake](https://delta.io/)
- [Power BI](https://powerbi.microsoft.com/)

## 🛠️ Pipeline de Dados

### 1. Ingestão
- Carregamento dos arquivos CSV da Superstore no Databricks.
- Armazenamento dos dados brutos em formato Delta Lake.

### 2. Transformações
- Limpeza e enriquecimento dos dados com **PySpark**.
- Criação de colunas derivadas, tratamento de dados ausentes e padronização de formatos.

### 3. Modelagem Dimensional
- Aplicação da técnica de **modelagem estrela (star schema)**.
- Criação das tabelas:
  - **Fato**: `fato_vendas`
  - **Dimensões**: `dim_cliente`, `dim_produto`, `dim_regiao`, `dim_tempo`
- Uso de particionamento, cache e otimizações para performance.

### 4. Exposição dos Dados
- Construção de uma **camada semântica SQL** no Databricks.
- Exportação do dataset final como tabela Delta para ser consumido pelo Power BI.

## 📈 Power BI

O arquivo `.pbix` contém o dashboard interativo com:

- KPIs de vendas, lucro e quantidade.
- Análises por região, categoria, cliente e período.
- Visuais personalizados e medidas DAX para insights estratégicos.
- Integração direta com o Databricks usando o conector nativo.

## 📊 Principais Insights

- Produtos mais lucrativos por categoria e subcategoria.
- Regiões com maior volume de vendas e oportunidades de crescimento.
- Perfil de clientes com maior rentabilidade.
- Análise temporal de desempenho.

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/Projeto-Superstore-Databricks-PowerBI.git
