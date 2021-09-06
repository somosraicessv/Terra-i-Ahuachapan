# MAPEO DE COBERTURAS PARA EL AÑO 2018 EN EL DEPARTAMENTO DE AHUACHAPÁN, EL SALVADOR
Terra-i es un sistema de monitoreo de cambios en las coberturas vegetales y uso del suelo, integra diferentes metodologías y datos para crear un sistema robusto con tres niveles de análisis: 

 - un 1er  nivel, de alertas tempranas de cambios en la cobertura vegetal, con modelos calibrados a escala nacional, basado en redes neuronales y sensores remotos; 
 - 2do  nivel, de mapeo de coberturas y cuantificación de la pérdida de la cubierta forestal en áreas de interés usando sensores remotos y aprendizaje automático; y por último un 
 - 3er nivel, de validación de la precisión de los datos generados y la identificación de causas o motores de deforestación e historia de uso a partir de metodologías de validación en campo en zonas de interés, usando vehículos aéreos no tripulados.
## CIAT y RAÍCES

CIAT junto a CRS bajo el programa RAÍCES, han implementado Terra-i en el departamento de Ahuachapán, con el objetivo de realizar el mapeo de las coberturas de la tierra, el cual será empleado como insumo de línea base para el año 2018, con el objetivo de reconocer las  coberturas presentes en el área, usando imágenes de satélite y técnicas de aprendizaje automático, que permitan realizar un monitoreo de forma rápida y precisa.

## Mapa de coberturas Ahuachapán

El mapa de cobertura vegetal se desarrolló utilizando imágenes de satélite **_Sentinel 2_** para el **_2018_**, aplicando el método de clasificación no supervisada _**K-MEANS**_ y supervisada **_Random Forest_**, logrando con el modelo una precisión del **_95%_**. La precisión global y exhaustividad del mapa fue evaluada en una misión de campo recolectando imágenes de alta resolución a través de drones y un formulario en la aplicación móvil KoboCollect, alcanzando una precisión final del 87%.

El  mapa de cobertura vegetal tiene 15 clases, basadas en la clasificación  del mapa de cobertura del suelo del Ministerio del Medio Ambiente, que incluye: agua, bosque caducifolio, bosque de galería, bosque siempre verde, café, caña de azúcar, árboles frutales, bosque de mangle, palma oleífera, mosaico de pastos y cultivos, plantaciones forestales monoespecíficas, playa, suelo desnudo, urbano y vegetación secundaria.

La  metodología con la que se realizó el mapa de coberturas de la tierra en Ahuachapán para el año 2018, se basó en cuatro macro-procesos, descritos a continuación:

1.  Recopilación de datos de entrada, el cual incluye:
    
    -   Pre-procesamiento de la colección de imágenes satelitales Sentinel-2 para el año 2018.
        
    -   Análisis  de mapas de coberturas de la tierra previos para establecer las categorías a clasificar.
        
    -   Selección  de datos de entrenamiento del modelo, utilizando imágenes de muy alta resolución en Google Earth Pro para el 2018.
        
2.  Evaluación  y selección de algoritmos de aprendizaje automatizado:
    
    -   Aplicación  del algoritmo de clasificación no supervisada: **_K-means_**.
        
    -   Evaluación del rendimiento de algoritmos de clasificación supervisada, a través de validación: Máquina de Soporte Vectorial, Naive Bayes, **Random Forest** y Perceptrón Multicapa.
        
3.  Clasificación de coberturas de la tierra y post-proceso de clasificación:
    
    -   Clasificación de coberturas con el modelo **_Random Forest_**, que tuvo el mejor rendimiento en proceso de evaluación de algoritmos.
        
    -   Post-proceso  de clasificación, aplicando herramientas de generalización cartográfica, como: filtro mayoritario, refinado de límites y eliminación de pequeñas regiones aisladas.
        
4.  Validación del mapa se realizó a través de:
    
    -   Recolección de datos en campo con drones y formulario.
        
    -   Recolección  de datos de cobertura utilizando imágenes de Google Earth Pro (GEP) para el año 2018.
        
    -   Evaluación  del mapa de coberturas con datos información de campo e imágenes de GEP para definir precisión global, exhaustividad por categoría, y precisión por categoría.

El mapa fue generado a través de la plataforma libre Google Earth Engine (GEE). La colección del mapa final se encuentra disponible para acceder como un ASSET de GEE, sin necesidad de descargar los datos. Para acceder utilizar el siguiente ID en GEE:

-   Mapa de cobertura de la tierra, Ahuachapán El Salvador, 2018:
**ID: users/jorgeperez/coberturas_wgs84**
-   Mosaico  Imágen Sentinel 2, 2018:
**ID: users/jorgeperez/Salvador_CRS/composite**
![Metodología mapeo de cobertura de la tierra usando sensores remotos y algoritmos de aprendizaje automatizado.](https://www.arcgis.com/sharing/rest/content/items/a8f346a9cb424bbba83679a4e12659bc/resources/metodologia_SM_ultimo__1569273324546__w1448.png)
## Validación en campo mapa de coberturas

La evaluación de la precisión del mapa de cobertura de la tierra se realiza mediante la visita de 100 áreas de muestreo en el corredor de Raíces y el análisis de imágenes de alta resolución en el resto del departamento. La información recolectada es utilizada para mejorar la precisión del modelo de clasificación.

1.  Recolección  de datos en campo, en el corredor de RAÍCES, en los municipios de San Lorenzo, Ahuachapán, Atiquizaya, Ataco, Apaneca, Jujutla, Guaymango y San Pedro Puxtla, junto al personal local de Caritas y CRS.
    
	- Selección  de **464 puntos** de muestra a validar utilizando métodos de evaluación de precisión de mapas del IPCC, 2013 y Olofsson, et al, 2014.
	- Recolección  de imágenes de alta resolución, utilizando drones Phantom lll Advanced, Phantom IV y Mavic air, realizando  **95 vuelos de 6.25ha**.
    
	- Reconocimiento de coberturas de la tierra, utilizando formulario de campo con la aplicación KoboCollector, recolectando  **95 muestras**.
    
	- Procesamiento  de imágenes de alta resolución para la creación de ortomosaicos.
    
	- Identificación  y creación de base de datos de coberturas de la tierra, reconocimiento de ~500 muestras.
    
2. Identificación de cobertura de la tierra en imágenes de alta resolución, en el área de estudio restante del departamento, - _Ver en el mapa pestaña “Fotos Google Earth”_-.  

3. Creación  de matriz de confusión, cálculo de precisión global , exhaustividad y precisión por clase.

## Socialización de trabajo realizado por Terra-i en Ahuachapán con actores locales

El 7 de Junio en el Municipio de Ahuachapán se realizó la primera socialización del trabajo realizado por el equipo Terra-i, CIAT, en el que participaron actores locales de la Alcaldía de Ahuachapán, Unidades agrícolas de San Lorenzo, Atiquizaya, Grupo Gestor MARN, RAÍCES, Caritas, CIAT, Unidades ambientales, Protección civil de Apaneca, Jujutla, Ataco, Guaymango, Grupo Gestor. Con el objetivo de realizar las siguientes actividades:

1.  Socialización de Terra-i en Ahuachapán: Método, usos, resultados.
    
2.  Lluvia de ideas de las diferentes aplicaciones del mapeo de cobertura por los usuarios.

## Resultados de Socialización

Los  resultados de la lluvia de ideas presentadas por los actores locales del departamento de Ahuachapán, se describe en el siguiente diagrama, el cual presenta las diferentes aplicaciones que tiene el mapa de cobertura de la tierra realizado por Terra-i, clasificadas en tres temáticas de alta importancia:  **monitoreo**,  **toma de decisiones**  y  **análisis**, los cuales se relacionan entre sí.
## Agradecimientos

Este trabajo fue realizado por el Centro Internacional de Agricultura Tropical  [(CIAT)](https://ciat.cgiar.org/)  en colaboración con el Proyecto Raíces Ahuachapán y Catholic Relief Services ([CRS](https://www.crsespanol.org/)).

![](https://www.arcgis.com/sharing/rest/content/items/a8f346a9cb424bbba83679a4e12659bc/resources/Logos_story_salvador__1570201002250__w940.png)

**_Story map:_**
https://arcg.is/1GHbT5

**_Story map preparado por:_**
Jhon Jairo Tello, Paula Paz, Jorge Perez

**e-mail de autores:** [j.j.tello@cgiar.org](mailto:j.j.tello@cgiar.org), [p.a.paz@cgiar.org](mailto:p.a.paz@cgiar.org), [j.perez@cgiar.org](mailto:j.perez@cgiar.org).

**_Fotografías por:_**

_Equipo Terra-i CIAT_

_Proyecto Raíces Ahuachapán_
