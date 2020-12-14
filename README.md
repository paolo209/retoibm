# retoibm
Paolo Casasola Esteban - Reto IBM

*El reto ha sido resuelto en modo StandAlone en un entorno local con maquinas virtuales, se hizo uso de docker y docker-compose, para ver la respuesta ejecute: 
docker-compose up -d --build
curl localhost/retoibm/sumar/10/20

*El directorio 'otros' contiene un archivo .yml para desplegar el proyecto backend sin hacer uso de un Dockerfile, si desea desplegar debe ubicarse dentro del directorio 'otros' y ejecute:
docker-compose up -d

*El directorio 'backend_docker_swarm' contiene un archivo .yml para deplegar el servicio dentro de un orquestador docker-swarm, para ejecutar se requiere tener habilitado el modo swarm en docker. De estar habilitado ubicarse en el directorio 'backend_docker_swarm' y ejecutar lo siguiente:
docker stack deploy --compose-file docker-compose.yml back


*NOTA:
El archivo de despliegue para docker swarm creara un servicio con el nombre del servicio declarado en el archivo .yml junto al prefijo que se utilizo en el comando para deplegar. En este caso el servicio se llamaria 'back_retoibm'.