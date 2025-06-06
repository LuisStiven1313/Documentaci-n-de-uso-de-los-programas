PROGRAMA CON FORMULAS EXACTAS

Este programa funciona de la misma manera tanto para modelos determinísticos como probabilísticos. Sin embargo, la mecánica del programa se explicará utilizando modelos determinísticos como ejemplo.
El primer paso en el desarrollo del programa fue traducir toda la lógica y las fórmulas matemáticas del libro a código en Python. Cada modelo determinístico cuenta con sus propios fragmentos de código y métodos de cálculo, como se muestra en las imágenes.

![Imagen1](https://github.com/user-attachments/assets/3eb93166-94e7-47f5-a6a0-d16dadc15e00)

![Imagen2](https://github.com/user-attachments/assets/82e7429e-82cf-419d-9af0-01bc66bd8abf)

Una vez traducida toda la lógica a código para cada modelo, se procedió a unificar todos ellos en un solo programa de selección de modelos. Este programa unificado contiene todos los modelos desarrollados.
El funcionamiento del programa consiste en seleccionar un modelo específico para realizar los cálculos correspondientes, que en la mayoría de los casos incluyen el cálculo del punto de reorden y la cantidad a pedir. Para ilustrar su funcionamiento, se utiliza como ejemplo el modelo EOQ.
El primer paso es seleccionar, entre todas las opciones disponibles, el modelo que se desea calcular.

![Imagen3](https://github.com/user-attachments/assets/452682bd-1936-4748-89ef-0dc69a303ca5)

Una vez seleccionado el modelo, el programa solicitará que se ingresen los parámetros necesarios para calcular el punto de reorden y la cantidad a pedir.

![Imagen4](https://github.com/user-attachments/assets/17d3bb96-34d8-4413-a7f9-123faabda954)

Una vez establecidos los valores de los parámetros para el modelo seleccionado, el programa realizará internamente el cálculo exacto de la cantidad a pedir y el punto de reorden correspondiente.

![Imagen5](https://github.com/user-attachments/assets/fcb6e509-2863-4be5-a5cf-1c0d5d332483)

Una vez obtenidos los resultados del modelo seleccionado, el programa ofrece la opción de calcular otro modelo disponible entre las opciones.
Tanto el programa para modelos determinísticos como el de modelos probabilísticos funcionan de la misma manera: en cada caso, solicitan los parámetros específicos requeridos para el cálculo y entregan los resultados correspondientes a cada modelo.


PROGRAMA CON ARBOL DE DECISIÓN


El primer paso para utilizar el programa con árboles de decisión es crear una base de datos con la que el programa trabajará. Esta base de datos servirá como referencia para que el programa realice predicciones sobre los valores que se desean obtener.
En el caso del modelo determinístico EOQ, se creó una base de datos con 10,000 registros. Esta base debe incluir tanto los parámetros utilizados para el cálculo como los resultados obtenidos a partir de dichos parámetros. Es fundamental que la base de datos sea lo suficientemente completa y representativa para garantizar un buen desempeño del modelo.
Una vez creada, el primer paso operativo es cargar la base de datos en el programa.

![Imagen6](https://github.com/user-attachments/assets/bc67f902-76d0-468b-80b2-b98a3a001b98)



Una vez establecida la base de datos con la que trabajará el programa, es necesario definir las variables de entrada y salida. Estas se seleccionan directamente de los datos contenidos en la base.
En el caso del modelo EOQ, las variables de entrada corresponden a los parámetros utilizados para el cálculo, mientras que las salidas pueden ser la cantidad a pedir o el punto de reorden, dependiendo de cuál sea el valor que se desea predecir.

![Imagen7](https://github.com/user-attachments/assets/5d32bd2d-d137-43f8-b561-b7f12a6b6e73)


Una vez definidas las variables de entrada y salida, el programa generará automáticamente el árbol de decisión y se entrenará utilizando la base de datos proporcionada. Durante este proceso, el modelo aprenderá a partir de los datos existentes para posteriormente, tomando como referencia ese aprendizaje, predecir la salida correspondiente a nuevos valores de los parámetros. En este caso, la salida a predecir sería la cantidad a pedir.

![Imagen8](https://github.com/user-attachments/assets/7b83cd14-ab42-43ee-b4e6-1938872e04cf)

Por último, una vez que el árbol de decisión ha sido creado y entrenado automáticamente por el programa, solo queda ingresar los valores de los parámetros deseados, respetando el mismo orden en que se definieron las variables de entrada. El programa, a partir de estos nuevos valores, realizará la predicción de la cantidad a pedir de forma automática.

![Imagen9](https://github.com/user-attachments/assets/7b0ddaee-a7ad-4d67-922b-e3db5196587d)

El procedimiento funciona de la misma manera para todos los modelos; la única diferencia radica en los parámetros que deben ingresarse como variables de entrada. Si se desea calcular el punto de reorden en lugar de la cantidad a pedir, basta con cambiar la variable de salida en el programa. En ese caso, el modelo se entrenará nuevamente, esta vez utilizando el punto de reorden como salida a predecir.

PROGRAMA CON REDES NEURONALES


El programa de redes neuronales funciona de manera similar al programa basado en árboles de decisión, con la diferencia de que, en lugar de trabajar directamente con entradas y salidas, opera mediante neuronas que procesan la información.
Al igual que el modelo anterior, este programa utiliza una base de datos para realizar sus predicciones. El primer paso consiste en cargar dicha base de datos en el programa. Para ilustrar su funcionamiento, nuevamente se utilizará el modelo EOQ como ejemplo.


![Imagen10](https://github.com/user-attachments/assets/1b3ef0ee-7ef7-4c5f-b26a-21f9813162e8)

A continuación, se deben definir las neuronas de entrada, que en este caso corresponden a los parámetros del modelo EOQ, y las neuronas de salida, que representan la variable que se desea predecir. En este ejemplo, la salida será la cantidad a pedir.

![Imagen11](https://github.com/user-attachments/assets/40698f07-3991-45d0-9dbf-17ec4929dec1)


Una vez definidas las neuronas de entrada y salida, el programa procede a construir la red neuronal, comenzando con una capa densa de 32 neuronas. A partir de allí, inicia el proceso de entrenamiento utilizando validación cruzada para aprender a partir de la base de datos proporcionada. Este entrenamiento se lleva a cabo durante 1,000 ciclos (épocas), optimizando progresivamente la precisión del modelo en la predicción de la cantidad a pedir.

![Imagen12](https://github.com/user-attachments/assets/4d12fbb9-4edb-475d-932d-46a613dda7c8)


Una vez que la red neuronal ha sido compilada y entrenada, el procedimiento es similar al del programa basado en árboles de decisión: se ingresan los valores de los parámetros como neuronas de entrada, y el programa, utilizando el modelo previamente entrenado, predice la cantidad a pedir.
Este procedimiento es aplicable a todos los modelos; la única diferencia radica en los parámetros específicos que se deben ingresar como neuronas de entrada. Si en lugar de la cantidad a pedir se desea predecir el punto de reorden, basta con cambiar la variable de salida. El programa volverá a entrenarse, esta vez utilizando el punto de reorden como salida a predecir.


![Imagen13](https://github.com/user-attachments/assets/65749eca-b32c-4536-9651-a911a71c718c)

