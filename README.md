# Prueba de selección
![](https://media.licdn.com/dms/image/C4D0BAQGkEgvEjR4KAA/company-logo_200_200/0?e=2159024400&v=beta&t=mvyJ3YPQksA6rjoxotFGcbfDQrxbq5t6a2qYWPg6Hb8)
En el presente repositorio encontrará todos los detalles sobre la prueba de selección para el cargo de **Científico de Datos**, por favor tenga muy presente las siguientes instrucciones.

El objetivo de la prueba es doble:

* Determinar sus *skills* en análisis de datos y aplicación de modelos de Machine Learning.
* Conocer sus capacidades en la construcción y validaciónde los modelos de Machine lLarning.

Por lo tanto en el desarrollo de la misma, por favor escriba brevemente la justificación de lo que consideró adecuado.

 
## Descripción del dominio del negocio

Se recolectaron datos correspondientes a campañas publicitarias en medios Digitales y ATL. El objetivo es a partir de estos lograr atribuir como las campañas tuvieron impacto en las decisiones de compra de los usuarios que visitaron las páginas (sitios web) de la compañia.

Los datos se recolectaron desde diferentes fuentes que brindan la siguiente información:


|Archivo (Haga click para descargar)   | Descripción           | Fuente                           |
| -------- | ---------------------- | ---------------------------------- |
| [Analítica](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Analitica.xlsx)| Trae la información general sobre las campañas | [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_ |
| [Interacciones](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Interacciones.xlsx) | Contiene los datos generales del comportamiento de cada usuario| [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Demografía](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Demografi%CC%81a.xlsx) | Contiene  información adicion  del comportamiento del cada Usuario dado su localización geografíca | [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Parrilla](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Parrilla.xlsx) |Contiene la información sobre la pauta y medios de comunicación|[Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Conversiones](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Participaciones.xlsx) |Contiene la información sobre el total de conversiones sobre la pauta dada la fecha|[Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|

# Diccionario de variables 

## Analítica
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Marca     | Nombre del anunciante    |chr |
|Campaña   | A que creatividad pertenece | chr|
|Conversion| El total de individuos que compran el **marca** gracias a la campaña| num|
|Fecha     | La fecha en que se realizó la pauta | Date|
|Medio     | Por cual medio apareció la pauta | Categorical|
|Fuente     | Origen de emisión de la pauta  | Categorical|

## Demografía
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Browser   | Tipo de navegador por usuario| Categorical |
|Ciudad    | Ciudad de la que viene el usuario| Categorical |
|Fecha     | Fecha en que se conecto el usuario| Date |
|Device    | Tipo de dispositivo|chr|
|Sistema Operativo| Sistema Operativo del Usuario| Categorical |
|Sesión| El número de veces que se conecto el usuario| num |
|Duración| El tiempo que diro la pauta|Date|
|Tiempo en Página| Duración del usuario en la página web| Date |

## Parrilla

|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Channel| Canal en que se dio la pauta| Categorical |
|End_date| Momento en que finalizó la pauta| Date|
|Formato| Describe el tipo de formato|levels|
|Inversión| El valor de la pauta dada la hora y día en que aparecio| num|
|Medium| Medio en que sale la pauta| Categorical |
|rating| Personas viendo la pauta dada la hora|num|
|Reference| Creatividad de la pauta|chr|
|Start_date| Fecha exacta en que comenzo la pauta| Date |


## Interacciones
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Promedio de duración| Tiempo del indiviuo viendo la pauta| num|
|Tiempo en página| Tiempo que duro el individuo en la web|num|
|ID| Identificación del usuario| Categorical |
|Fecha| Fecha en que e usuario vio la pauta|Date|
|Hora| Hora en que el usuario vio la pauta|Date|
|Minuto| Minuto en que el usuario vío la pauta|Date|


## Conversiones
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Campaña| Tipo ó clase de pauta| Categorical |
|Grupo| Franja horaria en la que se emitió el contenido  | Levels |
|Asistente| Agencia de publicidad que generó el contenido |num|
|Creatividad| Creatividad asociada a la pauta| Categorical |
|Número objetivo| Cantidad esperada conversiones|num|
|Fecha| Fecha de la pauta|Date|
|Medio| Asociación del medio en que aparecio dado el grupo de la pauta|num|
|Source| Código asociado a la pauta y creatividad | Levels |
|Total de conversiones| El total de conversiones dada la hora de la pauta y su creatividad| num |


# Parámetros de la prueba 

* Se debe desarrollar en Python.
* La prueba se divide en cuatro partes. Por favor desarrolle un script individual para cada una de ellas:
  + Análitica de datos: Análisis Exploratorio de Datos
  + Cruce de bases de datos: Recuerde que solo puede usar Python, pero puede invocar una API para utilizar las librerias/herramientas que considere necesarias.
  + Desarrollo del modelo ML (clasificador) que determine que medio y/o campaña tendrá mayor impacto en la conversión (decisión de compra) del usuario, bajo el algoritmo que considere mas adecuado (justifique porque se decidió por el mismo). Establezca así mismo un esquema apropiado de partición de datos para entrenamiento/prueba/validación, teniendo en cuenta que la empresa no cuenta con otro set de datos adicional.
  + Genere un formato de entrega de las **principales conclusiones** del mismo (se recomienda un Dashboard dentro del mismo notebook).
* Use Jupyter Notebook como entorno de solución. Los notebooks desarrollados deben ser enviados a la dirección de correo electrónico indicada.  




















