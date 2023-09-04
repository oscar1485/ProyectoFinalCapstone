# Análisis de Accidentes de Tránsito en Bucaramanga

## Descripción del Proyecto

El objetivo principal de este proyecto es analizar y comprender los patrones de accidentes de tránsito en la ciudad de Bucaramanga. Para lograrlo, utilizamos un conjunto de datos que registra la ubicación de accidentes de tránsito en la ciudad. Nuestro análisis de estos datos nos permitió identificar áreas problemáticas, factores de riesgo y tendencias que contribuyen a la ocurrencia de accidentes. Además, buscamos desarrollar recomendaciones y estrategias para mejorar la seguridad vial y reducir la frecuencia y gravedad de los accidentes.

## Datos Utilizados

Los datos utilizados en este proyecto se obtuvieron de la plataforma del gobierno colombiano Datos Abiertos, específicamente en la dirección [Accidentes de Tránsito en Bucaramanga](https://www.datos.gov.co/Transporte/03-ACCIDENTES-DE-TRANSITO-DESDE-ENERO-2012-A-FEBRE/7cci-nqqb). Este conjunto de datos contiene información detallada sobre los accidentes de tránsito en Bucaramanga, incluyendo la ubicación geográfica, fecha y hora, condiciones climáticas, tipo de vehículos involucrados, causa probable del accidente y otros detalles relevantes.

## Metodología

El proyecto siguió una metodología que abarcó varios pasos clave:

1. **Carga de Datos**: Se cargaron los datos desde un archivo CSV utilizando la biblioteca pandas, centrándonos en las coordenadas de latitud y longitud.

2. **Preprocesamiento de Datos**: Se seleccionaron las características relevantes para el clustering, como las coordenadas de ubicación, y se estandarizaron para asegurar una escala consistente.

3. **Determinación del Número Óptimo de Clústeres**: Utilizamos el método del codo para determinar el número óptimo de clústeres para el algoritmo KMeans.

4. **Agrupamiento con KMeans**: Aplicamos el algoritmo KMeans con el número óptimo de clústeres para categorizar las ubicaciones de los accidentes.

5. **Visualización de Resultados**: Generamos un mapa interactivo y diagramas de dispersión para visualizar los resultados del agrupamiento.

6. **Modelado de Clasificación con CatBoost**: Exploramos modelos de clasificación para predecir la gravedad de los accidentes basados en diversas características.

## Resultados

Los resultados destacaron patrones geográficos de accidentes en Bucaramanga y permitieron prever la gravedad de los accidentes en función de características específicas. Sin embargo, es esencial considerar la calidad de los datos y las limitaciones del enfoque elegido al interpretar los resultados.

## Enlaces Útiles

- [Mapa Interactivo de Clustering](https://oscar1485.github.io/ProyectoFinalCapstone/bucaramanga_clusters_map.html)
- [Informe del Trabajo](https://github.com/oscar1485/ProyectoFinalCapstone/blob/main/INFORME.pdf)
- [Conjunto de Datos con Coordenadas](https://github.com/oscar1485/ProyectoFinalCapstone/blob/main/barrios_con_coordenadas.csv)
- [Conjunto de Datos Preprocesado](https://github.com/oscar1485/ProyectoFinalCapstone/blob/main/barrios_con_coordenadas_prepocesado.csv)
- [Fuente del Dataset Original](https://www.datos.gov.co/Transporte/03-ACCIDENTES-DE-TRANSITO-DESDE-ENERO-2012-A-FEBRE/7cci-nqqb)

Este proyecto ofrece una visión detallada de los accidentes de tránsito en Bucaramanga y puede servir como base para futuras investigaciones y acciones en la mejora de la seguridad vial en la ciudad.
