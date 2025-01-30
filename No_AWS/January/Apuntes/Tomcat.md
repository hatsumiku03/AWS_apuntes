# -------------------------
# --- APUNTES DE TOMCAT ---
# -------------------------


## Introducción
* Servidor HTTP y programas de aplicación:
Este punto solo es que un servidor ha de ser capaz de procesar
aplicaciones que pidan y reciban peticiones de un cliente a un servidor.

* Protocolo HTTP:
Sin necesidad de otros protocolos más a ya del HTTP, la página logrará ser dínamica
a través de herramientas de tu framework/herramienta y las peticiones.

* Aplicaciones dinámicas:
Son webs en las que el usuario puede interactuar, y a tiempo real hay eventos, animaciones
y cosas que de normal, un usuario no podría ver en una web estática.

* JavaEE:
Es la navaja suiza de las aplicaciones de Java, básicamente, es una aplicación que te ofrece
3000 herramientas para trabajar con Java y testear con este.



## Servlets y JSP
Los servlets y JSP son componentes dentro de la capa web.

* Servlets:
Son clases de Java, que a través del protocolo HTTP reciben y procesan las peticiones en el servidor.

* JSP (JavaServer Pages): Es una técnologia que a través de las peticiones, se encarga de generar contenido dinámico en forma de peticiones.



## ESTRUCTURA DE UNA APLICACIÓN JAVA

* Directorio raíz: 
La base del servidor donde se encontraran los archivos de categoría pública y también tener subdirectorios.

* WEB-INF:
Carpeta que se especifica en en web.xml, pues contiene la configuración del proyecto

* WEB-INF\classes:
Carpeta para almacenar los servlets para las peticiones dinámicas, y cualquier clase de java complementaria para cualquier tipo de función de la aplicación.

* WEB-INF\lib: 
Son clases de java que, básicamente contienen plugins, como el que pueda ser lectura de un pdf para la aplicación, hacer conexiones a las bases de datos, ese tipo de cosas.

* META-INF:
Es un archivo de configuración adicional que sirve que flipas para las configuración de la estrucutura del proyecto entero a nivel web.



## EMPAQUETADO
A la hora de desplegar aplicaciones java, no deja de ser cómodo el agarrar un archivo comprimido donde este todo nuestro trabajo y, pum, todo ya en producción.

Por un lado tenemos el empaquetado jar y por el otro el war.

* jar: 
Es rollo el zip o tar, un archivo comprimido en java.

* war (Web ARchive): Es un tipo de archivo comprimido, que hace de resumen en un solo archivo de toda la aplicación web. Entonces a la hora
de desplegarlo en aplicaicones java es cómodo ya que es el estándar, es ir, subir el archivo war, y arreglado.

En java para crear un archivo war, necesitas el siguiente comando:
	jar -cvf ejemplo.war -C /ruta/de/la/aplicación


## DESCRIPTOR DE DESPLIEGUE
Las aplicaciones web al final tienen una configuración que definen su comportamiento.

Aquí es donde entra el descriptor de despliegue, es un archivo XML donde se especifica como se va a desplegar una aplicación y que dependencias va a utilizar.



## Maven
Es una herramienta open-source para simplificar la la hora de compilar proyectos para tenerlos listitos en la fase de producción.

Y encima a la hora de compilar te dice si hay algún error en alguna parte en especifico del proyecto.xml

(El resto de teoría mirar en aules)