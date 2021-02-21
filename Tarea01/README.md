# LMSGI / 
Curso Lenguaje de Marcas y Sistemas de Gestión de la Información / 
Estudiante y Autor: Pedro.J / 
Calificación: 6,60. / 
Observaciones: 
  Los documentos que habia que enviar se deben llamar: agenda.xml, recetas.xml y modulos.xml.
RECETA 
El enunciado dice “la información de las recetas de un restaurante y aplicarlo a la siguiente receta de cocina”. Ante esto, cabe pensar que en este documento podrán existir más de una receta. En conclusión el elemento raíz se llamaría recetas y dentro de él las diferentes recetas en un elemento llamado receta.
Si un elemento está estrechamente unido con otro, es decir que si modifico uno se modifica el otro no se aconseja ponerlo cómo atributo. Si sabemos que la unidad va a modificar a la cantidad, es decir no es lo mismo 250 gr. que 250 ml., se aconseja como elemento uno y el otro que modifica como atributo.

MÓDULO 
El nombre en el DOCTYPE tiene que coincidir con el elemento raíz.
Toda la información referente a módulos y alumnos está dentro del elemento módulo y a su vez dentro del elemento ciclo.
El elemento tiempo se llamaría horas_semanales y su contenido sería 4.
Según las especificaciones del enunciado se pretenden realizar los documentos dando prioridad a la claridad y a la estructura por lo que todos los atributos a excepción del nif del alumno serían elementos y no atributos. El nif sería un atributo de alumno..

 
//************************************************************************************************************
                                               TAREA 01
************************************************************************************************************//

//********** Tarea 1. Reconocimiento de las características de lenguajes de marcas *************************//

Casi siempre surge a todos los alumnos cuando realizan los XML la utilización de elemento o atributos. Pero en realidad no hay ninguna regla. Nos podemos encontrar XML con muchos atributos  y pocos elementos y al revés, llevan discutiendo esto en los foros de internet desde que empezó a ser popular XML.
Si bien es cierto que algunas empresas como  IBM han sacado artículos con  reglas para "intentar" estandarizar la legibilidad de los XML. En resumen, no hay una única respuesta correcta (dentro de las que están bien), y el alumno debe saberlo al realizar el documento XML. Le podemos orientar diciendo que utilicen el menor número de atributos posibles o al revés.  
Vamos a tomar como referencia los consejos de IBM:
Los elementos son datos importantes que hay que almacenar.
Los atributos puede ser elementos  cuya información no es "tan relevante", pero esto no es obligatorio puede ser también elementos.
El identificador es siempre un atributo (Es decir, id, dni, código único, etc.. lo que en el modelo ER se llama identificador).  Se trata de que los metadatos (datos sobre los datos) deben ser almacenados como atributos, y que los datos debe almacenarse como elementos.
Si quieres que los datos almacenados en el XML sean más legibles y estructurados utiliza mas elementos que atributos si quieres que sea más abreviado y menos legible utiliza "más atributos".
Si un elemento está estrechamente unido con otro, es decir que si modifico uno se modifica el otro no se aconseja ponerlo cómo atributos. Si sabemos que la unidad va a modificar el cantidad, es decir no es lo mismo 250ml que 250g se aconseja como elemento uno y el otro que modifica como atributo.
Un atributo no se puede dividirse "contener unidades más pequeñas". Aquí viene la típica duda de la fecha. La pongo como atributo (XX/XX/XXXX)? la pongo como un único elemento (XX/XX/XXXX)? o la pongo como un elemento fecha y tres subelementos (día, mes, año). Aconsejamos la tercera opción y tiene una razón. Nos tenemos que preguntar ¿Qué queremos hacer con la fecha?. Queremos solo mostrarla? las tres opciones son correctas. Queremos manipular por separado con alguna sentencia XQUERY  los dias, meses o años, la tercera opción es la correcta. Esta es la razón por la que la fecha te la puedes encontrar de las tres formas y las tres son correctas, depende de lo que quieres hacer y como las queremos almacenar.
Los atributos no se puede subdividir en el futuro, si tenemos un XML "extenso"  en el futuro pensamos que se pueden subdividir ese dato es más rápido hacerlo desde un elemento que desde un atributo, ya que no tengo que reestructurar "tanto" el documento.
Fuente: Alberto Plata
Con todo lo explicado anteriormente realizar los siguientes ejercicios dando prioridad a la claridad y la estructura del documento.

1.- Diseñar un documento válido en XML (agenda.xml) que permita estructurar la información de una agenda de teléfonos, suponer que la información que podemos tener de una persona es su nombre y apellidos, su dirección y sus teléfonos, que pueden ser el teléfono de casa, el móvil y el teléfono del trabajo.

La valoración de este ejercicio será de un total de 3 puntos, 2 puntos por utilizar la notación adecuada, 1 punto por definir y utilizar las etiquetas adecuadas.

Tiempo de resolución aproximado: 1 h.

2.- Diseñar un documento válido en XML (recetas.xml) que permita estructurar la información de las recetas de cocina de un restaurante y aplicarlo a la siguiente receta de cocina. Hay que hacerlo de modo que un sistema informático pueda realizar búsquedas por ingredientes, cantidad de comensales o nombre de la receta.

Sopa de cebolla (4 personas)

Ingredientes:

1 Kg. de cebollas.
2 l. de caldo de carne.
100 gr. mantequilla.
1 cucharada de harina.
100 gr. de queso emmental suizo o gruyére rallado.
Pan tostado en rebanadas.
Tomillo.
1 hoja de laurel.
Pimienta.
Proceso:

Pelar y partir las cebollas en rodajas finas.
Rehogarlas con la mantequilla, sal y pimienta a fuego lento hasta que estén transparentes sin dorarse.
Añadir la harina sin dejar de remover.
Ponerlo en una cazuela con el caldo, el tomillo y el laurel.
Dejar cocer a fuego lento durante unos 15 minutos.
Poner las rebanadas de pan encima, espolvorear el queso y gratinar al horno.
La valoración de este ejercicio será de un total de 3 puntos, 2 puntos por utilizar la notación adecuada, 1 punto por definir y utilizar las etiquetas adecuadas.

Tiempo de resolución aproximado: 1,5 h.

3.- Diseñar un documento XML (modulos.xml) válido que permita estructurar la información para permitir su gestión informática de los alumnos de un modulo del ciclo formativo DAM. Aplicarlo al módulo de Lenguajes de Marcas y Sistemas de Gestión de Información pero pueden aparecer el resto de módulos, sabiendo que tiene asignadas 4 horas semanales y es de carácter obligatorio. El modulo se imparte entre el 15 de septiembre de 2010 y el 30 de junio de 2011. La fecha nos servirá para realizar búsquedas en el documento por días, meses y años.

Existen matriculados dos alumnos:

Ana Fernández Gutiérrez con nif 16965696L teléfono 789654321 email ana.fdezgtrrez@hotmail.com, su dirección es C/ El Percebe, 13 de Santander CP 39302 No hay información sobre las faltas de asistencia o sus notas hasta el momento.

Pepito Grillo con nif 98765432H teléfono 656566555 email yhyh@yahoo.com, su dirección es Avd. El Pez, 5 de Suances CP 39401. Su nota es "apto" y no tiene faltas de asistencia
