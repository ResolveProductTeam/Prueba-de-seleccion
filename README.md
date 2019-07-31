# Prueba de selección
![](https://media.licdn.com/dms/image/C4D0BAQGkEgvEjR4KAA/company-logo_200_200/0?e=2159024400&v=beta&t=mvyJ3YPQksA6rjoxotFGcbfDQrxbq5t6a2qYWPg6Hb8)
En el presente repositorio encontrará todos los detalles sobre la prueba de selección para el cargo de **Científico de datos**, por favor tenga muy presente las instrucciones.

El objetivo de la prueba va en dos vías:

* Determinar sus *skills* en análisis de la información y proponer que  modelos de machine learning va  a utilizar.
* Conocer su desarrollo en la construcción de los modelos de machine learning

Por lo tanto en el desarrollo de la misma, por favor escriba brevemente la justificación de lo que considero adecuado.

# Parámetros de la prueba 

* Se debe desarrollar en Python
* Use Jupyter Notebook como script para la misma
* Divida la prueba en cuatro partes
  + Análitica de datos: Análisis Exploratorio de Datos
  + Cruce de bases de datos : Recuerde que solo puede usar Python, pero puede invocar una API para utilizar la herramienta que considere necesaria
  + Desarrollo del modelo ML (clasificador), bajo el algoritmo que considere necesario (Justifique porque se decidió por el mismo)
  + Genere un formato de entrega de las **principales conclusiones** del mismo (se recomienda un Dashboard dentro del mismo notebook).
  
  Teniendo en cuenta lo anterior, por favor a la hora de enviar o subir la prueba dividalo en scripts individuales para los pasos antes mencionados.
  
## Descripción del dominio del negocio

Se recolectaron datos correspondientes a campañas publicitarias en medios Digitales y ATL. El objetivo es a partir de estos , lograr atribuir como las campañas  tuvieron impacto en las decisiones de compra de los usuarios que visitaron las páginas (sitios web) de la compañia.

Los datos se recolectaron desde diferentes fuentes que brindan la siguiente información:



 
|Archivo    | Descripción           | Fuente                           |
| -------- | ---------------------- | ---------------------------------- |
| [Analítica](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Analitica.xlsx)| Trae la información general sobre las campañas | [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_ |
| [Interacciones](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Clasificacion.xlsx) | Contiene los datos generales del comportamiento de cada usuario| [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Demografía](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Demografia.xlsx) | Contiene  información adicion  del comportamiento del cada Usuario dado su localización geografíca | [Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Parrilla](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Parrilla.xlsx) |Contiene la información sobre la pauta y medios de comunicación|[Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|
| [Conversiones](https://github.com/ResolveProductTeam/Prueba-de-seleccion/blob/master/Data/Participaciones.xlsx) |Contiene la información sobre el total de conversiones sobre la pauta dada la fecha|[Daniel Jiménez](danieljimenezm.com); _Resolve Studio_|

# Diccionario de variables 
## Analítica
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Contenido | Nombre de la pauta    |chr |
|Campaña   | A que cretividad pertenece| chr|
|Conversion| El total de individuos que compran el **contenido** gracias a la campaña| num|
|Fecha     | La fecha en que se realizo la pauta | Date|
|Medio     |Por cual medio aparecio la pauta| factor|
|Source    |Nombre del medio en que aparecio la pauta |factor|

## Demografía
|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Browser   |Tipo de navegador por usuario|factor|
|Ciudad    |Ciudad de la que viene el usuario|factor|
|Fecha     |Fecha en que se conecto el usuario| Date|
|Device    |Tipo de dispositivo|chr|
|Sistema Operativo| Sistema Operativo del Usuario|factor|
|Sesión| El número de veces que se conecto el usuario| num|
|Duración| El tiempo que diro la pauta|Date|
|Tiempo en Página| Duración del usuario en la página web|Date|

## Parrilla

|Archivo    | Definición           |Tipo|
|----------|-----------------------|----|
|Channel| Canal en que se dio la pauta| factor|
|End_date| Momento en que finalizó la pauta| Date|
| Formato| Describe el tipo de formato|levels
















