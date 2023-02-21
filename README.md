<h1 align="center">Credit Limit</h1>

<p align="center">Projeto desenvolvido durante o evento <em>3º Hackday CDS</em> (Comunidade Data Science), utilizando algoritmos de Machine Learning via Python, para solucionar um problema de classificação de clientes.</p>

![Getting Started](img/credit_img_readme.jpg)

Table of Content
=================
<p align="center">
 <a href="#about">About</a> •
 <a href="#the-problem">The Problem</a> •
 <a href="#goals">Goals</a> •
 <a href="#assumptions">Assumptions</a> •
 <a href="#tools">Tools</a> • 
 <a href="#solution">Solution</a> • 
 <a href="#how-to-use">How to use</a> • 
 <a href="#lessons-learned">Lessons Learned</a> • 
 <a href="#next-steps">Next Steps</a> • 
 <a href="#referencias">Referências</a> • 
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

## Solution

- Criação de novas features
- A métrica utilizada foi a F1Score (média harmónica entre a precision(tentativas) e a recall(disponibilidade))




## How to use

+ Instalar as bibliotecas que estão no arquivo <em>requirements.txt</em>
+ 




## Lessons Learned

- 


## Next Steps

+



## Referências

[Kaggle](https://www.kaggle.com/competitions/cdshackdays3)

[Comunidade Data Science](https://www.comunidadedatascience.com/)


## Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/41192466?v=4" width="100px;" alt=""/>

[![Linkedin Badge](https://img.shields.io/badge/-MarcioBouhid-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/marciobouhid/)](https://www.linkedin.com/in/marciobouhid/) 


## Team

Danillo Barros(https://www.linkedin.com/in/danillo-cordeiro/)
Almir Lopes(https://www.linkedin.com/in/almirmartinslopes/)


## License

GNU General Public License v3.0

