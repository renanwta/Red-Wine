# Sobre
  Conhecido como uma das bebidas mais antigas do mundo, o vinho esteve presente desde o inicio da civilização,  datado cerca de 4000 A.c, as primeiras ferramentas específicas para a produção do vinho e locais de videiras foram encontrada desde a Armênia, Egito até a Grécia França e Itália. A partir disso, o Vinho vem sendo uma das principais bebidas do planetas a ponto de sua composição ser estudado cientificamente para melhorar sua qualidade.

  O presente estudo tem seu cunho de estudo sobre a qualidade do vinho e criar um modelo de Machine Learning para tentar prever qual a qualidade do vinho a partir de suas composições químicas presentes. Assim o modelo utilizado são os modelos de Support Vetorial Classifier (SVC) ,Logistic Regression e XGBoostClassifier para determinar a que classe o de qualidade o vinho pertence.

  Vale ressaltar que, apesar da base de dados ser retirado de um repositórido de base de dados públicos, os dados apresentaram inconsistências como presenças de outliers nas features e na variável dependente e o desbalanceamento no número de notas de qualidade do vinho, assim foi necessário a utilziação de métodos de pré processamentos dos dados para garantir a melhor acurácia dos modelo criado, Além disso, pela natureza das features, foi necessário o pré processamento de padronização dos dados antes da criação do modelo.

# Ferramentas
## Python
- Tratamento dos dados: Pandas
- Biblioteca de Machine Learning: Sklearn
- Biblioteca de seleção de Features: SelectKBest e F_classifier 
- Bibliotecas de pré processamentos: Imblearn e Sklearn
- Gráficos: Seaborn e Matplotlib

## Base de dados utilizado
  A base de dados é pública e foi retirada no site da UCI Machine Learning Repository:

Cortez,Paulo, Cerdeira,A., Almeida,F., Matos,T., and Reis,J.. (2009). Wine Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.

# Resultados
Após todos os tramentos e pré processamento dos dados, foi refeita os modelos de de SVC e Logistic Regression, assim, para poder validar e veriicar qual dos modelos a serem utilizados, foi calculado o a curva ROC e a pontuação AUC.
<div align="center">
<img src="https://github.com/renanwta/Red-Wine/assets/161327900/caf9aec9-482b-4fc0-9037-c08f5ed6d716" width="500px" />
</div>
Para a curva ROC do modelo de SVC temos que a pontuação AUC foi de 85%

<div align="center">
<img src="https://github.com/user-attachments/assets/7d8a2d6e-b3b7-4fbf-8e35-e47b2809809c" width="500px" />
</div>
Já para a curva ROC do modelo de SVC temos que a pontuação AUC foi de 81%


<div align="center">
<img src="https://github.com/user-attachments/assets/8401be45-de5e-4d60-b1c2-7846814a42e0" width="500px" />
</div>
Já para a curva ROC do modelo de SVC temos que a pontuação AUC foi de 92%

Assim dizemos que o melhor modelo a ser utilziado será o modelo de XGBoostClassifier para prever as classes da qualidade do vinho


# Step by Step
1. Importação dos dados
2. Conhecendo os dados

   2.1 Observando os Outliers
   
   2.2 Tratando os Outliers
   
   2.3 Histograma após o tratamento

3. Selecionando as features

   3.1 Encontrando as Colunas

4. Criação dos modelo Suport Vetorial Classification - SVC
   
   4.1 Cálculo do base line
   
5. Criação dos modelo Logistic Regression
   
   5.1 Cálculo do base line

6. Primeira Conclusão
7. Rebalanceamento dos dados da variável dependente
8. Novo Modelo de SVC
   
 8.1 Cálculo da Curva ROC e pontuação AUC
 
9. Novo Modelo de Logistic Regression

    9.1 Cálculo da Curva ROC e pontuação AUC

10. Modelo XGBoost

    10.1 Cálculo da Curva ROC e pontuação AUC

11. RandomSearchCV para o modelos selecionado
    
    11.1 Nested Cross Validation
    
12. Segunda Conclusão
13. Cálculo Pontuais
