# Sobre
  Conhecido como uma das bebidas mais antigas do mundo, o vinho esteve presente desde o inicio da civilização,  datado cerca de 4000 A.c, as primeiras ferramentas específicas para a produção do vinho e locais de videiras foram encontrada desde a Armênia, Egito até a Grécia França e Itália. A partir disso, o Vinho vem sendo uma das principais bebidas do planetas a ponto de sua composição ser estudado cientificamente para melhorar sua qualidade.

  O presente estudo tem seu cunho de estudo sobre a qualidade do vinho e criar um modelo de Machine Learning para tentar prever qual a qualidade do vinho a partir de suas composições químicas presentes. Assim o modelo utilizado são os modelos de Support Vetorial Classifier (SVC) e Logisstic Regression para determinar a que classe o de qualidade o vinho pertence.

  Vale ressaltar que, apesar da base de dados ser retirado de um repositórido de base de dados públicos, os dados apresentaram inconsistências como presenças de outliers nas features e na variável dependente e o desbalanceamento no número de notas de qualidade do vinho, assim foi necessário a utilziação de métodos de pré processamentos dos dados para garantir a melhor acurácia dos modelo criado, Além disso, pela natureza das features, foi necessário o pré processamento de padronização dos dados antes da criação do modelo.

# Ferramentas
## Python
- Tratamento dos dados: Pandas
- Biblioteca de Machine Learning: Sklearn
- Biblioteca para análise estatística: Statsmodels
- Bibliotecas de pré processamentos: Imblearn e Sklearn
- Gráficos: Seabron e Matplotlib

## Base de dados utilizado
  A base de dados é pública e foi retirada no site da UCI Machine Learning Repository:

Cortez,Paulo, Cerdeira,A., Almeida,F., Matos,T., and Reis,J.. (2009). Wine Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.

# Resultados


# Step by Step
1. Importação dos dados
2. Conhecendo os dados

   2.1 Observando os outliers
   
   2.2 Tratando os Outliers
   
   2.3 Histograma após o tratamento

3 Criando Modelo no Statsmodels
