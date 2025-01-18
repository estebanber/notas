- Requerimientos
  Modulo de gestion
  Administrar cosas (define fuente de datos)
  Administrar aplicaciones (define estructura de datos)
  Administrar soluciones (define instancia de base de datos e instancia de microservicio/parser)
  Administrar protocolos (define protocolos existentes)
  Administrar conectores bases de datos (define base de datos aceptadas)
  Levantar configuración y levantar microservicios para cada protocolo habilitado
- Módulo de procesamientos
  Broker de mensajes con un protocolo unico para todos los microservicios. Permite abrir un canal para cada servicio.
  Ejecuta reglas
  Ejecuta análisis de stream
  Mantiene sombras de cosas
  Responde solicitudes de aplicaciones externas (info de cosas, datos real time,estructura de base)
  Graba en base de datos de acuerdo a configuracion de app y solución
- Microservicios socket/parser
  Se encargan de gestionar las conexiones desde las cosas, procesar paquetes, responder ack, arma comando, traducir datos a protocolo comun.