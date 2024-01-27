# 🌐 Lab 1 - Redes de Computadoras 

## ¿Qué es una Red? 💻
Una red es aquella capaz de conectar a personas o equipos a partir de los puntos TX (Transmision) y RX (Recepcion)eutes de informaci[on. Usualmente a partir de un Router. 

## Tipos de Redes 💠
### PAN (Personal Area Network)
### LAN (Local Area Network) 
### WAN (Wide Area Network) 
### MAN (Metropolitan Area Network)

## Modelos TCP/IP y OSI
Aunque estos apuntes son principalmente para mi uso personal, se agradecen las contribuciones en forma de correcciones, sugerencias o recursos adicionales. Por favor, abre un issue o pull request para cualquier tipo de contribución.

### Modelo OSI 
Este modelo es correspondido a partir de distintas capas. 
1. Física
   Servidores Físicos, modelos de comunicación señas y direccionamiento transverso.
3. Enlace de Datos
4. Red
   Direccionamiento (o Routing) de las redes. 
5. Transporte
   Servicios de End-To-End, se asegura el control de flujo y se asocia el protocolo TCP y el protocolo UDP
6. Sesión
   Establece, gestiona y finaliza las sesiones de comunicación entre sesiones. Ej. Netbios, sistema básico de visualización de una red.
7. Presentación
   Compresión, codificación y cifrado directamente para la presentación al usuario. 
10. Aplicado
    La capa más cercana al usuario. El SMTP y el FTP.

Dentro de cada una de estas capas es posible encontrar la unidad de datos.
| Capa OSI | Unidad de Datos | Función |
|----------|-----------------|---------|
| 1. Física | Bit | Transmisión y recepción de datos brutos sobre medio físico |
| 2. Enlace de Datos | Trama | Detección y corrección de errores, acceso al medio |
| 3. Red | Paquete | Direccionamiento, encaminamiento y control de tráfico |
| 4. Transporte | Segmento | Transferencia fiable de datos end-to-end |
| 5. Sesión | Datos | Control de diálogos y conexiones |
| 6. Presentación | Datos | Traducción de datos, cifrado y compresión |
| 7. Aplicación | Datos | Interfaces y servicios para aplicaciones de usuario |


### Modelo TCP/IP 
Este modelo se refiere solamente a 4 tapas. 
- App Kayer
- Transport Layer
- Internet Layer
- Link Layer
Este se encuentra ligado al modelo OSI
| OSI Model         | TCP/IP Model |
|-------------------|--------------|
| Application Layer | Application Layer |
| Presentation Layer| Application Layer |
| Session Layer     | Application Layer |
| Transport Layer   | Transport Layer |
| Network Layer     | Internet Layer |
| Data Link Layer   | Link Layer |
| Physical Layer    | Link Layer |

## Protocolos 
Son aquellos que definen los detalles de como transmitir y entregar mensajes. 
Estos pueden ser TCP\IP, HTTP, etc. 
Ningun modelo es mejor que otro sin embargo, es necesario buscar una implementación bajo distintas 
necesidades. En el presente se utiliza el TCP-IP pues las capas se reducen. 
| Modelo OSI         | Modelo TCP/IP       | Familia de protocolo TCP/IP       |
|--------------------|---------------------|-----------------------------------|
| Capa de aplicación | Capa de aplicación  | HTTP, SMTP, FTP, DNS, SNMP, etc.  |
| Capa de presentación|                     |                                   |
| Capa de sesión     |                     |                                   |
| Capa de transporte | Capa de transporte  | TCP, UDP                          |
| Capa de red        | Capa de red         | IP, IGMP, ICMP                    |
| Capa de enlace de datos| Capa de acceso de red | Ethernet, Token Ring, ATM, Frame Relay |
| Capa física        |                     |                                   |

# Tipos de Cableado 
## Cableado Estructurado 
### Ventajas
- Es independiente de la información que se transmite
- Se gastan recursos en una sola estructura de cableado y no en varias
- Muy confiable
### Desventajas 
- Diferentes trazados de cableado
- Incopatibilidad de Sistemas
- Reinstalación para traslado

### Subsistemas de un cableado estructurado
Dentro de estos sistemas, se encuentran 7 divisiones. 
- Acometida
- Cuarto de Equipos
- Cableado vertical o Backbone
- Armario de Telecomunicaciones

  ## Cableado Horizontal
  Se extiende desde el area de trabajo WA hasta el cuarto de telecommunicaciones, pasando por una cruzada horizontal
  llamada Cross Connect.
  ## Cableado Vertical (O Backbone)
  - Ofrece interconexión entre el cuarto de servicios, al cuarto de equipo y  con el cuarto de telecomunicaciones
  ## Area de Trabajo
  El area de trabajo abarca la terminación del cableado horizontal en la salida de información hasta el equipo en el cual se está corriendo una aplicacion que se avoz, datos o control.
  ## Cuarto de Telecomunicaciones
  SU principal finalidad es la distribución del cableado horizontal, por tal razón atiended pisos individuales de edificios
  Se usan para conectar cableado horizontal con el backbone y con equipos de telecomunicaciones
  ## Cuarto de Equipos
  Tipicamente contienen una gran cantidad de equipos de telecomunicaciones que sirven a los ocupantes del edificio, terminaciones de cable.
  ünicamente debe guardar equipos diretamente relacionados con el sistema de telecomunicaciones y sistemas de soporte 
## Referencias
- [Título del Texto Principal], [Autor]
- [Título del Recurso Adicional], [Autor]
- [Enlace a Recurso en Línea]

## Licencia
[Tipo de Licencia Apropiada]

## Agradecimientos
Un agradecimiento especial a [Nombre del Instructor(a)] por su invaluable orientación y a mis compañeros en [Tu Universidad] por sus perspectivas y discusiones.

