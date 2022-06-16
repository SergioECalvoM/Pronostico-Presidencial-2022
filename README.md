# Pronóstico-Presidencial-2022
Pronóstico de las elecciones presidenciales de Colombia 2022 utilizando ponderación de encuestas y simulación de Monte Carlo. Este repositorio hace parte del soporte para la participación del autor en el recetario abierto de https://www.recetas-electorales.com/. 

Se elabora un achivo de texto con nombre: EncuestasSV2022.txt que contiene información sobre los sondeos de intención de voto para la segunda vuelta de las elecciones presidenciales de 2022 en Colombia. El archivo corresponde a los datos de las encuestas públicas con tiempos de recolección posteriores a las consultas presidenciales del 13 de marzo de 2022 para escenarios de segunda vuelta entre los candidatos Gustavo Petro y Rodolfo Hernández, así como las encuestas posteriores a la primera vuelta del 29 de mayo de 2022.

Ahora bien, tomando como base el archivo de encuestas previamente descrito, se elabora un archivo de datos SerieTemporalSV2022.txt con las mismas columnas exceptuando Pollster, MoE, Source y Link. Posteriormente, se realiza para el caso de varias encuestas con la misma fecha, un promedio ponderado por el tamaño de muestra. Lo anterior garantiza que para cada fecha se obtenga un registro único que consiste de tamaño de muestra, proporción de la intención de voto para cada candidato, el voto en blanco, indecisos y aquellos que no planean votar por ninguna opción. Los cálculos pueden encontrarse en el archivo de Excel AjusteSV.xlsx.

El modelo fue elaborado en el paquete estadístico R en el archivo ScriptModeloSV2022.R.
