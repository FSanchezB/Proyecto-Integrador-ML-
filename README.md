Este repositorio es un proyecto de machine learning que toma un dataset con varios features de pacientes hospitalizados o no hospitalizados, y clasifica a los pacientes conforme a si seran o no hospitalizados.
Se inicia con un analisis exploratorio de los datos y despues con la limpieza, al ser pocos los valores nulos se aplica un dropna(), ya que se perdia un porcentaje muy pequeño de la información.
Se seleccionan los mejores features con el criterio del data scientist por medio de visualizaciones como una matriz de correlación aplicada solo al target y con metodos como SelectKBest de sklearn, dando un resultado bastante parecido entre ambos metodos
de un total de 5 features.
Se alimentan los datos a modelos de árbol y KNN, para despues aplicar GridSearch para encontrar los mejores parametros que resultaron ser unos bastante eficientes en cuánto al costo computacional.
Ambos modelos resultaron con un F1 sorprendente de 1 con Max Depth de 2 o en caso de KNN, 2 vecinos.
Faltaría probar con 4 o tal vez 3 features si se mantiene el score de 1.0 para mejorar la eficiencia.
