# An-lisis-Connnecta-Tel

En este análisis identificaremos los clientes de mayor uso de la línea, segmentándolos por edades 

Ocupé tres data sets para hacer esta evaluación de clientes; fueron 'plans.csv', 'users_latam.csv' y 'usage.csv'

Primeramente hice un análisis exploratorio para validar nulos y sentineles, al mismo tiempo que identificaba los tipos de valores de cada columna.

Posteriormente, eliminé una columna por tener mas de 80% de nulos (churn_date), imputé los sentineles en "age" por la mediana, y en "city" imputé el valor "?" por "NA".
Después conté la cantidad de llamadas y mensajes en total por cliente, cada categoría en una columna diferente, les cambié el nombre a dichas columnas para una mejor lectura y comprensión, hice un "outer join" con el dataframe "users". Seguido de eso, imprimí histogramas para visualizar gráficamente el número de llamadas y mensajes.

Después identifiqué outliers y los viauslicé mediantes "boxplots" para determinar qué hacer con ellos, solamente capé los valores extremos de la columna "cant_minutos_llamada", porque son valores posibles pero muy alejados del límite superior.

Finalmente filtré por "edad" y por "uso" para etiquetar a cada segemento correspondiente de clientes.
Grafiqué dichos segmentos con gráfica de barras, para entender mejor visualmente los resultados, así identificando el segmento por uso y semgmento por edad
