<h1 align="center">Credit Limit</h1>

<p align="center">Projeto desenvolvido durante o evento <em>3º Hackday CDS</em> (Comunidade Data Science), utilizando algoritmos de Machine Learning via Python, para solucionar um problema de classificação de clientes.
Objetivos: Simular ambiente de negócio real | Trabalho em equipe | Networking | Aceleração do conhecimento | </p>

![Getting Started](img/credit_img_readme.jpg)

Table of Content
=================
<p align="center">
 <a href="#about">About</a> •
 <a href="#the-problem">The Problem</a> •
 <a href="#goals">Goals</a> •
 <a href="#assumptions">Assumptions</a> •
 <a href="#tools">Tools</a> • 
 <a href="#steps">Steps</a> • 
 <a href="#solution">Solution</a> • 
 <a href="#how-to-use">How to use</a> • 
 <a href="#lessons-learned">Lessons Learned</a> • 
 <a href="#next-steps">Next Steps</a> • 
 <a href="#references">References</a> • 
 <a href="#autor">Autor</a> • 
 <a href="#team">Team</a>  • 
 <a href="#license">License</a> • 
</p>

# About 

O Billion Bank é um banco digital brasileiro, fundado em 2021. Trabalha hoje com contas digitais, e cartões de crédito. 

# The Problem

Quando um cliente solicita aumento de limite no cartão de crédito, o banco consulta uma empresa de crédito terceira, que retorna uma recomendação: "negar" ou "conceder". Essa resposta é repassada ao cliente. Dado que a empresa de crédito precisa levantar maiores informações de histórico financeiro do cliente com terceiros, o retorno da recomendação ao banco leva até 5 dias úteis!

Tratando-se de um serviço, a cada solicitação de aumento de limite feita por um cliente, o banco tem um custo adicional de consulta. Visando reduzir este custo, em 2022, o banco passou a só aceitar novos pedidos de aumento de limite a cada 3 meses. O banco viu um aumento leve do churn no primeiro semestre, que se acentuou mais no segundo, chegando a um ponto já preocupante. O time de CS fez contato com antigos clientes, e constatou que o principal motivo do churn foi a percepção de burocracia relacionada ao aumento nos limites.

# Goals

- Desburocratizar o processo, permitindo que o cliente possa solicitar um novo limite uma vez por semana, tendo uma resposta instantânea.
- Desativar as consultas de recomendação de aumento de limites feitas hoje com a empresa terceira, que são demoradas e custosas.
- O modelo deverá avaliar a solicitaçaõ de aumento de limite de cartão de crédito.
- O modelo irá informar se o banco deverá conceder ou não o aumento do limite de crédito solicitado pelo cliente.

# Planning

## Assumptions

- Registros com idade superiores a 18 anos
- 

## Tools

As seguintes ferramentas foram usadas na construção do projeto:

- [Python](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [Jupyter Notebook](https://jupyter.org/)
- [Github](https://github.com/)
- [SKLearn](https://scikit-learn.org/stable/)
- [XGBoost](https://xgboost.readthedocs.io/en/stable/)

# Execution

## Steps

### Step 01. Data Description:
Coletar dados em um banco de dados na AWS Cloud.
</br>Compreender o significado de cada atributo dos interessados.
</br>Renomear colunas, compreender dimensões e tipos dos dados.
</br>Identificar e tratar dados nulos.
</br>Analisar atributos através de estatística descritiva.
</br>Separar 20% dos dados para teste (aleatoriamente, mas estratificados pela variável resposta).

### Step 02. Feature Engineering:
Criar mindmap de hipóteses de negócio.
</br>Realizar a feature engeneering, criando as features necessárias para validação das hipóteses.

### Step 03. Data Filtering:
Filtrar registros e atributos de acordo com restrições de negócio.

### Step 04. Exploratory Data Analysis:
Realizar uma análise univariada com uso do SweetViz, avaliando detalhes de cada atributo.
</br>Realizar uma análise bivariada, validando as hipóteses criadas e gerando insights de negócio.
</br>Criar tabela de resultados das hipóteses, e relevância estimada dos atributos para o aprendizado dos modelos.

### Step 05. Data Preparation:
Padronizar atributos numéricos com distribuição normal.
</br>Reescalar atributos numéricos com distribuição não normal.
</br>Codificar atributos categóricos em atributos numéricos.
</br>Aplicas as transformações acima aos dados de teste.

### Step 06. Feature Selection:
Separar dados de treino e validação.
</br>Rodar algoritmo para obter sugestão de atributos relevantes.
</br>Analisar o resultado em conjunto com os atributos relevantes estimado na EDA.
</br>Selecionar apenas os melhores atributos para treinar os modelos de machine learning.

### Step 07. Machine Learning Modelling:
Rodar algoritmos: KNN classifier, Logistic regression, ExtraTrees classifier, e XGBboost classifier.
</br>Plotar curva de ganho cumulativo e lift, e calcular precison@k/recall@k de cada modelo.
</br>Criar tabela de performance comparando precison@k/recall@k de cada modelo.

### Step 08. Hyperparameter Fine Tunning:
Fazer um ajuste fino de hiperparâmetros em cada modelo, identificando o melhor conjunto de parâmetros para maximizar suas capacidades de aprendizagem.
</br>Aplicar validação cruzada em cada modelo, reduzindo o viés de seleção (teoria da amostragem), por utilizar várias amostras diferentes dos dados.
</br>Selecionar os 4 modelos com melhor conjunto de hiperparâmetros, e avaliar sua capacidade de aprendizagem.
</br>Plotar curvas de ganho cumulativo e lift, comparando os 4 modelos.
</br>Calcular precison@k/recall@k dos 4 modelos, e selecionar o de melhor performance.
</br>Submeter esse modelo aos dados de teste, e plotar suas curvas de ganho cumulativo e lift.
</br>Comparar precison@k/recall@k em treino vs. teste, avaliando a capacidade de generalização do modelo (aprendizado com dados inéditos).

### Step 09. Convert Model Performance to Business Values:
Responder as questões de negócio do gestor ao call center.
</br>Comparar resultados da lista aleatória com a lista ordenada por propensão de compra.
</br>Traduzir a performance do modelo em resultados financeiros para a Insurance All.




## Solution

- Criação de novas features
- A métrica utilizada foi a F1Score (média harmónica entre a precision(tentativas) e a recall(disponibilidade))




## How to use

+ Executar o comando em ambiente local: <em>git clone https://github.com/mbouhid/hackdays3_credit_limit.git</em>
+ Instalar as bibliotecas que estão no arquivo <em>requirements.txt</em>
+ Executar o arquivo <em>notebooks/baseline_kaggle_hackdays3.ipynb</em>




## Lessons Learned

- Em projetos com curto espaço de tempo, importante estruturar e executar um modelo o mais rápido possível, pois o resultado servirá de baseline para os próximos.
- Planejar, definir e designar bem as atividades de cada participante.
- Focar em discussões para a criação de novas features.
- Conhecer sobre o negócio e entender as features do dataset original.


## Next Steps

+



## References

[Kaggle](https://www.kaggle.com/competitions/cdshackdays3)

[Comunidade Data Science](https://www.comunidadedatascience.com/)


## Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/41192466?v=4" width="100px;" alt=""/>

[![Linkedin Badge](https://img.shields.io/badge/-MarcioBouhid-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/marciobouhid/)](https://www.linkedin.com/in/marciobouhid/) 


## Team

Marcio Bouhid(https://www.linkedin.com/in/marciobouhid/)

Danillo Barros(https://www.linkedin.com/in/danillo-cordeiro/)

Almir Lopes(https://www.linkedin.com/in/almirmartinslopes/)


## License

GNU General Public License v3.0

