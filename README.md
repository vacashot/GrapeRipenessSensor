### Prototipo de control de la madurez de la uva mediante sensor espectral e inteligencia artificial:

La utilización de técnicas de inteligencia artificial puede ser muy útil en la viticultura para determinar el momento óptimo de la vendimia. En este trabajo, se plantea el diseño de un prototipo que utiliza un sensor espectral de bajo coste para medir el color de la uva. A partir de los datos obtenidos, se plantea un modelo de red neuronal artificial para predecir las fases de maduración. Esto permitiría tomar decisiones más precisas sobre cuándo recoger la uva para obtener las mejores características de la uva y del vino.
Se trata de un prototipo que aprovecha la inteligencia artificial (IA) para evaluar la madurez de la uva, un factor crucial en la toma de decisiones sobre el momento ideal para la vendimia. El dispositivo incorpora un sensor multiespectral de bajo coste con canales para el visible y el infrarrojo cercano. Este sensor se integra en una placa electrónica basada en Arduino, con capacidad  de procesamiento de los datos al borde de la red. Esto significa que el procesamiento de datos se realiza en el propio prototipo en lugar de enviar los datos a un servidor remoto para su procesamiento, permitiendo monitorizar la evolución en campo. El concepto clave detrás del prototipo se basa en que las estructuras moleculares de los compuestos responsables del cambio de color de la uva, reflejan longitudes de onda específicas durante su proceso de maduración. Estos cambios de color se producen de manera gradual a partir del envero en función de la presencia de compuestos fenólicos en la uva,  a medida que se produce un   aumento del contenido de azúcar y una disminución de la acidez. Para asignar a los resultados de color del sensor a un estado de maduración se utiliza un indicador de la madurez basado en la determinación de la concentración de azúcar (grado Brix). Una vez obtenido un conjunto de datos válidos de color, es posible construir y entrenar un modelo de  red neuronal artificial (ANN) para interpretar el color espectral de la uva con el fin de predecir las fases de maduración. La capacidad de realizar mediciones de la madurez de la uva en tiempo real, sin necesidad de realizar muestreos en campo puede ayudar a los viticultores y enólogos a mejorar la calidad de sus productos y a optimizar la vendimia.

![imagen_sensor](https://github.com/vacashot/GrapeRipenessSensor/blob/main/esquema_conexiones.png)

### Aspectos Innovadores:
1.	Uso de Sensores Multiespectrales de Bajo Coste: La incorporación de un sensor multiespectral de bajo coste con canales para el visible y el infrarrojo cercano. El objetivo de utilizar tecnología de bajo coste es mejorar la escalabilidad del producto.
2.	Procesamiento de Datos en el Borde de la Red (Edge Computing): La capacidad de procesar los datos directamente en el prototipo en lugar de enviarlos a un servidor remoto es una característica innovadora. Se trata de un nuevo paradigma de computación cuyo enfoque acerca el procesamiento y el almacenamiento de datos hasta los dispositivos que los generan. El objetivo de utilizar esta tecnología en el prototipo es eliminar la dependencia de servidores ubicados a miles de km de distancia, optimizando la tasa de transmisión de datos.
3.	Modelo de Red Neuronal Artificial (ANN): La utilización de un modelo de red neuronal artificial se utiliza para realizar tareas de aprendizaje automático, como clasificación, regresión, procesamiento de imágenes, procesamiento de texto. En el prototipo se utiliza para interpretar los datos espectrales del sensor y predecir las fases de maduración de la uva como enfoque innovador en la agricultura. Las ANN son capaces de aprender patrones complejos y pueden adaptarse a las variaciones en los datos, lo que hace que este enfoque sea poderoso y versátil.
4.	Monitorización en Tiempo Real (5G): La capacidad de realizar mediciones de la madurez de la uva en tiempo real, sin la necesidad de realizar muestreos manuales en el campo, es una innovación importante. Esto proporciona a los viticultores información en tiempo real sobre el estado de sus cultivos, lo que puede ayudar a tomar decisiones más precisas sobre el momento de la vendimia. La implementación de las comunicaciones 5G en este proceso es un aspecto especialmente innovador, ya que permite una transmisión de datos instantánea, de largo alcance, de bajo consumo y confiable desde los sensores en el viñedo.
5.	Optimización de la Calidad del Producto: La aplicación de la inteligencia artificial para evaluar la madurez de la uva tiene el potencial de mejorar la calidad de los productos vinícolas. Esto permite a los viticultores cosechar las uvas en el momento óptimo para obtener las mejores características de sabor y aroma en el vino.
6.	Seguridad alimentaria: El sensor, al detectar cambios en el color, podría potencialmente detectar el desarrollo de enfermedades que afecten la epidermis del ollejo, como el oidio o la botrytis, mejorando no sólo la calidad si no también la seguridad alimentaria.

![imagen_grape](https://github.com/vacashot/GrapeRipenessSensor/blob/main/Imagen%20de%20WhatsApp%202024-07-09%20a%20las%2014.44.46_d28408eb.jpg)

![imagen_sensorica](https://github.com/vacashot/GrapeRipenessSensor/blob/main/20240709_135442.jpg)

![imagen_completinstalation](https://github.com/vacashot/GrapeRipenessSensor/blob/main/20240709_135456.jpg)

### PROTOCOLO PARA TOMA MUESTRAS
1. Muestras de tempranillo. Parte media del racimo, todas del mismo color y en buen estado sanitario
2.  Entre 5 y 10 muestras por día
3.  Cada muestra es un bulk de 10 bayas ( se ira reduciendo el número de bayas, para cubrir el mosto con el refractómetro, lo ideal una baya una medida con el refráctometro)
4.  Primero se realizan las medidas con el sensor y despues con el Refráctometro
5.  Para identificar las muestras utilizamos el ID de ZZZ/XX/YY:  ZZZ= numero de muestras (0-999) / XX= número de bulk (5-10)/ YY= número de baya (1-10)
6.  Anotar el estado fenologico en el estadillo
### INSTRUCCIONES SENSOR 
1. INICIAMOS ARDUINO IDE
2. SELECCIONAMOS PLACA: ARDUINO UNO
3. PUERTO COM USB
4. ACTIVAMOS "MONITOR SERIAL"
5. SELECCIONAMOS 115200 bauds
6. SEGUIMOS INSTRUCCIONES EN PANTALLA
### PROTOCOLO MEDIDA CON SENSOR
1. Luz led a 5 de intensidad
2. En condicines de oscuridad, tapa cerrada y espuma de cable puesta
3. Si se repiten medidas se indica como ID ZZ/XX/YY/bis
4. Es importante que la baya este pegada al sensor a la misma distancia, y en el parte media de la baya

![imagen_instruccionesn](https://github.com/vacashot/GrapeRipenessSensor/blob/main/ITACyL_2024/instrucciones.JPG)
![imagen_instonesn](https://github.com/vacashot/GrapeRipenessSensor/blob/main/ITACyL_2024/estados_fenologicos_de_la_vid_1_20150202_1544847080.jpg)
