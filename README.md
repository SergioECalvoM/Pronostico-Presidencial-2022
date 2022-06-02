# Pronóstico-Presidencial-2022
Pronóstico de las elecciones presidenciales de Colombia 2022 utilizando ponderación de encuestas y simulación de Monte Carlo. Este repositorio hace parte del soporte para la participación del autor en el recetario abierto de https://www.recetas-electorales.com/. 

En el archivo DataColSV2022.xlsx se encuentra en la hoja "Polls" la tabla de información de cada encuesta publicada después de las consultas presidenciales del 13 de marzo de 2022. Por cada encuestada se tiene la información de: Nombre de encuestadora ("Pollster"); fecha mediana de muestreo ("Date"); margen de error ("MoE"); fuente ("Source"), enlace ("Link") y la intención de voto por los candidatos: Gustavo Petro y Rodolfo Hernández, así como el voto en blanco ("Blanco"), ninguno ("None") y no sabe no responde ("Uncertain"). 

En la segunda hoja del libro de excel, llamada "Rating" se encuentra por cada encuestadora su calificación ("Rating") basado en el semáforo de encuestadoras electorales en Colombia de La Silla Vacía (https://www.lasillavacia.com/historias/silla-nacional/el-semaforo-de-las-encuestadoras-electorales-en-colombia/). La tercera hoja, llamada "VeB" contiene un promedio del voto en blanco de los comicios de segunda vuelta presidencial entre 2002 y 2018 el cual será utilizado como estimación inicial de este valor, también se encuentra la fuente y enlace.

En el archivo ScriptSVCol22.R se utiliza el paquete tidyverse para generar los data frames que requiere el modelo y sus gráficas, este archivo está comentariado. Adicionalmente, añadimos una sección de código para obtener la precisión del pronóstico. El archivo DescripciónModelo.pdf contiene la descripción del modelo así como las referencias. 
