# 📊 Pipeline de Vendas com Microsoft Fabric, PySpark e Power BI

Este projeto demonstra a construção de um pipeline de dados moderno voltado para análise de vendas, utilizando a arquitetura Medallion e tecnologias líderes de mercado. O objetivo é estruturar os dados de forma eficiente para análise, visualização e geração de insights.

## 🚀 Tecnologias Utilizadas

- **Microsoft Fabric** (versão de avaliação) — criação do Data Lake e uso de Lakehouse com tabelas Delta.
- **PySpark** — programação de notebooks para ingestão, transformação e modelagem dos dados.
- **Power BI** — construção de modelo semântico e criação de relatório interativo.

## 📌 Etapas do Projeto

1. 🔍 **Levantamento e análise das fontes de dados**
2. 🧩 **Modelagem conceitual**
3. 🔗 **Conexão com banco SQL Server** *(somente leitura)*
4. 🧱 **Camada Landing Zone** — ingestão dos dados brutos
5. 📦 **Camada Bronze** — armazenamento dos dados brutos em formato Delta
6. 🧹 **Camada Silver** — tratamento, limpeza e transformação dos dados
7. 🔁 **Camada Gold** — aplicação de SCD Tipo 2 e estruturação do modelo analítico
8. 🧠 **Criação de Tabelas Delta (Lakehouse)**
9. 🎯 **Modelagem Semântica**
10. 📈 **Importação no Power BI e construção de relatório final**

## 🗂️ Estrutura do Repositório

```bash
📁 notebooks/
   ├── 01_landing_zone.py
   ├── 02_bronze.py
   ├── 03_silver.py
   ├── 04_gold.py
   └── utils.py

📁 modelagem/
   ├── modelo_conceitual.drawio
   └── dicionario_dados.xlsx

📁 relatórios/
   └── pipeline_vendas.pbix

📁 imagens/
   └── estrutura_medallion.png

📊 Relatório Final
O relatório foi desenvolvido no Power BI com base nas tabelas Delta estruturadas em Fabric. Ele apresenta indicadores de performance, análise de vendas por região, produto e tempo, além de segmentações dinâmicas.

📎 Arquivo disponível em: relatórios/pipeline_vendas.pbix

📌 Observações
A conexão com o SQL Server foi realizada com permissão somente leitura, assegurando a integridade da fonte de dados.

O projeto aplica boas práticas de engenharia de dados, como versionamento, uso de Delta Lake e separação por camadas lógicas.

💡 Próximos Passos
Implementar automações com triggers no Fabric

Monitoramento com ferramentas de observabilidade

Otimizações de performance com Z-Ordering e Compactação Delta

👩‍💻 Desenvolvido por
Esmenia
Data Professional | PySpark • Microsoft Fabric • Power BI
LinkedIn (adicione seu link)

README.md
