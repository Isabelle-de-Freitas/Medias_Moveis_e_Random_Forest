# Modelos: Médias Móveis e Random Forest

* **Definição - Modelo de Médias Móveis:** técnica utilizada em séries temporais para suavizar dados ou prever valores futuros com base em flutuações passadas. Ele pode ser aplicado tanto para análise de dados históricos quanto para modelagem estatística.

* **Definição - Modelo Random Forest:** baseado em árvores de decisão (estrutura de dados que representa uma sequência de decisões e suas consequências). Ele pertence à classe dos métodos $ensemble$, que combina vários modelos para melhorar a precisão e reduzir o risco de $overfitting$. Possui característica de ser resistente a $outliers$ e dados ruidosos.


O **objetivo** deste trabalho é realizar a previsão da temperatura para as próximas 24 horas, baseada nas observações anteriores, utilizando como métrica de avaliação principal o **Mean Absolute Error (MAE)**.


## Dependências

* ```pandas```: para leitura e manipulação dos dados
* ```numpy```: para realizar operações em array
* ```matplotlib```: para visualizações estáticas ou interativas
* ```seaborn```: para criar gráficos de forma eficiente e visualmente atraente
* ```sklearn```: para criar, treinar e implementar modelos de aprendizado de máquina

## Estrutura do projeto

- $1.$ Introdução sobre o tema
- $2.$ Contexto sobre o dataset
    - $2.1$ Mas, o que é biogeoquímica?
    - $2.2$ Por que esses estudos são importantes?
- $3.$ Dados
- $4.$ Objetivo do estudo
- $5.$ Importação de bibliotecas e pacotes
- $6.$ Leitura dos dados
- $7.$ Análise descritiva geral
    - $7.1$ Análise descritiva das variáveis "T (degC)" e "Date Time"
- $8.$ Proposta de um Modelo Baseline
    - $8.1$ Preparação dos dados
    - $8.2$ Modelo de Médias Móveis
    - $8.3$ Gráfico de linhas do Modelo de Médias Móveis
    - $8.4$ Tratamentos para aplicar a métrica MAE
    - $8.5$ Métrica MAE - Mean Absolute Error
    - $8.6$ Análise de resíduos
    - $8.7$ Conclusão sobre o Modelo de Médias Móveis
- $9.$ Proposta de um modelo mais complexo
    - $9.1$ Aprendizado de máquina
    - $9.2$ Random Forest
    - $9.2.1$ Preparação dos dados
    - $9.2.2$ Análise descritiva
    - $9.2.3$ Preparação dos dados para a modelagem
    - $9.2.4$ Modelagem
    - $9.2.5$ Gráfico de linhas do Modelo Random Forest
    - $9.2.6$ Aplicação da métrica MAE - Random Forest
    - $9.2.7$ Análise de resíduos
    - $9.2.8$ Seleção de variáveis importantes
    - $9.2.9$ Otimização de hiperparâmetros
    - $9.2.10$ Aplicação da métrica MAE - Random Forest Otimizado
    - $9.2.11$ Gráfico de linhas do Modelo Random Forest Otimizado
    - $9.2.12$ Análise de resíduos
    - $9.1.13$ Seleção de variáveis importantes - Random Forest Otimizado
- $10.$ Conclusão final sobre os modelos propostos
    - $10.1$ Em relação ao custo operacional
    - $10.2$ Em relação à métrica MAE
    - $10.3$ Em relação à complexidade dos dados
    - $10.4$ Em relação à captura da sazonalidade
- $11.$ Sugestões de outros modelos
    - $11.1$ Modelos Estatísticos
    - $11.2$ Modelos de Aprendizado de Máquina
    - $11.3$ Modelos de Séries Temporais

**Obs.:** o conjunto de dados, Jena Climate, foi coletado no site $Kaggle$: (https://www.kaggle.com/datasets/mnassrib/jena-climate/data).
