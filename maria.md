# Tareas María

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





