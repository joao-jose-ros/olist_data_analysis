# 📊 Olist Payments Analysis

## 📌 Sobre o Projeto
Este projeto apresenta uma análise exploratória dos dados de pagamentos do e-commerce **Olist**, utilizando **Python, Pandas e SQL**, com foco em:
- Qualidade dos dados  
- Comportamento de pagamento dos clientes  
- Geração de insights de negócio  

Foram aplicadas etapas de **ETL (Extração, Transformação e Carga)**, limpeza dos dados, análise estatística e geração de recomendações de negócio.

---

## 🎯 Objetivos
- **Compreender** o perfil de pagamentos dos clientes  
- **Identificar** os métodos de pagamento mais utilizados  
- **Analisar** padrões de parcelamento  
- **Detectar** inconsistências e problemas de qualidade dos dados  
- **Gerar** recomendações de negócio baseadas nos resultados  

---

## 🛠️ Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3.11.2-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557C?logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13.x-4C72B0?logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-2.x-D71F00?logo=sqlalchemy&logoColor=white)
![PyMySQL](https://img.shields.io/badge/PyMySQL-1.x-4479A1?logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?logo=mysql&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-1.x-007ACC?logo=visualstudiocode&logoColor=white)

---

## 📂 Dataset
Foram utilizados os seguintes datasets:
- `olist_order_payments_dataset.csv`  
- `olist_orders_dataset.csv`  

As tabelas foram integradas para permitir análises mais completas sobre pagamentos e pedidos da plataforma Olist.

**Principais campos analisados:**

| Coluna               | Descrição                               |
| -------------------- | --------------------------------------- |
| order_id             | Identificador único do pedido           |
| payment_sequential   | Sequência do pagamento dentro do pedido |
| payment_type         | Método de pagamento utilizado           |
| payment_installments | Quantidade de parcelas                  |
| payment_value        | Valor pago                              |

---

## 🔄 Processo ETL

### 1. Extração
- Importação dos datasets CSV utilizando Pandas
- Verificação da estrutura inicial dos dados

### 2. Transformação
- Verificação de tipos de dados e busca por valores ausentes
- Análise e tratamento de registros duplicados
- Análise de valores extremos e criação de métricas descritivas

### 3. Carga
- Integração dos dados em ambiente MySQL utilizando SQLAlchemy
- Criação de consultas SQL para validação e exploração
- Utilização dos dados tratados para análises exploratórias e geração de insights

---

## 📊 Análise Exploratória

### Métodos de Pagamento
- Predominância do **cartão de crédito**
- **Boleto bancário** como segunda opção mais utilizada
- Métodos digitais com participação menor na base histórica

### Parcelamento
- Maioria dos pedidos em **pagamento único**
- Existência de pedidos com elevado número de parcelas
- Casos extremos exigem atenção para avaliação de risco financeiro

### Qualidade dos Dados
- Ausência de valores nulos relevantes
- Registros duplicados identificados e investigados
- Tipos de dados validados para garantir consistência

---

## 💡 Principais Insights
1. O **cartão de crédito** concentra a maior parte das transações
2. Grande parte dos clientes prefere **pagamentos à vista** ou com baixo número de parcelas
3. Existem casos com **parcelamentos muito elevados**, indicando possíveis riscos financeiros

---

## 📈 Recomendações de Negócio

1. **Incentivar pagamentos à vista** — criar campanhas de desconto para reduzir custos operacionais e riscos financeiros
2. **Monitorar parcelamentos elevados** — acompanhar pedidos com muitas parcelas para avaliar inadimplência e perfil de risco
3. **Expandir métodos digitais** — incentivar meios digitais para reduzir custos transacionais e capturar oportunidade de crescimento
4. **Revisar processos de cancelamento** — pedidos cancelados que chegaram a ser entregues indicam falhas de controle que exigem atenção
5. **Otimizar logística em períodos críticos** — novembro (Black Friday) concentra picos de vendas; monitorar entregas acima de 30 dias e criar alertas internos

---

## 🚀 Como Executar o Projeto

Clone o repositório:
```bash
git clone https://github.com/joao-jose-ros/olist_data_analysis.git
```

Instale as dependências:
```bash
pip install -r requirements.txt
```

Abra o notebook:
```bash
jupyter notebook
```

---

## 📁 Estrutura do Projeto

```
olist-payments-analysis/
│
├── data/
│   ├── olist_order_payments_dataset.csv
│   ├── olist_orders_dataset.csv
│   └── olist_analysis_ecommerce.sql
│
├── notebooks/
│   └── olist_payments_analysis.ipynb
│
├── reports/
│   └── figures/
│       ├── page-1.jpg
│       ├── page-2.jpg
│       ├── page-3.jpg
│       ├── page-4.jpg
│       ├── page-5.jpg
│       └── page-6.jpg
│
├── crosstab_analysis_1.sql
├── crosstab_analysis_2.sql
├── olist_data_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## 🔮 Próximos Passos
- Criar visualizações mais avançadas
- Integrar a análise com as tabelas de produtos, itens e clientes
- Construir dashboard em Power BI
- Expandir o projeto para outras tabelas da Olist
- Criar um pipeline ETL automatizado

---

## 👤 Autor
**João José R. O. Silva**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-João%20José-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/joao-jose-ribeiro-oliveira-silva/
