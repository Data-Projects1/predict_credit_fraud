# Previsão de fraude em compras com cartão de crédito

![card_safe](/img/secure_payment.jpg "Card Safety")

Este projeto contempla o ciclo completo de um modelo de Machine Learning, baseado no método CRISP desde o entendimento do problema, limpeza de dados, exploração de dados (EDA), modelagem dos dados, treinamento e avaliação do modelo até a disponibilização de uma base de dados com base de prováveis respostas de satisfação depassageiros de companhia aérea.

O modelo foi treinado utilizando o dataset train.csv, com o objetivo de prever se um passageiro estará satisfeito com serviços de uma companhia aérea.

O projeto aborda etapas importantes do ciclo CRISP-SP de um modelo de Machine Learning:

1. Questão de negócio
2. Entendimento do negócio
3. Coleta de dados
4. Limpeza de dados
5. Exploração de dados (EDA)
6. Modelagem de dados
7. Algoritmos de Machine Learning (treinamento de modelos de classificação)
8. Avaliação dos algoritmos (otimização de hiperparâmetros)
9. Exportação do modelo

## Estrutura das pastas

| Pasta            | Descrição                                                             |
| ---------------- | --------------------------------------------------------------------- |
| img              | Imagens utilizadas no projeto                                         |
| notebook         | Notebook com processo de análise de dados e desenvolviemnto do modelo |
| src              | Versionamento do python                                               |
| .gitignore       | Arquivos com dados a serem ignorados na publicação                    |
| README.md        | Documentação do projeto                                               |
| requirements.txt | Requisitos mínimos para executar o projeto                            |

## Análise curva ROC

A avaliação da análise será com base na área sob a curva ROC (Receiver Operating Characteristic), para avaliar o desempenho de modelos de classificação de satisfação de forma binária na comparação do cálculo de probabilidade prevista e o resultado observado através de modelos de Machine Learning como Logistic Regression, Random Forest, XGBoost e LightGBM.

### Problema de Negócio

O resultado deve fazer a previsão da probabilidade para a variável de fraude com cartão de crédito.

#### Base de Dados

train.csv - conjunto de treinamento, com dados de fraude como alvo.<br/>
test.csv - conjunto de teste, utilizado para prever a fraude em transações com cartão de crédito.<br/>
sample_submission.csv - arquivo de submissão de exemplo no formato correto.<br/>

[Kaggle - Predicting Credit Card Fraud](https://www.kaggle.com/competitions/playground-series-s6e11/overview)

#### Campos de Dados

- id - ID que representa uma compra do conjunto de teste.<br/>
- amount_usd <br/>
- hours_since_last_txn <br/>
- txn_count_last_24h <br/>
- distance_from_home_km <br/>
- card_age_months <br/>
- customer_age <br/>
- account_balance_usd <br/>
- cvv_retry_count <br/>
- velocity_score <br/>
- time_of_day_hour <br/>
- day_of_week <br/>
- merchant_risk_score <br/>
- prior_disputes <br/>
- merchant_category <br/>
- card_type <br/>
- auth_method <br/>
- channel <br/>
- device_type <br/>
- is_foreign_transaction <br/>
- is_new_merchant <br/>
- used_vpn <br/>
- ip_country_mismatch <br/>
- billing_shipping_mismatch <br/>
- is_ai_generated_scam_attempt <br/>
- is_fraud <br/>
