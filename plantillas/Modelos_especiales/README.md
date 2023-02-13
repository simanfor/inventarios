<h1><center>Plantillas de inventarios para modelos especiales de</center></h1>
<center>
<img src="https://raw.githubusercontent.com/simanfor/web/main/logos/simanfor.png" alt="simanfor" width="350"/>
</center>


---

Esta carpeta contiene plantillas de inventario en un formato legible por SIMANFOR. Contenido
* Cladanifer_plantilla_inventario: plantilla de inventario de datos para el modelo *Cladanifer_stand__zam__v01*. Para utilizarla has de cubrir únicamente la hoja 'Parcelas' (no elimines la hoja 'PiesMayores'), cubriendo las 7 primeras columnas, donde:
  - TR: Variable dummy (igual a 1 si el matorral fue desarrollado en una zona quemada e igual a 0 si fue desarrollado en una zona desbrozada)  
  - TIME_AT: Tiempo tras el tratamiento de desbroce o quema prescrita (años)  
  
  Las restantes columnas hacen referencia a variables que necesita el modelo, y se calcularán de manera automática a partir de las variables con fondo amarillo, donde:  
  - P_: hace referencia a precipitación del mes que le sigue (mm)
  - T_: hace referencia a la temperatura media del mes que le sigue (ºC)
  - TMIN_: hace referencia a la temperatura mínima del mes que le sigue (ºC)
  - TMMIN_: hace referencia a la temperatura mínima promedio del mes que le sigue (ºC)
  

* Mixtos-plantilla_inventario: plantilla de inventario de datos para el modelo *PnigraPsylvestris_mix__es__v01*. Para utilizarla has de cubrir los campos que encontrarás en las hojas 'Parcelas' y 'PiesMayores'. Encontrarás una explicación de las variables nuevas en la hoja 'Metadatos', explicada a continuación:

  - ID_SP1: Código identificador de la especie 1 en masas mixtas, según el criterio del IFN (Inventario Forestal Nacional (España)). La especie 1 debe correspondense con la primera especie enunciada en el nombre del modelo
  - ID_SP2: Código identificador de la especie 2 en masas mixtas, según el criterio del IFN (Inventario Forestal Nacional (España)). La especie 2 debe correspondense con la segunda especie enunciada en el nombre del modelo
  - MARTONNE_1: Índice de Martonne, calculado para el momento 1. Se aplicará sobre los cálculos del modelo desde el inicio de la simulación hasta el año 2020
  - MARTONNE_2: Índice de Martonne, calculado para el momento 2. Se aplicará sobre los cálculos del modelo desde el año 2020 hasta el año 2040
  - MARTONNE_3: Índice de Martonne, calculado para el momento 3. Se aplicará sobre los cálculos del modelo desde el año 2040 hasta el año 2060
  - MARTONNE_4: Índice de Martonne, calculado para el momento 4. Se aplicará sobre los cálculos del modelo desde el año 2060 en adelante

  *Nota*: si no quieres que se modifique el Índice de Martonne durante la simulación, introduce el mismo valor en las 4 columnas.
