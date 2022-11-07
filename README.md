<h1 align="center">Credit Limit (Hackday's Project)</h1>

<p align="center">A Credit Limit Classification Business Problem.</p>

Table of Content
=================
<p align="center">
 <a href="#about">About</a> •
 <a href="#objective">Objective</a> •
 <a href="#on-premise">On-Premise</a> •
 <a href="#technologies">Technologies</a> • 
 <a href="#solution">Solution</a> • 
 <a href="#Lesson_Learned">Lesson Learned</a> • 
 <a href="#backlog">Backlog</a> • 
 <a href="#references">References</a> • 
 <a href="#autor">Autor</a> • 
 <a href="#team">Team</a>  • 
 <a href="#license">License</a> • 
</p>

### About

A Credit Limit Classification Business Problem. We need to develop a model in 2 days to predict if a bank should concede or not give a higher credit limit to its clients.


### Objective
O Objetivo na exploração dos dados é analisar e identificar:
 1. Imóveis que estejam abaixo da mediana da região de localização
 2. Imóveis com boas condições e vista para a água
 3. Identificar a sazonalidade da data da compra (summer or winter)
 4. Analisar e confirmar as hipóteses:
    - H1: Imóveis que possuem vista para água, são 30% mais caros, na média.
    - H2: Imóveis com data de construção menor que 1955, são 50% mais baratos, na média.
    - H3: Imóveis sem porão possuem área total 50% maiores do que com porão.
    - H4: O crescimento do preço dos imóveis YoY (Year over Year) é de 10%
    - H5: Imóveis com 3 banheiros tem um crescimento MoM (Month over Month) de 15%


### On-Premise

- Na limpeza dos dados:
   - Retirados os ID´s duplicados
   - Retirado o ID com número de quartos igual a 33 (possível erro de digitação)  
- Imóveis em bom estado foram considerados como condition igual 3 ou 4
- O crescimento anual foi calculado com o valor médio dos imóveis por ano, pois a base de dados só possuia o período de 13 meses.


### Technologies

As seguintes ferramentas foram usadas na construção do projeto:

- [Python](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [SKLearn](https://scikit-learn.org/)

### Solution

- [HC_App_final_Streamlit.pdf](https://github.com/mbouhid/project_house_rocket/blob/main/hc_app_final_Streamlit.pdf)
- [HC_App_final_Streamlit_Menu.pdf](https://github.com/mbouhid/project_house_rocket/blob/main/hc_app_final_Streamlit_Menu.pdf)

### Lesson Learned

- A base de dados tem que estar limpa
- As afirmações devem ser bem claras para que a solução da análise confirme ou não as hipóteses
- Nem toda afimação/hipótese tem solução ou será respondida
- Identificar claramente as premissas para alinhamento das expectativas
- Importante saber exatamente o que o cliente precisa.
- Identificar as necessidades mesmo que não esteja no pedido do cliente.

### Backlog

- Identify new features
- Apply others ML Algorithms
- Find news hyperparameters


### References

[Kaggle](https://www.kaggle.com/)

[Github](https://github.com/)

[Comunidade Data Science](https://www.comunidadedatascience.com/)

[Blog Seja Um Data Scientist](https://medium.com/@meigarom/os-5-projetos-de-data-science-que-far%C3%A1-o-recrutador-olhar-para-voc%C3%AA-c32c67c17cc9)


### Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/41192466?v=4" width="100px;" alt=""/>

[![Linkedin Badge](https://img.shields.io/badge/-MarcioBouhid-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/marciobouhid/)](https://www.linkedin.com/in/marciobouhid/) 


### Team

O projeto não teve contribuidores oficiais. A Comunidade Data Science foi consultada em determinados momentos.


### License

GNU General Public License v3.0

