# Topología de red Etapa Estelar de Villa Club en Packet Tracer

Diseñamos esta configuración de red para una urbanización, dadas algunas limitaciones que se nos plantearon para el desarrollo del proyecto. El tema principal es acerca de un adecuado direccionamiento de red.
Es un proyecto interesante, porque nos plantea el hecho de configurar la red de una urbanización, dando libre elección. Presentando ciertos detalles al momento del desarrollo y compartiéndolo con otros usuarios para su guía a futuro.
Red Diseñada
 
**Urbanización: Villa Club Etapa Estelar (Google Maps)

# Planteamiento

En el Proyecto se nos propuso elegir una etapa de una urbanización, siguiendo ciertas indicaciones. 
“Cada grupo deberá escoger una urbanización (mediante google maps) y una dirección de red de clase B. Luego en base al número de casas y manzanas realizar un adecuado direccionamiento de red que evite que el broadcast de una manzana afecte a otra (subredes y vlans)”.
Tomando en cuenta esto diseñamos la red de la urbanización con 4 computadores conectados a un mismo dispositivo de red, cubriendo una manzana de la urbanización. 
Dado que son 8 manzanas las que posee la Etapa Estelar, se necesita de 32 pc, conectados a los dispositivos de red correspondientes:
 
1era Manzana: “Mz 1 Vlan 2” (4 PC)
Ip: 134.18.0.1
2da Manzana: “Mz 2 Vlan 4” (4 PC)
Ip: 134.18.32.1
3era Manzana: “Mz 3 Vlan 6” (4 PC)
Ip: 134.18.64.1
4ta Manzana: “Mz 4 Vlan 8” (4 PC)
Ip: 134.18.96.1
5ta Manzana: “Mz 5 Vlan 10” (4 PC)
Ip: 134.18.128.1
6ta Manzana: “Mz 6 Vlan 12” (4 PC)
Ip: 134.18.160.1
7ma Manzana: “Mz 7 Vlan 14” (4 PC)
Ip: 134.18.192.1
8va Manzana: “Mz 8 Vlan 16” (4 PC)
Ip: 134.18.224.1
 
Como se nos pidió, todos los dispositivos de red se deben encontrar interconectados y tener una salida a la internet mediante una única conexión. 

Limitaciones
Para facilidad del trabajo desarrollamos la simulación de la topología en el Cisco Packet Tracer para diseñar de manera óptima y segura la red, sabiendo cuantos dispositivos se iban a emplear, siguiendo los puntos que nos especificaron.
Se nos planteó elegir un método para realizar el direccionamiento de la red que hayamos seleccionado, nosotros elegimos el método de router on a stick; el cual es una de los métodos más comunes para hacer el enrutamiento inter-VLAN. Consiste en crear sub interfaces en una sola interface física de un router; tenemos con esta configuración la posibilidad de utilizar una sola interface para enrutar los paquetes de varias VLAN que viajan a través del puerto trunk de un switch conectado a esa interface.

# Como Ejecutar el Proyecto
Instalar Packet Tracer y descargar el proyecto .pkt, ejecutarlo y ver el funcionamiento adecuado
