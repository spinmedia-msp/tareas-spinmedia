# Tareas Oscar

## 31-10-2018

Montaje de 3 Equipos de Difusión sobre Mate 18.04

[documentacion y presentacion] gitkraken ui

[previsto] Revisión de resion.io

## 30-10-2018

Revisión de imcopatibilidades Difusion Windows&Linux

Revisión de apertura de servicio

Node y Electron sobre Raspbian

Reunión de Seguimiento



## 29-10-2018

Finalizado del sistema de actualización completo con modules vía git.
No compatible de forma simultanea entre windows y linux

## 26-10-2018

consolidación del actualizador mezclando las 2 técnicas (descompresión y git)



## 25-10-2018

Proyecto paralelo de actualización vía node con sistema git sobre windows/linux cliente
La aplicación queda como una mezcla de la anterior con git
.
La primera instalación con todos los (node_modules) se hace con la generación de un .zip global y las actualizaciones posteriores se generan a modo de "pull" usando git de forma automatizada y recogiendo solo los ficheros necesarios.

Los equipos windows requieren de la instalación de Git y correr un pequeño script para enviar su clave rsa de confianza al servidor local que contiene el repositorio .git

El objetivo es conseguir un actualizador con el menor coste posible de red y totalemnte off-line (de internet)


## 24-10-2018

Revisión de Git Server como Docker y pruebas

https://www.linux.com/learn/how-run-your-own-git-server

Documentado en el proyecto de test
Queda automatizado sobre git la actualización de un repositorio sin peticin de claves ssh

Centos7
https://gist.github.com/ch3nkula/73a5f25fc0348597df368283e0fcc437


## 23-10-2018

Subida de repositorio de mapas sobre rm2all.com

Montaje de docker nginx sobre servidores para ficheros estáticos

Creación de sistema de seguimiento hash del .dat

Creación de documentación para seguimiento de estado en los servidores carpeta /home/elecciones/recibido

https://github.com/spinmedia-msp/test-electorales/blob/master/script%26ejemplos/revision_directorio_recibidos.md


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
