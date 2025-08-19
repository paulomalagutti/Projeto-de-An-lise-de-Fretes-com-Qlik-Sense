# Projeto de Análise de Fretes com Qlik Sense

## 1. Visão Geral do Projeto

Este projeto consiste em um dashboard desenvolvido em Qlik Sense para a análise detalhada da performance logística da empresa, com foco principal nas operações de frete. O painel centraliza indicadores-chave para monitorar custos, eficiência e utilização da frota, fornecendo insights para a otimização de custos e tomada de decisões estratégicas.

## 2. Fontes de Dados

Os dados são carregados a partir do **Google BigQuery**, conectando-se ao dataset `cbsi-operacional`. As principais tabelas utilizadas são:

* `fatos_fretes`: Contém os registros detalhados de cada viagem de frete.
* `vw_operacoes_consolidadas`: Visão consolidada das operações.
* `catalogo_ativos`: Informações sobre os veículos e outros ativos.
* `equipes_tecnicas`: Dados sobre as equipes envolvidas.
* `registros_operacionais`: Logs de eventos operacionais.
* `insights_gerados_ia`: Tabela com insights gerados por IA (não utilizada nos visuais atuais).

## 3. Métricas e Indicadores (KPIs)

O dashboard destaca os seguintes indicadores de performance:

* **Custo Médio por Frete:** R$ 2.396
* **Perda por Ocupação (R$):** R$ 4.18M
* **Peso Médio Transportado (Kg):** 4.66k
* **Custo por Tipo de Veículo:** Análise detalhada do custo médio por viagem para Carreta Eixo Estendido, Carreta Simples, Truck e Toco.
* **Custo por Kg:** Comparativo de custo por quilograma transportado entre VUC, Toco e Carretas.
* **Taxa de Ocupação:** Percentual de utilização da capacidade dos veículos.

## 4. Análises e Visualizações

O painel inclui diversos gráficos para facilitar a análise, como:

* **Evolução do Frete e Peso:** Gráficos de linha que mostram a tendência de custos e volume ao longo do tempo.
* **Análise Comparativa de Veículos:** Gráficos de barras comparando o custo médio por frete, por Km e por Kg entre os diferentes tipos de veículos.
* **Variação Mensal:** Análise da variação percentual dos custos de frete mês a mês.

## 5. Principais Insights e Recomendações

Com base nos dados, o painel oferece as seguintes recomendações estratégicas:

* **Veículo de Maior Custo:** As **Carretas de Eixo Estendido** possuem o maior custo médio por viagem, totalizando R$ 3.004
* **Melhor Custo-Benefício:** O **VUC (Veículo Urbano de Carga)** apresenta o menor custo por quilômetro, sendo a opção mais eficiente para otimização de despesas de transporte.
* **Recomendação Principal:** Priorizar o uso de **VUCs** sempre que a capacidade de carga e o tipo de ativo permitirem, a fim de reduzir significativamente os custos operacionais.
