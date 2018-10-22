# Tareas Oscar

## 22-10-2018

Repaso y estudio de los objetos singleton en node (basicamente no existen como tal).
Estuduio del comportamiento de los require y de sus ciclos de vida.

### problema de conexiones mongodb y saturación de envíos sobre el servidor
Modelo de autoreconexión MongoDb con Cero Buffer en caso de desconexión.
Resuelto y operativo para controlar las conexiones y las caidas sin dejar buffer de querys.

https://github.com/spinmedia-msp/oscar-pruebas-electorales/tree/master/control-conexiones-mongo

Esta operativa resuelve uno de los misterios de las conexiones multiples sobre mongodb.
Se implementa en la Difusin y se pone a prueba.

## 19-10-2018
pruebas fabric y Ansible.
Reunión Seguimiento

## 18-10-2018
Reinstalación de CentOs7. Revisin de documentación del instalador

  https://github.com/spinmedia-msp/elecc2019-dockers/blob/master/instalacionesCentos.md

## 17-10-2018
Mejoras en el script-python de simulación de envíos indra.
Se parametriza y se cuadran los registros en redis para la coincidencia de envíos y errores.

  https://github.com/spinmedia-msp/elecc-node-ftp-release/blob/master/python/bucle_sftp.md

El simulador se deberá lanzar desde un equipo externo a los servidores para que el flujo sea una simulación correcta y también validar de esta forma el docker-sftp

Añadido de nombre fijo a los dockers y variables de entorno para parametrizar y depurar mejor los log

## 16-10-2018
Electron WebViewer, ajuste de parametros de entrada compatible con el formato de venta de msp. Proyecto .git para clonar en instalaciones de msp si se requiere.

Core Msp, busca la existencia de Electron Viewer y en caso afirmativo lanzará todas las web por esta vía.
Actualización y pruebas en 'mspdemo'

https://github.com/spinmedia-msp/electron-msp-webview

Arranque y lanzador del 'cortados de ficheros' sobre un docker de forma autonoma y respondiendo a los ficheros que entran desde un segundo equipo. (simulación indra 100% fiable)

### Guía de comandos básicos de linux (entorno debían pero bastante generalista)
Todo el mundo debería tener unos conocimientos mínimos

https://github.com/spinmedia-msp/elecc2019-dockers/blob/master/comandos_basicos_linux.md

### Revisión de API Dokcer para automatizacin de tares y control de estados

https://docs.docker.com/develop/sdk/

Automatización desde node:
https://github.com/apocas/dockerode

## 15-10-2018
Revisión de performance en equipos. Control de conexiones a base de datos, revisión de conexiones multiples. Software Linux para control de performance provocando un uso de CPU 100% de forma controlada.
Creación de Electron WebViewer para msp.

## 11-10-2018
Revisión de errores de rendimiento de node el proceso de corte.

Error tipo (too manay files open) - sustitición de biblioteca nativa fs por fs-graceful.

Nuevas pruebas

## 10-10-2018
Agrupación/Revisión de proyectos demos en un repositorio general y borrado de repositorios sueltos.

https://github.com/spinmedia-msp/oscar-pruebas-electorales

Solución para reconexiones vía amqp, puesta en marcha del proyecto de actualiación y primeras pruebas

## 09-10-2018
Revisión de problemas en el servicio de corte, llenado de disco duro.
Reunión de Seguimiento
Levantado proyecto de actualización via NODE.
Busqueda del modo de autoreconexión de amqp (rabbitmq) de forma autonoma

https://github.com/spinmedia-msp/elecc-node-updater-release.git

## 08-10-2018
Revisión de problemas en el servicio de corte, pruebas y cursos de nuevas herramientas.

[trabajo_diario.md]
https://github.com/spinmedia-msp/elecc-node-ftp-release/blob/master/TRABAJO_DIARIO.md

## 05-10-2018
Montaje de equipos indra, instalaciones linux en hp, revisiones varias de proyectos electorales

[trabajo_diario.md]
https://github.com/spinmedia-msp/elecc-node-ftp-release/blob/master/TRABAJO_DIARIO.md

## 04-10-2018
Revisión con Maria de estructura básica de la difusión. Funcionamiento de "ejs" contra "pug".

Creación de ficheros js de registros de Noche y Partidos heredados de las primeras pruebas.

[trabajo_diario.md]
https://github.com/spinmedia-msp/elecc-node-ftp-release/blob/master/TRABAJO_DIARIO.md
