# Previsão de Doença Cardiovascular: CRISP-DM com Deployment no Amazon SageMaker

> Projeto completo nas 6 fases do CRISP-DM, terminado com um modelo XGBoost publicado num endpoint do SageMaker para inferência em tempo real e em lote.

**Mestrado em Business Intelligence & Analytics (ISCAP)**, cadeira de Business Analytics: Ferramentas e Aplicações, 2025/26

## O problema
Identificar pacientes com risco de doença cardiovascular a partir de variáveis fáceis de recolher, como idade, pressão arterial, colesterol e hábitos, para apoiar a triagem clínica.

## Fases CRISP-DM
1. **Business Understanding**: problema, objetivos, questões de pesquisa e análise SWOT.
2. **Data Understanding**: dicionário de dados e qualidade (valores em falta, duplicados, outliers clínicos).
3. **Data Preparation**: regras de limpeza, feature engineering e codificação.
4. **Modeling**: 4 modelos com normalização e divisão treino/teste.
5. **Evaluation**: métricas, matrizes de confusão, curvas ROC/AUC e importância das variáveis.
6. **Deployment**: XGBoost no **Amazon SageMaker**, com endpoint em tempo real e *Batch Transform*.

## Resultados
- AUC de cerca de **0,79** e accuracy de cerca de **73%**, com desempenhos parecidos entre os quatro modelos.
- O modelo foi escolhido com prioridade ao **recall**, porque o erro mais grave é um falso negativo: classificar um doente como saudável.

## Stack
`pandas` · `scikit-learn` · `XGBoost` · `Amazon SageMaker` · `boto3` · `seaborn`

## Autores (Grupo 3)
Giulia Jacobina · João Coelho · Larissa Tostes
