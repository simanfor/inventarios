<h1><center>Plantillas sencillas de inventarios para</center></h1>
<center>
<img src="https://raw.githubusercontent.com/simanfor/web/main/logos/simanfor.png" alt="simanfor" width="350"/>
</center>


---
Esta carpeta contiene plantillas de inventario sin datos, con los encabezados necesarios para que sean entendibles por SIMANFOR. 

Para la mayoría de modelos, rellenar los campos de estas plantillas es suficiente, no obstante, echa un vistazo a las recomendaciones de uso del modelo a utilizar en su correspondiente [ficha](https://github.com/simanfor/modelos) para saber si necesita información adicional. 

Los campos que se incluyen en ellas son:

*   La hoja "Parcelas" hace referencia a la información de la parcela, donde tendrás que cubrir:  
  
  * ID_Inventario: identificador de inventario, puedes poner la fuente de donde has obtenido los datos (OJO, los árboles de la parcela deben llevar el mismo código)
  * ID_Parcela: identificador de parcela, en donde debes poner un código numérico (no te líes, sirve con 1, 2, 3...) (OJO, los árboles de la parcela deben llevar el mismo código)
  * ID_especie_principal: es el código de referencia que corresponde a la especie principal de la parcela según el Inventario Forestal Nacional. Puedes consultarlo en la página 24 del [documentador del IFN3](https://www.miteco.gob.es/es/biodiversidad/servicios/banco-datos-naturaleza/documentador_bdcampo_ifn3_tcm30-282240.pdf).
  * T: edad promedio de la parcela (años)
  * N: densidad de la parcela (pies/ha)
  * G: área basimétrica de la parcela (m2/ha)
  * Ho: altura dominante de la parcela (m). Puedes calcularla haciendo el promedio de la altura de los 100 árboles más altos por hectárea (ordena los árboles de mayor a menor altura, y ten en cuenta que cada árbol representa a un nº de árboles determinado a nivel de parcela (factor_expansion); suma el factor de expansión hasta llegar a tener los 100 primeros árboles más altos y haz el siguiente cálculo:  
  
		              (factor_expansion_1·h_1 + factor_expansion_2·h_2 + ... + factor_expansion_n·h_n)/100  
      
* La hoja de "PiesMayores" hace referencia a la información sobre los árboles de la parcela, donde tendrás que cubrir:  

  * ID_Inventario: el mismo código de la parcela a la que pertenece el árbol  
  * ID_Parcela: el mismo código de la parcela a la que pertenece el árbol  
  * ID_arbol: identificador numérico único del árbol dentro de la parcela (no te líes, sirve con 1, 2, 3...)  
  * factor_expansion: es el número de árboles al que representa el árbol sujeto a nivel de hectárea. Se calcula así: (10.000 m2) / (superficie parcela en m2)  
  * dbh: diámetro del árbol (cm)  
  * h: altura del árbol (m) 
  
