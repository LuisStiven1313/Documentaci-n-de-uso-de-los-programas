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



