COVID-19 Brasil Dashboard - Análise e Visualização de Dados
TL;DR
Este projeto constrói um dashboard interativo sobre a evolução da COVID-19 no Brasil, utilizando dados de casos e vacinação. O processamento de dados é feito em Python (Pandas, NumPy) e o dashboard final está no Google Data Studio.

Dashboard Interativo: [Link do Data Studio]

Processamento de Dados: [Link para Kaggle Notebook]

Fontes de Dados:

Casos: Universidade John Hopkins (link)

Vacinação: Universidade de Oxford (link)

Introdução
A COVID-19 é uma infecção respiratória de alta transmissibilidade e potencial gravidade. Ter dados confiáveis e atualizados é essencial para tomada de decisões em saúde pública. Este projeto busca processar, limpar e transformar dados brutos em insights estratégicos, permitindo acompanhamento da pandemia e vacinação no Brasil.

Objetivo
Construir uma base de dados consistente de casos e vacinação no Brasil.

Criar indicadores analíticos: casos diários, médias móveis, tendências, mortalidade.

Gerar um dashboard interativo para visualização e exploração de dados.

Etapas do Projeto
1. Extração
Dados de casos diários da COVID-19 por estado do Brasil, de janeiro a dezembro de 2021.

Dados de vacinação diária por país.

Scripts em Python iteram sobre arquivos diários para construir a base de dados completa.

2. Limpeza e Transformação (Wrangling)
Seleção de colunas relevantes (confirmed, deaths, state, population, date).

Normalização de nomes de estados.

Cálculo de população estimada a partir da taxa de incidência.

Cálculo de novos indicadores:

Casos diários (confirmed_1d)

Média móvel 7 dias (confirmed_moving_avg_7d)

Tendência 14 dias (confirmed_trend)

Mortes diárias e médias móveis (deaths_1d, deaths_moving_avg_7d, deaths_trend)

3. Enriquecimento de Dados
Criação de colunas temporais: month, year.

Conversão de tipos para garantir consistência (Int64, datetime64).

Reorganização das colunas para facilitar análise e visualização.

Tecnologias Utilizadas
Linguagens & Bibliotecas: Python, Pandas, NumPy

Visualização: Google Data Studio

Extração: CSVs públicos da Universidade John Hopkins e Our World in Data

Resultados
Base de dados limpa e padronizada para análise de COVID-19 por estado e por dia.

Indicadores temporais que permitem detectar tendências de crescimento, estabilidade ou queda de casos e mortes.

Dashboard interativo que facilita a exploração de dados para stakeholders, como órgãos de saúde e pesquisadores.

Possíveis Melhorias
Adicionar previsão de casos usando modelos de Machine Learning.

Automatizar a atualização diária do dashboard.

Expandir análise para outros países da América Latina.

Conclusão
Este projeto demonstra a transformação de dados brutos em insights estratégicos, com foco em qualidade, confiabilidade e usabilidade. O dashboard fornece informações acionáveis que podem apoiar decisões de saúde pública e políticas de vacinação.
