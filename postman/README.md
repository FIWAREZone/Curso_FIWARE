# Introducción

Para hacer pruebas con la API de FIWARE será necesario disponer de una herramienta que permita hacer peticiones HTTP e interactuar con esta. En este caso, nosotros recomendamos la herramienta Postman, que permite gestionar las colecciones de peticiones, por lo que será muy sencillo realizar las operaciones necesarias.

Postman permite definir un catálogo de peticiones ([Collection](Collection.postman_collection.json)) y un fichero con variables donde almacenar los datos típicos del entorno donde realizar las pruebas ([Environment](Enviroment.postman_environment.json)). Estos ficheros se pueden exportar e importar para facilitar el uso por otras personas. 

## Instalación y configuración de Postman

1. Descargar [Postman](https://www.getpostman.com/) e instalar

2. Descargar los ficheros de  [colección](Collection.postman_collection.json) y [entorno](Enviroment.postman_environment.json) del curso y extraerlos. Para descargar, hacer click [aquí](https://github.com/FIWAREZone/Curso_FIWARE/blob/master/postman/postman.zip?raw=true)
5. Abrir Postman

6. Importar los dos ficheros contenidos en el zip
![Importar Collection](https://github.com/danvilmot/IoT_Course/blob/master/postman/files/import_collection.jpg)

8. Configurar las credenciales: user, password, service y subservice (Service Path) que se darán en cada sesión.


## Variables de entorno

Una vez hayamos importado tanto la colección de peticiones como el entorno (los dos ficheros descargados en el punto anterior) 

Las variables de entorno contienen parámetros que se aplican a todas las colecciones pero, que para facilitar cambiarlas todas a las vez, se han hecho variables de entorno, como por ejemplo la URL del servidor. Es necesario modificar las variables de entorno con los parámetros correspondientes:

| Parametro         |descripción   												|
| :-----------------|:--------------											|
| user              | Usuario con permisos de acceso							|
| password          | Contraseña del Usuario 									|
| service   		| Servicio del contex broker (Header Fiware-Service) 		|
| subservice      	| Subservicio del context broker (Header Fiware-ServicePath) |
| token 			| Token de autenticación de usuario dinámico 				|
| host 				| URL del servidor, es decir, del Orion Context Broker 		|
| host_iota 				| URL del servicio IoT Agent 		|
| iota_port 				| URL del servicio IoT Agent		|
| UL_apikey 				| Apikey para el envío de datos por IoTA con protocolo ultralight 		|
| JSON_apikey 			| Apikey para el envío de datos por IoTA con protocolo JSON 		|
| device_ID 				| Identificador de dispositivo		|

