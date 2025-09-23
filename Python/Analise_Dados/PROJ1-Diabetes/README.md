# PROJETO 1 - DIABETE-DATALAB

![Abertura do projeto](imgProj1.png)


🎯 PROBLEMA DE NEGÓCIO:

Trabalhar com um conjunto de dados contendo informações sobre pacientes que foram  diagnosticados  com  diabetes  ou  que  não  apresentaram  a  condição. O objetivo  é extrair uma amostra desses dados focando nos pacientes que têm mais de 50 anos de idade. Para cada indivíduo nesse subconjunto, necessitamos adicionar uma nova coluna especificando se o paciente está classificado como normal, com um índice de massa corporal (IMC) inferior a 30, ou obeso, com um IMC igual ou superior a 30. Posteriormente, os dados manipulados deverão ser exportados para um novo arquivo CSV e encaminhados ao Cientista de Dados responsável.

Para   solucionar   essa   demanda,   empregaremos   Banco   de   Dados,   Python   e   SQL. Inicialmente,  os  dados  serão  importados  utilizando  a  linguagem  de  programação  Python.  Em seguida,  criaremos  uma  réplica  desses  dados  em  um  banco  de  dados,  onde  realizaremos  as transformações necessárias utilizando consultas SQL. Após a conclusão das alterações e adições requeridas,  os  dados  serão  então  transferidos  de  volta  para  um  dataframe  do  Pandas  e, finalmente, salvaremos o conjunto de dados resultante em um arquivo no formato CSV.Usaremos como fonte de dados o dataset PIMA disponível para download no link abaixo. 

---
🌐 FONTE:

 https://data.world/data-society/pima-indians-diabetes-database

---
📂 CONTÉM NESTE DIRETÓRIO:
- Dataset.csv: arquivo de dados baixado da fonte
- dsadatabase.db: banco de dados SQLite com os dados do dataset.
- PROJ1-diabetes-datalab.ipynb: Arquivo Jupyter notebook com script python.
- imgProj1.png: imagem de abertura do projeto referenciado neste README.
- resultado.csv: relatório que será entregue ao tomador de decisções.