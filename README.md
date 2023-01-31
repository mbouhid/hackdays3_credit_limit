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
 <a href="#solução">Solução</a> • 
 <a href="#utilizacao">Como instalar</a> • 
 <a href="#Lições_Aprendidas">Lições Aprendidas</a> • 
 <a href="#proximos_passos">Próximos Passos</a> • 
 <a href="#referências">Referências</a> • 
 <a href="#autor">Autor</a> • 
 <a href="#contribuidores">Contribuidores</a>  • 
 <a href="#licenc-a">Licença</a> • 
</p>

# About 

O Billion Bank é um banco digital brasileiro, fundado em 2021. Trabalha hoje com contas digitais, e cartões de crédito. 

## The Problem

Quando um cliente solicita aumento de limite no cartão de crédito, o banco consulta uma empresa de crédito terceira, que retorna uma recomendação: "negar" ou "conceder". Essa resposta é repassada ao cliente. Dado que a empresa de crédito precisa levantar maiores informações de histórico financeiro do cliente com terceiros, o retorno da recomendação ao banco leva até 5 dias úteis!

Tratando-se de um serviço, a cada solicitação de aumento de limite feita por um cliente, o banco tem um custo adicional de consulta. Visando reduzir este custo, em 2022, o banco passou a só aceitar novos pedidos de aumento de limite a cada 3 meses. O banco viu um aumento leve do churn no primeiro semestre, que se acentuou mais no segundo, chegando a um ponto já preocupante. O time de CS fez contato com antigos clientes, e constatou que o principal motivo do churn foi a percepção de burocracia relacionada ao aumento nos limites.

## Solving

Para reverter o cenário, o banco traçou um plano de ação com dois objetivos:
1 - Desburocratizar o processo, permitindo que o cliente possa solicitar um novo limite uma vez por semana, tendo uma resposta instantânea.
2 - Desativar as consultas de recomendação de aumento de limites feitas hoje com a empresa terceira, que são demoradas e custosas.


## Goals
O Objetivo do modelo será:

1. Avaliação de aumento de limite de cartão de crédito
2. Informar se o banco deverá conceder ou não o aumento do limite de crédito solicitado pelo cliente.


## Assumptions

- Na limpeza dos dados:
   - Retirados os ID´s duplicados
   - Retirado o ID com número de quartos igual a 33 (possível erro de digitação)  
- Imóveis em bom estado foram considerados como condition igual 3 ou 4
- O crescimento anual foi calculado com o valor médio dos imóveis por ano, pois a base de dados só possuia o período de 13 meses.

# Planning
## Tools

As seguintes ferramentas foram usadas na construção do projeto:

- [Python](https://www.python.org/)
- [Streamlit](https://streamlit.io/)
- [Pandas](https://pandas.pydata.org/)

## Solução

- [HC_App_final_Streamlit.pdf](https://github.com/mbouhid/project_house_rocket/blob/main/hc_app_final_Streamlit.pdf)
- [HC_App_final_Streamlit_Menu.pdf](https://github.com/mbouhid/project_house_rocket/blob/main/hc_app_final_Streamlit_Menu.pdf)

## Como Instalar

Passo a passo de como rodar o modelo.

## Lições Aprendidas

- A base de dados tem que estar limpa
- As afirmações devem ser bem claras para que a solução da análise confirme ou não as hipóteses
- Nem toda afimação/hipótese tem solução ou será respondida
- Identificar claramente as premissas para alinhamento das expectativas
- Importante saber exatamente o que o cliente precisa.
- Identificar as necessidades mesmo que não esteja no pedido do cliente.


## Referências

[Kaggle](https://www.kaggle.com/)

[Github](https://github.com/)

[Comunidade Data Science](https://www.comunidadedatascience.com/)

[Blog Seja Um Data Scientist](https://medium.com/@meigarom/os-5-projetos-de-data-science-que-far%C3%A1-o-recrutador-olhar-para-voc%C3%AA-c32c67c17cc9)


## Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/41192466?v=4" width="100px;" alt=""/>

[![Linkedin Badge](https://img.shields.io/badge/-MarcioBouhid-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/marciobouhid/)](https://www.linkedin.com/in/marciobouhid/) 


## Contribuidores

O projeto não teve contribuidores oficiais. A Comunidade Data Science foi consultada em determinados momentos.


## Licença

GNU General Public License v3.0

