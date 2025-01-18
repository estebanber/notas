## Ideas
- Animación de recorridos y rutas
- [Cortador de botella](https://www.instructables.com/DIY-Automated-Glass-Bottle-Cutter/?utm_source=newsletter&utm_medium=email)
- [Video de cortador de botellas](https://www.youtube.com/watch?v=Gdn8ix2_LdE&t=607s)
- [Mini drone](https://www.instructables.com/Make-a-Tiny-Arduino-Drone-With-FPV-Camera/?utm_source=newsletter&utm_medium=email)

## Links Budderfly
- [Discussion about bacnet-stack on ESp32](https://github.com/bacnet-stack/bacnet-stack/issues/196)
- [Library BACnet](https://github.com/bacnet-stack/bacnet-stack)

# 2024-05-12
Finalmente armé un script para crear notas rapidamente en linux
Me faltaría talvez crear un workspace para el trabajo. Quizas sea sufieciente con copiar el archivo y apuntar a otra carpeta

# 2024-05-16
Pixelorama - Software para hacer pixelart
Ver Godot

# 2024-05-17
Probar Osu (Juego de ritmo) que por alguna razón era super popular en redit

# 2024-06-03
Modificación para usar switch budderfly HW ver 1.0
//#define RELAY_ON_PIN                                                  GPIO_NUM_4
//#define RELAY_OFF_PIN                                                 GPIO_NUM_21
#define RELAY_ON_PIN                                                    GPIO_NUM_16
#define RELAY_OFF_PIN                                                   GPIO_NUM_17

# 2024-06-13
## Cursos de embebidos
[](https://pro.codely.com/library/patrones-de-diseno-creacionales-167860/about/)
[](https://www.udemy.com/course/embedded-c-programming-design-patterns/?utm_source=adwords&utm_medium=udemyads&utm_campaign=LongTail_la.EN_cc.ROW&campaigntype=Search&portfolio=ROW-English&language=EN&product=Course&test=&audience=DSA&topic=&priority=&utm_content=deal4584&utm_term=_._ag_77879424134_._ad_535397279649_._kw__._de_c_._dm__._pl__._ti_dsa-1007766171312_._li_9185698_._pd__._&matchtype=&gad_source=1&gclid=EAIaIQobChMIqNrTk4fRhgMVIEVIAB3pJQEOEAAYASAAEgItaPD_BwE&couponCode=2021PM25)
[](https://python-graph-gallery.com/color-palette-finder/)

# 2024-06-29
Me siento un poco estresado y muy desmotivado para arrancar cualquier cosa. Lo unico que soy capaz de hacer aun es trabajar. Pero no se por cuanot tiempo
Tengo un poco de miedo de tener algun problema de ansiedad o ataques de pánico. En estemomento siento una presión permanente en la cabeza y en los ojos.
Quiero hacer tantas cosas que no se por donde empezar. Debo empezar por algo y dejar de procrastinar

# 2024-06-30
Finalmente me senté a trabajar en omnitronic. Estuve todo el día pero hice un buen progreso ya que determiné que gran parte del diseño funciona bien.
No se si esp or la cercanía de las vacaciones o por el magnesio que tomo a la noche, pero hoy me sentí con bastante energía.

# 2024-07-04
Encontré esta pagina miy interesante con consejos y tutoriales para ejecutar proyectos electrónicos:
[Hutscape](https://hutscape.com)


# 2024-07-05
Al parecer la maxima cantidad de memoria externa que puede direccionar el ESP32 son 4MB.
Se puede hacer un bank switching usando el módulo Himem.
[Himem](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/system/himem.html)
[Example](https://github.com/espressif/esp-idf/tree/1cb4f346/examples/system/himem)

Shotcut o Openshot?

[Grupo de desarrolladores](https://dyne.org/)

# 2024-08-10
Aun no trabajo como me gustaría. Me siento muy perdido y desmotivado. Al menos aun puedo trabajar en mi trabajo oficial. Pero fuera de eso no hago practicamente nada. You tube me roba mucho tiempo. Es una adicción peligrosa que siento que me está deteriorando como persona.

# 2024-08-15
Día tranquilo, aunque se empieza a mover el tema casa. Me da miedo que nos gastemos el dinero.Tenemos que arrancar ahora mismo.
Hoy trabajé poco, he estado un poco perdido y lento. Sigo teniendo dudas de mi inglés. Aunque fluye y puedo comunicarme. Debería intentar leer un libro en ingles, probablemente stephen king.
Mañana debería armar el banco de pruebas si o si, tambien completar los excels de las promociones.
Quero leer, quiero ver quiero dibujar... y no hagop nada.

# 2024-08-23
Viernes, finalmente... estoy con muy poca plata y para como gastamos 25k en fotocopias... Estoy cansado, pero este fines no tenemos planes. quizas me haga un asado.

# 2024-08-25
Voy a realizar un nuevo intento de automatizar mi instalación de archlinux. El objetivo es tener mi propio scrip qu automatice la instalación del sistema, descarga de todos los paquetes necesarios y la configuración de mis utilidades.
Primer paso: documento markdown con todos los pasos para tener un sistema completamente funcional de 0.
Segundo paso: Creación de scripts.
    - Instalación básica, particiones, descarga de sitema base
    - Configuración de herramientas básicas en CLI
    - Configuración de herramientas básicas con GUI
    - Clonar repositorios personalizados
    - Descargar software secundario
        - Desarrollo C
        - Desarrollo de embebidos
            - ESP-IDF
            - MPLABX
            - KICAD
                - Clonar librerías personalizadas
        - Trabajo
        - Fotografía (gestión y procesado)
        - Juegos
        - Backup y nube (syncthing, repositorios)
        - Colecciones:
            - Libros
            - Imagenes
            - Comics
            - Peliculas y series?
    - Configuración de software linkeando dotfiles

# 2024-08-29
    - [X] Test firmware 1.25.0-391 over 1.24.9-385 --> no change of settings; no other issues!
    - [X] OTA endpoint must work correctly
    - [X] Only send connection string message after the successful first metric from stm32
        - [X] After successful ota from stm32, and you get yet another metric on the new firmware; re-send the connection string
    - [ ] restart esp32 whenever the main esp32 OTA task fails

    - Checklist the testing
    - Crear tool para checkear CRC16 de eeprom
    - Calcular el CRC16 de la eeprom e imprimirlo en pantalla en un modo debug
    - No configuraciones (ESP32, STM32) ni networking para Aadi

# 2024-09-01

# 2024-09-02
Finalmente estoy terminando la placa de Omnitronic. Un poco mas complejidad que esta y necesito mas capas o mas espacio.

# 2024-09-03
Fui a la Pile y luego me fui al cine a ver Alien Romulus.

# 2024-11-14
Nuevamente procrastinando, jugando con una nueva instlación de linux, sistema de repositorios y notas

