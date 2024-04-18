# Classificação de pontuação de crédito

Neste projeto, utilizei um dataset de pontuação de crédito disponível no Kaggle, onde cada cliente é classificado em três categorias:

* Bom.
* Regular.
* Ruim.

Comecei com a parte de tratamento dos dados, seguindo os passos:

* Identificação de tipos de variáveis não adequados.
* Remoção de colunas irrelevantes.
* Padronização dos dados faltantes: todos foram preenchidos com NaN.
* Tratamento dos dados faltantes ou problemáticos em cada coluna em que tais problemas foram identificados. Os dados faltantes foram preenchidos usando ffil.
* Em algumas variáveis, foi feita uma visualização dos dados por meio de box-plots ou histogramas.

Em seguida, avaliei quais variáveis deveriam ser incluídas nos modelos de Machine Learning, por meio de um heatmap com as correlações das variáveis. Após escolhidas as variáveis que entrariam no modelo, foi feita uma divisão da base em treino, teste e validação. O passo seguinte foi a aplicação de dois modelos:

* Random Forest.
* Gradient Boosting.

Para ambos os modelos foi feito um método de grid search, onde buscamos descobrir os melhores hiperparâmetros. Vimos que era interessante adicionar mais variáveis ao modelo a fim de melhorar a acurácia das previsões. O último passo foi fazer uma cross-validation, buscando aumentar a acurácia das previsões sem aumentar tanto o número de estimadores dos modelos.
