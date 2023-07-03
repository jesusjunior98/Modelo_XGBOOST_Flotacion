# Modelo_XGBOOST_Flotacion
Modelo de regresión XGBOOST para predecir la ley de Cobre en un proceso de Flotación

MARCO TEÓRICO

En la industria minera, para la obtención de concentrados de gran valor agregado a partir de los minerales que encontramos en la corteza terrestre, es necesario tres etapas en todo el proceso productivo, las cuales son: exploración, extracción y procesamiento. La etapa de procesamiento de minerales es donde bajo diversas operaciones unitarias que incluyen métodos físico-químicos se logra obtener un concentrado de alta pureza para su posterior refinamiento y obtener los diversos metales que son indispensables en nuestras vidas.

FLOTACIÓN DE MINERALES

Una operación unitaria que es indispensable en casi toda unidad minera es la flotación de minerales, la cual permite lograr una separación de los minerales valiosos y de los no valiosos, aprovechando las propiedades hidrofóbicas de los mismos. Es decir, en una celda de flotación se provee aire para generar burbujas y los minerales dependiendo de la propiedad mencionada se adhieren a las burbujas o no. La flotación de minerales es un proceso complejo que involucra diversas variables para obtener los mejores resultados.

Indicadores de eficiencia en la Flotación:

-La ley y recuperación son indicadores relativos del rendimiento en el proceso de flotación.

-La ley es el contenido del mineral valioso en el concentrado.

-La recuperación  hace referencia al porcentaje en peso del total de mineral que se obtuvo en el concentrado.

XGBOOST

XGBoost (Extreme Gradient Boosting), es uno de los algoritmos de machine learning de tipo supervisado más usados en la actualidad. XGBoost Extreme Gradient Boosting es un algoritmo predictivo supervisado que utiliza el principio de boosting. La idea detrás del boosting es generar múltiples modelos de predicción “débiles” secuencialmente, y que cada uno de estos tome los resultados del modelo anterior, para generar un modelo más “fuerte”, con mejor poder predictivo y mayor estabilidad en sus resultados. Para conseguir un modelo más fuerte a partir de estos modelos débiles, se emplea un algoritmo de optimización, este caso Gradient Descent (descenso de gradiente). Durante el entrenamiento, los parámetros de cada modelo débil son ajustados iterativamente tratando de encontrar el mínimo de una función objetivo, que puede ser la proporción de error en la clasificación, el área bajo la curva (AUC), la raíz del error cuadrático medio (RMSE) o alguna otra. 
Cada modelo es comparado con el anterior. Si un nuevo modelo tiene mejores resultados, entonces se toma este como base para realizar modificaciones. Si, por el contrario, tiene peores resultados, se regresa al mejor modelo anterior y se modifica ese de una manera diferente. Qué tan grandes son los ajustes de un modelo a otro es uno de los hiper parámetros que debe definir el usuario.
Este proceso se repite hasta llegar a un punto en el que la diferencia entre modelos consecutivos es insignificante, lo cual nos indica que hemos encontrado el mejor modelo posible, o cuando se llega al número de iteraciones máximas definido por el usuario.
