# Supply Chain Analytics (PySpark)

## Visão Geral
Este projeto tem como background o estudo da área de Supply Chain Analytics e o uso de PySpark para análise de dados em escala. O objetivo é analisar o risco de atraso na entrega de produtos após a compra, explorando o conjunto de dados, extraindo padrões e treinando um modelo preditivo.

## Objetivos
- Entender o comportamento das vendas e dos pedidos por região, produto e mercado.
- Explorar padrões de compra com regras de associação (FPGrowth).
- Construir um modelo preditivo para classificar o risco de atraso na entrega.

## Dataset
- Fonte: DataCo Supply Chain Dataset (Mendeley)
- Arquivo principal: `dados/DataCoSupplyChainDataset.csv`
- Arquivo processado: `dados/DataCoSupplyChainDatasetProcessados.csv`

## Ferramentas e Bibliotecas
- Python
- PySpark (MLlib)
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Estrutura do Projeto
- `SupplyChain-Analytics-PySpark.ipynb`: notebook principal com EDA, regras de associação e modelagem.
- `dados/`: diretório esperado para os arquivos CSV.

## Etapas do Projeto
1. **Análise Exploratória (EDA)**
   - Limpeza de colunas e tratamento de valores ausentes
   - Exploração de vendas por região, produto e mercado

2. **Regras de Associação**
   - Agrupamento de compras por cliente
   - Extração de padrões com FPGrowth

3. **Modelagem Preditiva**
   - Preparação das features
   - Treinamento de modelo com Decision Tree
   - Avaliação de desempenho

## Resultado Final e Métricas
O resultado final é um pipeline analítico completo, que vai da exploração dos dados até a construção de um modelo preditivo para risco de atraso na entrega. A avaliação do modelo inclui:
- **Acurácia**
- **Precisão (weighted)**
- **Recall (weighted)**
- **F1-score**
- **AUC (ROC)**
- **Matriz de confusão**

As métricas e resultados numéricos são exibidos na seção **Avaliação do Modelo** dentro do notebook.

## Análise Final dos Resultados
Os resultados indicam que o pipeline é capaz de capturar padrões relevantes tanto no comportamento de compra quanto no risco de atraso, permitindo uma visão integrada entre análise exploratória, regras de associação e predição. As métricas fornecem um diagnóstico inicial do desempenho do modelo, destacando pontos fortes e possíveis gargalos para futuras iterações. No geral, o projeto cumpre o objetivo de demonstrar conceitos essenciais de Supply Chain Analytics com PySpark, deixando espaço para melhorias incrementais em validação e engenharia de dados.

---

## Como Executar
1. Abra o notebook `SupplyChain-Analytics-PySpark.ipynb`.
2. Garanta que os dados estejam disponíveis na pasta `dados/`.
3. Execute as células em ordem.

## Limitações e Futuras Melhorias
- **Split simples** (random split sem estratificação ou validação cruzada)
- **Potencial de melhorar o pré-processamento** (mais robustez e automação)
- **Melhoria do pipeline para melhor reprodução** (padronização e reprodutibilidade)


