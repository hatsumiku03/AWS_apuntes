# Objetivos:
	*Identificar la diferencia entre las regiones de AWS, las zonas de disponibilidad y ubicaciones perimetrales.
	
	* Identificar servicios y categorías de servicios de AWS.
	
1. AWS tiene propósito de ofrecer almacenamiento en la nube
2. AWS ofrece un huevo de redundancia a nivel de red a la hora de hablar de la escalabilidad 
	(Utiliza todos sus servidores ubicados en una zona geográfica para poder aumentar la escalabilidad si un servidor no puede ofrecerla)
3. Los datos entre servidores de regiones distintas quedan aislados entre si.
4. Según la zona geográfica, algunas leyes gubernamentales puedes obligar a que los datos se queden SOLO en esa región

# Extras:
  * Quienes usen AWS han de respaldar los datos por su propia cuenta
  * Como mínimo, AWS tiene dos servidores de disponibilidad en una zona geográfica en caso de que uno de ellos falle
  * Servidores creados después del 20 de mayo de 2019 si quieres usarlos has de habilitarlos tu de manera manual
  * Según la procedencia de tu cuenta, es posible que tengas restringido el acceso a ciertos servidores de AWS
  * A la hora de decidir donde vas a ubicar tu AWS ten en cuenta en que zona lo quieres dedicar más, be like, si es para francia, pillate algún servidor para allí
  	Cuadraran correctamente:
  		1. Normas gubernamentales
  		2. Comodidad a los clientes que se vayan a hospedar en tus servicios de AWS
  		3. Servicios dedicados para ayudarte
  		4. Costes
  	(De normal el factor más determinante es la comodidad hacía los clientes)


# Conceptos básicos
  * Zona de disponibilidad: Son servidores disgregados dentro de la misma región, su función es estar operativas en caso de que un servidor caiga, se pueda respaldar con otro dentro de la misma región.

  * Red Troncal: Red de redes, es un tipo de red que interconecta otras redes entre si.
    (A nivel de AWS, la conexión con los servidores es de red troncal)

  * Puntos de presencia: 