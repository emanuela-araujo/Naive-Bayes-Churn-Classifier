# Naive-Bayes-Churn-Classifier
## Objetivos:
Este repositório contém um projeto básico de ciência de dados focado na previsão de churn de clientes usando modelos de Naive Bayes.
O código foi desenvolvido com o objetivo de praticar a estrutura básica para a construção de um modelo de Naive Bayes.

## Como usar?
Baixe a base de dados do repositório e altere o caminho no trecho quem que o `pandas` lê o csv `pd.read_csv(caminho do arquivo)`
 
## A Base de dados:
Os dados usados para treinar o modelo são de uma base fictícia do Kaggle.

O dataset inclui dados sobre:
* Clientes que deram churn no último mês
* Serviços contratados por cada cliente (Telefone, Backup, Proteção de dispositivo, suporte técnico, Canais de streaming, etc)
* Conta do cliente (Quanto tempo como cliente, contrato, método de pagamento, recargas mensais, recargas totais,etc.)
* Informações demográficas dos clientes (Gênero, faixa etária, etc.)

## Os modelos escolhidos
O Naive Bayes tem como base o **teorema de Bayes**, um princípio da probabilidade. 
A biblioteca Scikit Learn traz três tipos de Naive Bayes: Gaussiano, Multinomial e de Bernoulli.
Para este projeto, foram utilizados os modelos Gausiiano e de Bernoulli.

## Resultados
Ao testar os dois tipos de modelo, foi possível observar que o modelo de Bernoulli apresentou métricas melhores que o Gaussiano. Isso ocorre porque o Naive Bayes de Bernoulli é projetado para dados binários (presença ou ausência de features), enquanto o Naive Bayes Gaussiano é mais adequado para dados contínuos que seguem uma distribuição normal.

Os dados utilizados no treinamento do modelo (a maior parte deles categóricos) foram  transformados em representações binárias via One-Hot Encoding, o que tornou o modelo de Bernoulli mais adequado.
