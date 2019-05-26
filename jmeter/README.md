## Test de carga a un servidor web usando JMeter

##### David Cabezas Berrido

He creado un archivo .jmx en el que simulo 4 hebras de alumnos que
realizan cada una un login como alumno y una solicitud de sus datos 10
veces.

(2 solicitudes * 10 veces * 4 hebras = 80 solicitudes)

También simulo una hebra administrador que se loguea como
administrador y solicita los datos de 20 alumnos.

(1 login + 20 solicitudes de datos = 21 solicitudes)

En la imagen se ve el report con las 80 + 21 = 101 solicitudes
realizadas al servidor. También en results.jtl, que he sacado
ejecutando el comando de la captura summary.