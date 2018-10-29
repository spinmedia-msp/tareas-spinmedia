# Tareas María

## 29/10/2018
* Error detectado y resuelto. Lo he probado muchas veces y no se ha vuelto a dar el caso. NO SE PUEDEN PONER LAS LLAMADAS A LOS JS DESDE LOS PUG. 
Explicación del error: https://github.com/spinmedia-msp/difusion_electron_release/blob/archivos_independientes/app/assets/js/app_difusion_portavoz.md

## 26/10/2018
* Proceso de independizar las animaciones en archivos js y cambio de variables y nombres de las funciones. En portavoz da un error y pierde la función lanzaAnimPortavozFormatoDia (lanzaAnimPortavozFormatoDia is not defined). El error salta al cerra la animación y volver a iniciarla pero de forma aleatoria. Lo voy a estudiar.

## 25/10/2018
* Alturas de items para comparativa y sin comparativa. 
* Cálculo correcto de sumatorio de items para el paginado con el margen sumado (He tenido que usar Jquery, incapaz de pescar el margen con Javascript. Sólo me pintaba el margen si estaba puesto en el style de la plantilla a pelo.)
* Hay que repensar el paginado porque tal y como está hecho no encuentro la manera de identificar el momento previo a que pinte el siguiente item en la pantalla.
* Plantillas pug portavoz. No las he podido probar. No conseguía ver la pantalla de portavoz en el Electron. Está corrigiéndolo Nacho.
* Cambios matutinos en las maquetas de portavoz: para César y Patri y pantalla portavoz datos sin cargos.

## 24/10/2018 
* Leyenda independizada y barras animadas redondeadas.
https://github.com/spinmedia-msp/difusion_electron_release/tree/maria_02
* Hay que pintar el gráfico del parlamento con forma de herradura. La librería chartjs no dispone de ningún parámetro para pintar esa forma de gráfico. En la web de elecciones tienen una ejemplo resuelto pero sin animación. Parece que está hecho con la librería https://www.flotcharts.org/flot/examples/ pero es de hace 3 años. Me he descargado el archivo:
https://github.com/spinmedia-msp/difusion_electron_release/blob/maria_02/app/assets/js/ejemplo_grafico_herradura_2015.js
Tendremos que implementar algo así para el chartjs.

## 23/10/2018
* Altura variable de los items resuelta en el branch Maria_02 del repositorio Difusion_electron_release. Código comentado entre las líneas 334 y 375 de app_difusion.js
* Ya he independizado uno de los archivos js de las animaciones. Hay que consensuar la nomenclatura y la división de los mismos. Cuando tengáis tiempo.

## 22/10/2018
* Item noche con caja que crece de background y coge la altura de la que tiene los datos. Se adapta al tamaño del contenido.
* Queda por resolver el alto del logo y el apilado de items en el contenedor si las cajas son de tamño variable.

## 19/10/2018
* Para que el animejs interprete correctamente la altura de la primera barra animada es necesario introducir un div vacío e invisible en el primer if de la función pintadoLista_noche (en el proyecto del que dispongo es la línea 238 de app_difusion.js):
``` $('#ListaPartidos').append('<div style="height:1px; visibility: hidden;">div de relleno</div>');  ``` 
``` //este div es un elemento invisible para que el primer elemento de la lista de items tenga una altura correcta.```

## 18/10/2018
* Pantalla vertical hecha. Estoy con los css de la adaptación de pantallas. Ya se adapta y es proporcianal. No tiene tamaños fijos. Problema alto item sin resolver. Ese valor es fijo:
https://github.com/spinmedia-msp/maria/blob/master/PROTOTIPO_MAQUETA_DIFUSION/pantallas/difusion/noche/pantalla_vertical.md

* Hay que resolver el tema de los módulos (los que se muestran y los que no).

* Me di cuenta ayer de que no necesitamos varias plantillas de item. Con quitar los elementos correspondientes en cada caso es suficiente. He hecho un ejemplo en mi maqueta. https://github.com/spinmedia-msp/maria Entre la línea 253 y 269 del archivo "dfh_noche_barras_comparativa.html". https://github.com/spinmedia-msp/maria/blob/master/PROTOTIPO_MAQUETA_DIFUSION/pantallas/difusion/noche/dfh_noche_barras_comparativa.html
Hay que ponerlo tras matar el animejs.
Lo ha cambiado Nacho por la línea de JQuery.
Con la plantilla item_barras_compara, que lo tiene todo, debería ser suficiente. Aunque tengo que probar si borrando "datos-comparativos" también borra los hijos.

* Anoche no pude subir lo del OpenLayers. Pero vaya, misterio ninguno. El bundle de openlayers en el electron: https://openlayers.org/en/latest/doc/tutorials/bundle.html  Yo hice un cerate window para probar el mapa sólo.
Es una guarrería la que lía con un archivo js kilométrico de mucho cuidado. Al hacer el npm start te crea un servidor localhost:1234. En cualquier caso tampoco lo he logrado ver pintado. Y le he dado un millón de vueltas.

## 17/10/2018
* Esta noche subo los último intentos de anoche con el openlayers desde casa. Pero sigue sin verse.
* Le he pasado el ejemplo del parlamento con el Chartjs a Nacho.
* Ya están las pantillas en el pug de todos los casos posibles de presentación de datos en difusión noche.
* Estoy con las pantallas verticales de presentación de datos: estoy intentando hacerlo con la misma plantilla para que sólo sea cuestión de cambiar el tamaño de la pantalla.

## 16/10/2018
* Nuevos intentos fallidos con la libreria Openlayers. Ya sobre electron pero sigue sin pintar el mapa.
* Estilos en Prototipo maqueta difusion en proceso de mejora. Mañana voy a hacer estilo genérico pantalla vertical y estilo genérico de barras verticales. 
* Mañana subo los nuevos estilos sobre el ejemplo de nacho que lo va a subir ya con el pug.

## 15/10/2018
* Pruebas fallidas con del mapa con la librería OpenLayers. Lo he intentado sobre la maqueta arrancando un servidor y me aparecen las flechas y no da error pero no se pinta el mapa. Sobre el electron de nacho no he sido capaz de momento.
* Proceso de mejora de los scss. Cada vez más ordenado y más sencillo de modificar desde el archivo _variables.scss.


## 14/10/2018

* Ejemplo template literals vs Pug/EJS. Enlace a la información de la prueba: https://github.com/spinmedia-msp/difusion_electron_release/blob/maria/app/assets/js/template_literals.md


## 10/10/2018

* Sobre el proyecto de difusion_electron_release: https://github.com/spinmedia-msp/difusion_electron_release/blob/maria/app/Maquetas.md
* Sobre mi maqueta en html: https://github.com/spinmedia-msp/maria/blob/master/PROTOTIPO_MAQUETA_DIFUSION/README.MD


## 09/10/2018

* Pantallas dfh_dia_primer_avance.html y dfh_dia_apertura.html hechas.
Enlace al readme del día: https://github.com/spinmedia-msp/maria/blob/master/PROTOTIPO_MAQUETA_DIFUSION/pantallas/difusion/dia/README.md

## 08/10/2018

* Cambio nomenclatura archivos
* Gráfico del aside con datos sobre la línea del gráfico. 
Plugin incluído mediante enlace cdn. Habría que incluirlo en los node_modules.
https://chartjs-plugin-datalabels.netlify.com/
* Todas las pantallas de portavoz terminadas: tienen un único js porque solo tiene 3 animaciones diferentes asociadas. Se puede cambiar.

Enlace trabajo del día: https://github.com/spinmedia-msp/maria





