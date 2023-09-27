## Docker SWARM 
- Para la realizacion del trabajo utilice un servidor de express pequeño y cree una imagen con él llamada "node_ayrton"
- Para crear el servicio se utilizó el comando "docker stack deploy -c node_servers.yml server_swarm, donde node_servers.yml es el archivo para generar el servicio y server_swarm el nombre del servicio que le asigno

## Preparar el entorno
- Para que este comando funcione primero hay que activar swarm en el dispositivo, para ello se utiliza el comando "docker swarm init" 

## Escalar servicio
- Para escalar el servicio se debe utilizar el comando "docker service scale nombre=cantidad", donde nombre es el nombre del servicio y cantidad el numero de contenedores al que escalará el servicio, ya sea menor o mayor. 
- A la hora de usar el comando para escalar el servicio, los contenedores caen y se levantan nuevamente en la cantidad asignada con el comando. Entonces cabe recalcar que se debe hacer un volumen para mantener la persistencia de datos.