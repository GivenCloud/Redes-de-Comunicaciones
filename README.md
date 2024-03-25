La práctica consiste en realizar un sistema de compartición y transferencia de
ficheros al que denominaremos nanoFiles, y que se describe a continuación.
El sistema nanoFiles está formado por un servidor de directorio y un conjunto de peers (pares), que se
comunican entre sí de la siguiente forma:
Por un lado, la comunicación entre cada peer y el servidor de directorio se rige por el modelo clienteservidor. Un peer actúa como cliente del directorio para registrar un nombre de usuario, consultar los
nombres de usuario registrados, consultar los ficheros que pueden ser descargados de otros peers,
publicar los ficheros que quiere compartir con el resto de pares, etc.
Por otro lado, el modelo de comunicación entre pares es peer-to-peer (P2P).
Cuando un peer actúa como cliente de otro peer servidor, el cliente puede solicitar el listado de
ficheros que el servidor comparte, descargar dichos ficheros, etc.
De manera complementaria, un peer puede convertirse a petición del usuario en servidor de
ficheros, de forma que escuche en un puerto determinado en espera de que otros peers se
conecten para solicitarle los archivos que el servidor está compartiendo. Dependiendo de la
funcionalidad implementada por el alumnado, es posible que un peer pueda llegar a actuar
simultáneamente como cliente y como servidor de otros peers, si bien como paso previo
(funcionalidad mínima obligatoria) se contempla el escenario en que un peer únicamente
pueda actuar en uno de los dos roles (cliente o servidor) en un instante dado.
