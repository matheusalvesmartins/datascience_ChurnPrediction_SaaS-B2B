# datascience_ChurnPrediction_SaaS-B2B
Este projeto realiza uma análise de dados exploratória em um dataset de empresa SaaS B2B contendo informações de MRR, engajamento, NPS, chamados de suporte, entre outras informações; e implementa um método de cálculo de Churn Score e por fim o treinamento de um modelo de machine learning para predizer os clientes que poderão churnar.

# <font color='#843CFF'>INTRODUÇÃO

<font color='#330870'> **O problema de negócio**

<font color='#330870'> Em empresas SaaS B2B, especialmente em plataformas de CRM, o churn de clientes representa um risco significativo tanto para a previsibilidade de receita quanto para a eficiência operacional das equipes de Customer Success. O cancelamento raramente ocorre de forma abrupta; em geral, ele é precedido por sinais comportamentais como redução de uso do sistema, aumento de chamados de suporte, insatisfação expressa em interações com a equipe de CS ou queda em métricas de percepção de valor. No entanto, na ausência de mecanismos estruturados de priorização, esses sinais tendem a ser analisados de forma reativa e subjetiva, dificultando a alocação eficiente do esforço do time de Customer Success nos clientes com maior risco de churn.

<font color='#330870'> **Os dados disponíveis**

<font color='#330870'> Para enfrentar esse problema, este estudo utiliza dados consolidados em um data lake no Google BigQuery, integrando múltiplas fontes operacionais do ecossistema do CRM. Estão disponíveis informações cadastrais dos clientes, dados financeiros (MRR), métricas de engajamento com o produto, registros de tickets de suporte, chamados de produto, histórico de reuniões com Customer Success — incluindo extração de sinais qualitativos a partir de transcrições — e métricas de satisfação do cliente, como NPS. Esses dados são agregados em nível de cliente e organizados de forma temporal, permitindo a análise de tendências e variações comportamentais ao longo do tempo, fundamentais para a construção de indicadores de risco de churn.

# <font color='#843CFF'>OBJETIVO

<font color='#330870'> **Objetivo Geral**

<font color='#330870'> Desenvolver um churn score baseado em dados comportamentais, operacionais e de satisfação do cliente, capaz de identificar e priorizar clientes com maior risco de churn, apoiando a atuação proativa da equipe de Customer Success na retenção de clientes em um contexto SaaS B2B de CRM.

<font color='#330870'> **Objetivo Específico**

* <font color='#330870'>Estruturar uma base analítica integrada, consolidando múltiplas fontes de dados em uma visão única por cliente.

* <font color='#330870'>Definir e calcular métricas de engajamento, suporte e relacionamento com Customer Success, com foco em tendências e variações temporais.

* <font color='#330870'>Construir um churn score explicável, baseado em regras e pesos interpretáveis, adequado para uso operacional.

* <font color='#330870'>Classificar clientes em faixas de risco de churn, viabilizando a priorização de ações preventivas pela equipe de Customer Success.

* <font color='#330870'>Estabelecer uma base metodológica que permita a evolução futura do churn score para modelos preditivos supervisionados.
