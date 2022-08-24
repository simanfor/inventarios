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
