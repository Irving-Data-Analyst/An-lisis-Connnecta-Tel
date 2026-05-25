# An-lisis-Connnecta-Tel

En este análisis identificaremos los clientes de mayor uso de la línea, segmentándolos por edades 

Ocupé tres data sets para hacer esta evaluación de clientes; fueron 'plans.csv', 'users_latam.csv' y 'usage.csv' (descárgalos)
plans: https://drive.usercontent.google.com/download?id=17Mkcs9rRWwiC_gaqVBYuFieON7s9v7Bn&export=download&authuser=0
users_latam: https://drive.usercontent.google.com/download?id=17wuqxalUsUnw9PXvCN2_UaAz6xeS9B0T&export=download&authuser=0
usage: https://drive.usercontent.google.com/download?id=11T8MQf-ouxJu9tia4F8aNpY7M_fb9O4h&export=download&authuser=0}

Una vez descargados los archivos, copia la dirección de descarga en el código de carga/lectura, hecho estos pasos, puedes ejecutar el código en Google colab y tendrás el código funcionando, aquí abajo detallo el procedimiento del análisls...


Primeramente hice un análisis exploratorio para validar nulos y sentineles, al mismo tiempo que identificaba los tipos de valores de cada columna.

Posteriormente, eliminé una columna por tener mas de 80% de nulos (churn_date), imputé los sentineles en "age" por la mediana, y en "city" imputé el valor "?" por "NA".
Después conté la cantidad de llamadas y mensajes en total por cliente, cada categoría en una columna diferente, les cambié el nombre a dichas columnas para una mejor lectura y comprensión, hice un "outer join" con el dataframe "users". Seguido de eso, imprimí histogramas para visualizar gráficamente el número de llamadas y mensajes.

Después identifiqué outliers y los viauslicé mediantes "boxplots" para determinar qué hacer con ellos, solamente capé los valores extremos de la columna "cant_minutos_llamada", porque son valores posibles pero muy alejados del límite superior.

Finalmente filtré por "edad" y por "uso" para etiquetar a cada segemento correspondiente de clientes.
Grafiqué dichos segmentos con gráfica de barras, para entender mejor visualmente los resultados, así identificando el segmento por uso y semgmento por edad
