[![author](https://img.shields.io/badge/author-rgolino-red.svg)](https://www.linkedin.com/in/renato-golino/) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-365/) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/rafaelnduarte/portfolio/issues)

# Previsão de Rotatividade de Clientes nas Empresa de Telecomunicações
<img src ="https://img.freepik.com/fotos-gratis/tablet-com-aplicacoes_1134-123.jpg?t=st=1732056112~exp=1732059712~hmac=1a4be5fe493c1882d388357eb5c2c9516ad19230030a626338c1ba5645d808ee&w=1480">


## Objetivo
O projeto tem como objetivo prever a evasão de clientes (*churn*) em uma empresa de telecomunicações. A ideia principal é identificar clientes com alto risco de cancelar seus serviços, permitindo que ações estratégicas sejam tomadas para a retenção.

## Aplicabilidade
O churn é uma métrica crucial, pois reduzir a taxa de evasão é mais eficiente e menos custoso do que adquirir novos clientes. Assim, prever o churn ajuda a:
- Identificar clientes em risco de saída.
- Propor ações direcionadas para retenção.
- Aumentar a eficiência operacional e reduzir custos com novos clientes.

## Resolução Proposta
A solução proposta baseia-se na aplicação de ciência de dados, com etapas estruturadas em uma pipeline de Machine Learning:
1. **Coleta de Dados**: 
    - Dados coletados da plataforma IBM Developer.
    - Dataset com 7043 registros e 21 variáveis.

2. **Pré-processamento**: 
    - Tratamento de dados ausentes na coluna `TotalCharges`.
    - Conversão de variáveis categóricas em numéricas.
    - Análise e remoção de colunas irrelevantes, como `customerID`.

3. **Modelagem**: 
    - Teste de diferentes algoritmos, incluindo:
        - Random Forest
        - XGBoost
        - Regressão Logística, entre outros.
    - Uso de técnicas de balanceamento de classes para lidar com o desbalanceamento.

4. **Avaliação**:
    - Métricas como ROC-AUC, F1-Score, e matriz de confusão para análise do desempenho.


## Pipeline do Projeto
1. **Importação dos Dados**:
   - Fonte: [Dataset IBM](https://raw.githubusercontent.com/carlosfab/dsnp2/master/datasets/WA_Fn-UseC_-Telco-Customer-Churn.csv).

2. **Pré-processamento**:
   - Análise de valores ausentes.
   - Conversão de tipos de dados.
   - Codificação de variáveis categóricas.

3. **Análise Exploratória**:
   - Verificação das distribuições de variáveis.
   - Identificação de padrões e correlações.

4. **Modelagem e Treinamento**:
   - Treinamento de modelos supervisionados.
   - Uso de técnicas de validação cruzada e ajuste de hiperparâmetros.

5. **Avaliação de Resultados**:
   - Relatórios de desempenho com base nas métricas.

## Execução
### Requisitos
Instale as dependências necessárias executando:
```bash
pip install scikit-plot imbalanced-learn lightgbm xgboost
```

### Execução do Projeto
1. Clone o repositório e abra o notebook.
2. Certifique-se de que o dataset está acessível no caminho especificado.
3. Execute as células sequencialmente para replicar os resultados.

## Conclusão
O projeto demonstra como técnicas de ciência de dados podem ser usadas para resolver problemas de negócios, como a previsão de churn. A abordagem é escalável e pode ser adaptada para outras indústrias e casos de uso similares.

**Observações**
O projeto utiliza um pipeline padronizado para projetos de ciência de dados e pode ser ampliado para incluir técnicas adicionais, como explicabilidade de modelos e otimização em produção.

## Projeto Completo

[Previsão de Rotatividade](https://github.com/rgolino/Previsao_Rotatividade/blob/main/PROJETO_Churn_Prediction_para_uma_empresa_de_Telecomunica%C3%A7%C3%B5es.ipynb)

