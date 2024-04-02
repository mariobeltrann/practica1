# Descarga la imagen 'ubuntu y comprueba que está en tu equipo
    con docker run -it --name practica1 ubuntu:latest bash descargamos la última imagen de ubuntu 
    con docker image comprobamos las imágenes

![creacion](./imagenes/Screenshot_20240402_160110.png)

    Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre
    con docker run -it ubuntu bash creamos un contenedor sin nombre

![Alt text](imagenes/Screenshot_20240402_165316.png)

    con docker ps -a nos muestra los contenedores , y estará de primero en el último de el que salimos , que será del que queremos obtener el nombre.

![Alt text](imagenes/Screenshot_20240402_165357.png)

# Crea un contenedor con el nombre 'practica1'. ¿Como puedes acceder a él?

![creacion](./imagenes/Screenshot_20240402_160110.png)
![comprobacion](./imagenes/Screenshot_20240402_161206.png)
![comprobacion](imagenes/Screenshot_20240402_161012.png)

# con docker run -it --name ubu1 ubuntu bash creamos el contenedor
		con exit dejamos de interactuar con el contenedor

![comprobacion](imagenes/Screenshot_20240402_161313.png) 

		con docker start ubu1 iniciamos el contenedor
		con docker exec -it ubu1 bash accedemos al contenedor

![comprobacion](imagenes/Screenshot_20240402_161724.png) 


# Comprueba que ip tiene y si puedes hacer un ping a google.com
    con apt update actualizamos los paquetes

![Alt text](imagenes/Screenshot_20240402_161920.png)

    con apt install net-tools instalamos el paquete net-tools

![Alt text](imagenes/Screenshot_20240402_162226.png)

    con ifconfig comprobamos nuestra ip

![Alt text](imagenes/Screenshot_20240402_162254.png)

    con apt install iputils-ping instalamos el paquete iputils-ping

![Alt text](imagenes/Screenshot_20240402_162022.png)

    con ping google.com hacemos ping a google.com

![Alt text](imagenes/Screenshot_20240402_162421.png)

# Crea un contenedor con el nombre 'practica1.2'. ¿Puedes hacer ping entre los contenedores?
		con docker run -it --name prctica1.2 ubuntu bash creamos el contenedor

![Alt text](imagenes/Screenshot_20240402_162621.png)

		con apt update actualizamos los paquetes

![Alt text](imagenes/Screenshot_20240402_162724.png)

		con apt install net-tools instalamos el paquete net-tools

![Alt text](imagenes/Screenshot_20240402_162832.png)

		con ifconfig comprobamos nuestra ip y la copiamos

![Alt text](imagenes/Screenshot_20240402_162920.png)

	en otra pestaña hacemos atach sell a la otra maquina  (ya instalamos iputils-ping) con ping 172.17.0.4 hacemos ping a la ip del otro contenedor que 
    antes ya habiamos copiado.

![Alt text](imagenes/Screenshot_20240402_163124.png)

		
# Sal del terminal, ¿que ocurrió con el contenedor?
Se detuvo el contenedor
# ¿Cuanta memoria en el disco duro ocupaste? ¿Hay alguna herramienta de docker para calcularlo?
		con el comando docker stats podemos comprobarlo

![Alt text](imagenes/Screenshot_20240402_163518.png)

# ¿Cuanta RAM ocupan los contenedores? Crea cuantos contenedores necesites para calcularlo.?
		
![Alt text](imagenes/Screenshot_20240402_163518.png)
