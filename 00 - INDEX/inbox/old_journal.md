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


# 2025-02-10
    //Check LoRa module
    //Join and connect
    //if (LoRa OK)
    //  startLoRaWANTasks(BUDD_MPA_MQTT_TASK_STACK_SIZE,
    //                      BUDD_MPA_MQTT_TASK_PRIORITY);
    //else


# 2025-02-23
SSYNCMODE,1
SSYNCMODE,1
SCICLTIEM,10,10,0
SCICL,1
SSYNCMODE,1,7200
SSYNCMODE,3,7200
SSYNCMODE,1
SSYNCMODE,1
SCICLTIEM,10,10,0
SCICL,1
SSYNCMODE,3,7200
SSYNCMODE,1
SCICL,1
SSYNCMODE,2,300
SSYNCMODE,3,7200
SSYNCMODE,1


Modo automatico
Configurar cada cuanto enciende gps
registrar desfasaje

Modo manual
Apagar Bluetooth
Apagar rele
apagar GPS
apagar led (todos)

Comando
Estado todo

Boton
mostrar estado general con los led durante n segundos



```c
void debug_printr(char* txt, u8 reset)
{
    static int i = 0;
    if (reset) i = 0;
	sRECT rect;
	rect.x1 = 0;
	rect.y1 = 25*i;
	rect.x2 = 300;
	rect.y2 = rect.y1 + 25;
	SetFont((void*)&Roboto_Medium_19);
	SetColor(WHITE);
	SetBgColor(STATUS_DIVLINE_COLOR);
	OutTextInRect(WIDGET_INIT, &rect, txt, TEXT_LEFT_ALIGN, FONT_SYS);
	SetBgColor(BG_DEFAULT_COLOR);
    i++;
}

```

# 2025-02-27
08-3a-8d-19-90-18

# 2025-02-28
W (157377) rn126x-driver: rm126x_send: AT+SEND "8BA1023301000C0AC267E9033C46000000000000000042464200008C42000040410000803F0000803F00001142CDCC9C420066661E4200"
W (157391) rn126x-driver: SENDING COMMAND: AT+SEND "8BA1023301000C0AC267E9033C46000000000000000042464200008C42000040410000803F0000803F00001142CDCC9C420066661E4200"
W (158586) rn126x-driver: RECEIVED RESPONSE: 
OK
Sending packet: Type=3, Seed=5169, Seq=1, Total=2, Len=32
I (158587) budd-mpa-main: lora_task: Sending Payload using LoRaWAN
W (158594) rn126x-driver: rm126x_send: AT+SEND "8BA1122000803F00009A42000084420000484200007042CDCC804200007F43143EFB3F01"
W (158606) rn126x-driver: SENDING COMMAND: AT+SEND "8BA1122000803F00009A42000084420000484200007042CDCC804200007F43143EFB3F01"


W (218289) rn126x-driver: rm126x_send: AT+SEND "A2A1655301004E0CC267E9033C46000000000000000042464200008C42000040410000803F0000803F00001142CDCC9C420066661E420000803F00009A42000084420000484200007042CDCC804200007F43E03DFB3F01"
W (218310) rn126x-driver: SENDING COMMAND: AT+SEND "A2A1655301004E0CC267E9033C46000000000000000042464200008C42000040410000803F0000803F00001142CDCC9C420066661E420000803F00009A42000084420000484200007042CDCC804200007F43E03DFB3F01"

# 2025-03-05

# 2025-03-10
SEND_AT_CMD("ATS629?", NULL);
CHECK_AT_CMD("ATS613" , "10"        , store_config);       //RX1 delay

# 2025-03-18

void smart_recovery_calc_rate(u8 current_heat, u8 current_cool)
{
    //char debug_text[50];
    if (last_heat_stage != current_heat)
    {
        if (last_heat_stage == 0 && current_heat == 1)
        {
            start_time   = mktime(&CurtmTime);
            start_temp   = SysPara.RoomTemp;
            init_measure = 1;
            //sprintf(debug_text,"------> START H | %d | %d", smart_recovery_cooling_rate,smart_recovery_heating_rate);
            //debug_print(debug_text,0);
        }
        else if (last_heat_stage == 1 && current_heat == 0 && init_measure)
        {
            u16 _heating_rate = ((mktime(&CurtmTime) - start_time) / (SysPara.RoomTemp - start_temp)) * 10;
            if ((MIN_RATE < _heating_rate) && (_heating_rate < MAX_RATE))
            {
                smart_recovery_heating_rate = _heating_rate;
                IIC_Write(EEP_INDEX_HEATING_RATE, (u8 *)&_heating_rate, 2);
            }
            init_measure = 0;
            //sprintf(debug_text,"------> STOP H | %d | %d | %d",_heating_rate, smart_recovery_cooling_rate,smart_recovery_heating_rate);
            //debug_print(debug_text,0);
        }
        else 
        {
            init_measure = 0;
        }
        last_heat_stage = current_heat;
    }

    if (last_cool_stage != current_cool)
    {
        if (last_cool_stage == 0 && current_cool == 1)
        {
            start_time = mktime(&CurtmTime);
            start_temp = SysPara.RoomTemp;
            init_measure = 1;
            //sprintf(debug_text,"------> START C | %d | %d",smart_recovery_cooling_rate,smart_recovery_heating_rate);
            //debug_print(debug_text,0);
        }
        else if (last_cool_stage == 1 && current_cool == 0 && init_measure)
        {
            u16 _cooling_rate = ((mktime(&CurtmTime) - start_time) / (start_temp - SysPara.RoomTemp)) * 10;
            if ((MIN_RATE < _cooling_rate) && (_cooling_rate < MAX_RATE))
            {
                smart_recovery_cooling_rate = _cooling_rate;
                IIC_Write(EEP_INDEX_COOLING_RATE, (u8 *)&_cooling_rate, 2);
            }
            init_measure = 0;
            //sprintf(debug_text,"------> STOP C | %d | %d | %d",_cooling_rate, smart_recovery_cooling_rate,smart_recovery_heating_rate);
            //debug_print(debug_text,0);
        }
        else 
        {
            init_measure = 0;
        }
        last_cool_stage = current_cool;
    }
}



void smart_recovery_run()
{
    char debug_text[50];
    int day;
    int idx;
    s32 time_to_setpoint = _get_next_schedule(SysPara.ProgramMode, &day, &idx);
    u16 heat_setpoint    = SysPara.Schedule[day][idx].HeatSetTemp;
    u16 cool_setpoint    = SysPara.Schedule[day][idx].CoolSetTemp;
    u16 current_temp     = SysPara.RoomTemp;

    if (time_to_setpoint == -1 || time_to_setpoint > SMART_RECOVERY_TIME_LIMIT) //Ignore any recovery state more than an hour before any schedule
    {
        sprintf(debug_text,"------> NR | TTS: %d | %d | %d",time_to_setpoint,smart_recovery_cooling_rate,smart_recovery_heating_rate);
        debug_print(debug_text);
        return;
    }

    if (current_temp > cool_setpoint)
    {
        s32 time_to_recover = ((current_temp - cool_setpoint) * smart_recovery_cooling_rate)/10;
        if (time_to_recover >= time_to_setpoint)
        {
            sprintf(debug_text,"------> TTR: %d | TTS: %d | %d | %d",time_to_recover,time_to_setpoint,smart_recovery_cooling_rate,smart_recovery_heating_rate);
            _turn_on_recovery_stage(MODE_COOLING);
        }
        else
        {
            sprintf(debug_text,"------> NR | TTR: %d | TTS: %d | %d | %d",time_to_recover,time_to_setpoint,smart_recovery_cooling_rate,smart_recovery_heating_rate);
        }
    }
    else if (current_temp < heat_setpoint)
    {
        s32 time_to_recover = ((heat_setpoint - current_temp) * smart_recovery_heating_rate)/10;
        if (time_to_recover >= time_to_setpoint)
        {
            sprintf(debug_text,"------> TTR: %d | TTS: %d | %d | %d",time_to_recover,time_to_setpoint,smart_recovery_cooling_rate,smart_recovery_heating_rate);
            _turn_on_recovery_stage(MODE_HEATING);
        }
        else
        {
            sprintf(debug_text,"------> NR | TTR: %d | TTS: %d | %d | %d",time_to_recover,time_to_setpoint,smart_recovery_cooling_rate,smart_recovery_heating_rate);
        }
    }
    else
    {
        sprintf(debug_text,"------> ON TEMPERATURE | %d | %d",smart_recovery_cooling_rate,smart_recovery_heating_rate);
    }
    debug_print(debug_text);
}

# 2025-03-19
https://medium.com/@wide4head/modbus-crc-in-c-how-to-dea119940256
https://www.neoteo.com/wacup-winamp-rescatado-por-la-comunidad/
https://www.instructables.com/DIY-Yagi-Antenna-for-LoRa/?utm_source=newsletter&utm_medium=email
https://github.com/soulscircuit/pilet
https://www.kickstarter.com/projects/soulscircuit/pilet-opensource-modular-portable-mini-computer

# 2025-04-08

# 2025-04-10

"schedules": {
          "1": {
            "enabled": true,
            "time": "06:00",
            "recurring": [
              "weekdays"
            ],
            "action": {
              "type": "SET_TEMPERATURE_MODE",
              "cool_setpoint": 72.0,
              "heat_setpoint": 69.0
            },
            "occupied": false
          },
          "2": {
            "enabled": true,
            "time": "07:00",
            "recurring": [
              "sat"
            ],
            "action": {
              "type": "SET_TEMPERATURE_MODE",
              "cool_setpoint": 72.0,
              "heat_setpoint": 69.0
            },
            "occupied": false
          },
          "3": {
            "enabled": true,
            "time": "09:00",
            "recurring": [
              "sun"
            ],
            "action": {
              "type": "SET_TEMPERATURE_MODE",
              "cool_setpoint": 72.0,
              "heat_setpoint": 69.0
            },
            "occupied": false
          },
          "4": {
            "enabled": true,
            "time": "21:00",
            "recurring": [
              "sun"
            ],
            "action": {
              "type": "SET_TEMPERATURE_MODE",
              "cool_setpoint": 79.0,
              "heat_setpoint": 61.0
            },
            "occupied": false
          },
          "5": {
            "enabled": true,
            "time": "22:00",
            "recurring": [
              "mon",
              "tue",
              "wed",
              "thu",
              "fri",
              "sat"
            ],
            "action": {
              "type": "SET_TEMPERATURE_MODE",
              "cool_setpoint": 79.0,
              "heat_setpoint": 61.0
            },
            "occupied": false
          }
        }
      },

# 2025-04-11


# 2025-04-22

# 2025-05-22
* Minimum 4 years of professional experience developing software in modern C++ (C++11 or later) for embedded or IoT systems.
* Strong understanding of embedded systems architecture and constrained environments, including memory and power limitations.
* Experience developing device drivers, hardware abstraction layers (HAL), or middleware for microcontrollers (e.g., ARM Cortex-M).
* Hands-on experience working with real-time operating systems (RTOS) or bare-metal systems.
* Solid knowledge of communication protocols such as MQTT, CoAP, BLE, Zigbee, or UART/SPI/I2C.
* Proficiency in debugging embedded systems using tools like logic analyzers, oscilloscopes, or hardware simulators.
* Familiarity with cross-compilation toolchains, build systems (e.g., CMake), and CI/CD pipelines for embedded projects.

# 2025-05-26
## How to fix monuconfig in old idf project:
add "int" before main(){} in file tools/kconfig/lxdialog/check-lxdialog.sh
## HOw to wait connection on project
```
    EventBits_t bits = xEventGroupWaitBits(
        mqtt_event_group,                    // Event group handle
        BUDD_MPA_MQTT_CONNECTED_BIT,        // Bits to wait for
        pdFALSE,                            // Don't clear bits on exit
        pdFALSE,                            // Wait for ANY bit (not all)
        portMAX_DELAY                       // Wait indefinitely
    );
    if (bits & BUDD_MPA_MQTT_CONNECTED_BIT) {
        ESP_LOGI(TAG, "MQTT is now connected!");
    } else {
        ESP_LOGE(TAG, "Unexpected event group state");
    }
```
## Set fixed IP in ESP32 Ethernet interface
```
        tcpip_adapter_dhcpc_stop(TCPIP_ADAPTER_IF_ETH);

        tcpip_adapter_ip_info_t ip_info;
        IP4_ADDR(&ip_info.ip, 192, 168, 2, 100);
        IP4_ADDR(&ip_info.gw, 192, 168, 2, 1);
        IP4_ADDR(&ip_info.netmask, 255, 255, 255, 0);

        ESP_ERROR_CHECK(tcpip_adapter_set_ip_info(TCPIP_ADAPTER_IF_ETH, &ip_info));
```
## Lora OTA code (in progress)
```
    //uint8_t ota_response[20];
    //size_t  ota_response_len;

        //ota_response_len = 0;
        //if (esp_ota_update_task(ota_response, &ota_response_len))
        //{
        //    bool ota_run = true;
        //    uint64_t last_ota_package = 0;
        //    xTimerStop( xPubMeasureTimer, 0 );
        //    while (ota_run)
        //    {
        //        esp_task_wdt_reset();
        //        if (ota_response_len || esp_ota_update_task(ota_response, &ota_response_len))
        //        {
        //            last_ota_package = esp_timer_get_time()/1000;
        //            bf_pkg_t packet;
        //            bf_pkg_multi_data_context_t context = {0}; // Initialize context
        //            bf_pkg_status_t status;
        //            status = bf_pkg_prepare_data(&packet,
        //                                        &context,
        //                                        BF_MPA_PAYLOAD_OTA,
        //                                        ota_response,
        //                                        ota_response_len);
        //            ota_response_len = 0;
        //            if (status == BF_PKG_SUCCESS)
        //            {
        //                lora_send((char*)&packet, packet.length + BF_PKG_HEADER_SIZE);
        //                ESP_LOGW(TAG, "%s: SEND OTA ACK", __func__);
        //                vTaskDelay(250 / portTICK_RATE_MS);
        //            }
        //        }
        //        if (0)
        //        {
        //            ota_run = false;
        //            xTimerStart( xPubMeasureTimer, 0 );
        //        }

        //        if (esp_timer_get_time()/1000 - last_ota_package > 10000)
        //        {
        //            char P = 'N';
        //            lora_send(&P, 1);
        //            last_ota_package = esp_timer_get_time()/1000;

        //        }
        //        vTaskDelay(10);
        //    }
        //}
```

# 2025-06-11
Reporte fedex C193695658

# 2025-06-22
Get esp-clang
Instalar el ultimo release del siguiente repositorio
https://github.com/espressif/llvm-project/releases/

# 2025-06-24
Auditoría OSDE 2614693700


# 2025-07-27
