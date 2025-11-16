# ppp_cmux
🔌 PPP y CMUX en módems GSM

Cuando trabajamos con un módem GSM/4G, lo mas común es emplear comandos AT. Prácticamente todos los modems ofrecen comandos para levantar conexiones TCP (crudas) que se pueden utilizar para enviar peticiones a un servidor. En ese caso, el microcontrolador es responsable de crear las peticiones http y parsear las respuestas.

Algunos modelos ofrecen comandos dedicados para http/https, de más alto nivel, con los cuales podemos hacer peticiones GET/POST, etc sin preocuparnos de la sintaxis.

Pero hay otras opciones que suelen pasar desapercibidas: PPP y CMUX

🔹 PPP (Point to Point Protocol)
PPP Permite configurar el módem como un adaptador de red real. Con esto, el microcontrolador adquiere una IP directamente del modem, y emplea su stack TCP como si estuviera conectado por WiFi o Ethernet. Las "aplicaciones" que emplean HTTP, MQTT, etc, no distinguen de donde "proviene" internet ya es el propio stack, el responsable de rutear las peticiones por las interfaces de red activas. 

Esto permite:

 👉 Conectividad redundante Modem/Wifi/Ethernet, lo cual es muy deseable para muchas aplicaciones. 
 👉 Simplificar el código de la aplicacion, ya que las funciones para http, mqtt, etc, son agnosticas de la interface "real" por la cual se cursan efectivamente , ya que esto lo decide el stack tcp.
 👉 Mas flexibilidad en la gestión de las conexiones, certificados, etc, ya que todo lo maneja el firmware, y no se depende de implementaciones parciales en el set de comandos AT del modem.

🔹 CMUX (Multiplexación de canales AT)
Pero el "problema" de PPP, es que cuando se configura el modem en este modo, el stack TCP/IP del microcontrolador "captura" la comunicacion y es imposible enviar comandos AT, que a veces son necesarios para conocer por ejemplo, el nivel de señal del modem, o para obtener posicion GPS en esos modems con GNSS integrado.

Lo normal es conmutar entre modo Dato y modo Comando. Al hacer eso, se sale momentaneamente de PPP, se pasa a modo AT, se ejecutan los comandos deseados y luego se vuelve a PPP.

Pero hay una opcion muy potente para resolver esto que es CMUX (formalmente el estandard GSM 0710). 

Cmux "encapsula" los datos bidireccionales de varios puertos seriales "virtuales", sobre un puerto serie físico real. De esta forma, se puede emplear un puerto virtual para comandos AT y otro para PPP, sin necesidad de estar conmutando entre modos y cortando / restableciendo la conexión a internet.

🔧 ESP32
El ecosistema de firmware ESP32 (IDF y Arduino) posee todas las herramientas para implementar PPP y CMUX. Incluso va un paso mas allá, permitiendo hacer NAT entre interfaces.

👉 ¿Ya probaste PPP / CMUX en tus proyectos?

Estás desarrollando un proyecto IoT y necesitas apoyo en hardware o firmware? Con experiencia en el diseño e implementación de soluciones IoT, puedo ayudarte a llevar tus ideas al siguiente nivel. ¡Hablemos! 🚀
