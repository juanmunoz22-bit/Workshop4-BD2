# Workshop4-BD2

# Integrantes
Juan Pablo Muñoz
Raúl Gonzalez
Jeisson Jossa
Moisés Salcedo

# Desarrollo y solución

INTRODUCCIÓN
Para el desarrollo del taller número 4 optamos por hacer uso de Big table desde Python. Una de las razones de usar python es para poder utilizar la libreria de pandas, la cual permite trabajar fácilmente los datasets. 

DESARROLLO

# Lectura ficheros, creación de familias de columnas, conexión y escritura en Big Table
Para esto ejecutamos la siguiente línea
![image](https://user-images.githubusercontent.com/53981601/138381464-e73f0535-3339-4b8e-8ede-59418c749be4.png)

Luego importamos todas las librerias necesarias para ejecutar el programa 
![image](https://user-images.githubusercontent.com/53981601/138381521-4559920d-32fe-4fd0-adb1-c51f91f3f7d2.png)

Luego instanciamos la base de datos, creamos las tablas necesarias e iniciamos la conexión. Al tener la oportunidad de usar gratis el crédito de google Cloud creamos una nueva base de datos de Big Table. Es por esta razón que el jason de conexión es diferente al de la clase. Creamos las tablas TABLE_WEATHER_ID la cual usamos para el punto 1, eta tabla va a contener los datos del fichero Plant_2_Weather_Sensor_Data.csv, despues creamos otra tabla TABLE_GENERATION_ID, la cual va a contener todos los valores del fichero Plant_1_Generation_Data.csv, el cual usamos para resolver el punto 2
![image](https://user-images.githubusercontent.com/53981601/138381910-c418966e-40cd-40c0-8c46-610e26d453e8.png)

Creamos las familias de tablas a usar y cargamos los ficheros con pandas.
![image](https://user-images.githubusercontent.com/53981601/138382620-6cd3c53c-f71d-4324-8ad0-3e6882cba3fa.png)

Escribimos la información en la tabla TABLE_WEATHER_ID
![image](https://user-images.githubusercontent.com/53981601/138382392-87c4f193-8563-4cb3-81a4-65d7ccb7657f.png)

Escribimos la información en la tabla TABLE_GENERATION_ID
![image](https://user-images.githubusercontent.com/53981601/138382695-b531ea5b-1186-495f-b95f-df45b4e79e13.png)

# Punto 1
Para resolver el punto 1 procedemos a hacer la búsqueda en Big Table por medio del jey indentificador, dando como key inicial el valor de la planta con la hora de 6 am y el jey final con el identificador de la planata y la hora del medio día, de forma que nos arroje los valores de temperatura en estas horas. Adempas creamos el filtro para mostrar solo la temperatura y aplicamos dicho filtro
![image](https://user-images.githubusercontent.com/53981601/138383411-900cd8b2-b680-49de-a44b-3122779e4ecc.png)

# Punto 2
Para resolver el punto 2, hacemos una búsqueda por key y hora, y tomamos el daily yield haciendo uso de filtros para mostrar la respuesta
![image](https://user-images.githubusercontent.com/53981601/138383533-25f889f3-170a-4e4a-9394-2e36c94ee195.png)

CONCLUSIÓN 
Hacer uso de una base de datos diferente, y de librerias en python a la que no estamos acostumbrados nos permite agregar nuevas herramienta de trabajo a las que tenemos, de esta forma se pueden construir apliacciones con más recursos y dependiendo de las necesidades podemos usar diferentes tipos de bases de datos. El hacer uso de python y de pandas nos ha facilitado trabajar con data frames con una cantidad considerable de registros, y esto también puede ayudarnos en la línea de Big Data en el futuro.



