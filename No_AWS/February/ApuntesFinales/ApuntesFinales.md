# Repaso final

### ¿Qué es docker?
Es un sistema de contenedores de linux que usa como base, efectivamente, linux para el despliegue de aplicaciones.

Es de código abierto y es recurrente integrarlo con servicios en la nube.

La estructura de docker se estructura en 3 partes:
* *Cliente*: Es el software que usas el contenedores que se comunica con docker.
* *Servidor*: Docker, quien hostea todo y atiende a peticiones y esas cosas.
* *Registro*: Es el lugar donde se guardan las imagenes que descargarmos después, tanto públicas como privadas de docker.

#### Componentes de docker
* *Docker engine*: Es para resumir todo el entorno de trabajo de docker, la parte encargada de ofrecer una experiencia interactiva con los contendores y ateneder peticiones de estos.
* *Imagenes de docker*: Es una plantilla que usamos de un entorno de trabajo ya preparado, esas cosillas que están subidas a lo que es docker engine y luego nosotros usamos a modo de contendoresm sn también las que mantienen activos los contenedores.

### Virtualización
Es el concepto de con medios hardware, utilizarlos en el software para por dentro simularlo como hardware.

### Contenedores
Es una tecnología de virtualización que usa el sistema operativo de base para ejecutarse. Es un entorno privado en el que ejecutas cosicas más pequeñas como lo que pueda ser modulos o dependencias especificas.

Docker como concepto usa de base linux para ejecutar los contenedores.
Si estás en windows necesitas 100% asegurado un subsistema de linux para que te pueda funcionar docker.

También en este apartado están los namespaces y los cgroups:

*Namespaces*: Dan aislamiento a cada contendor para que tengan sus propias configuraciones de red, procesos y demás.
*Cgroups*: Es un grupo de controladores que evitan que los contenedores chupen toda la CPU, memoria y esas cosas y no afecte severamente al rendimiento tener un contenedor por ahí suelto.

### Puntos del uso de los contenedores
* Un contenedor para trabajar ya suele estar preparado para lo que tiene que hacer.
* Facilitar el ensayo y error
* Evitan problemas de compatibilidad, al final si ejecutamos un php7 será ese para lo que necesitemos, fin.
* Podemos sincronizar contenedores para montar ahí algo chulo.
* Ocupan poco espacio.
* Acceder a los contenedores puede ser algo pesado si no se configura correctamente.
* Hay que tener en cuenta que los contenedores están directamente conectados con tu sistema operativo, si metes algún bicho el pato lo paga igual el sistema operativo entero. 

### Dockerfile
Scripts de docker que usamos para instruir como instalar imagenes y montarlas.

### Docker Hub
Es un repositorio de docker engine donde se guardan las imagenes y cosicas que usamos después de docker.

### Volúmenes de Docker
Sirve para almacenar y compartir los datos de los contenedores