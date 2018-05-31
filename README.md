# owasp-goat-tests

## HTTP Protocol.

### Métodos

* GET
Fallo de seguridad:
No enviar información por GET (pasados por URL)

* HEAD

* POST

* PUT
PUT en Tomcat, crear archivos con este metodo JSP, y permite ejecutar código remoto.
En STRUTS tambien hubo vulnerabilidades.

* DELETE
Revisar permisos de 

* TRACE
Vulnerabilidad : Deshabilitar métodos desde server.
vulnerable a Cross Site Tracing XST

* OPTIONS
Lista metodos habilitados, probar s

### HEADERS

* Accept-Encoding: buena idea poner gzip

* Content-Type: Validación de subida de archivos.

* HSTS: protege comunicación por SSL
(herramienta delorean: )

* Set-Cookies: Que se destruyan cookies, que sean cifradas

* X-CSRF-Token

### Mensajes

## Metalenguaje XML

Se pueden realizar ataques basados en

## HTTPS
Usar TLS 1.2 o superior.
No usar certificados autofirmados.

## Tipos Autenticación

* básica
* Digest
* HTTPS client
* Form-Based
* Doble-Factor 

Desarrollar pensando en 2 capas de autenticación


## Arquitectura Web

Validaciones por JS
Validaciones dobles (via server y via frontend)

Es malo solo ofuscar sólo con base64
Preferir SHA256 o superior

Incluir Seguiridad en las distintas etapas de desarrollo de SW

Solicitar no indexaciones en ciertos recursos
Revisar perfiles de usuarios y hacer validaciones por cada uno de ellos para distintas funcionalidades de la app.

Fijación de SESION (Buscar en OWASP)

Tokens y cookies no predecibles

Revisar mensajes de errores no controlados.

## Diseños seguros
* de mensajes de error
* autenticación
* autorización
* separación de privilegios
* interacción con firewalls e IDS
(Revisar esto para evitar ataques automatizados)
* admin info sensible
    Revisar indexacion de apps webs
* auditoría y logging
Ataques de Fuerza Bruta, monitorear multiples requests
* análisis riesgo

# Seguridad de Diseño


# Desarrollo

Escalamiento vertical de privilegios
Escalamiento horizontal de privilegios:
    Transferencia de banco de otro usuario para realizar en nombre mio.

Manipular errores de forma adecuada, no exponer mensajes de error especificos al usuario

## Test de Seguridad Adicional


* Bloqueo de cuentas (sencillo)
* Funcionalidad de Captchas

## Test de Stress

## Test de Mutación de Datos

## Revisión de código

## Mantenimiento

## Owasp ESAPI (Enterprise Security API)
(Revisar code review guide)

# Reconocimiento

## OSINT

* Google
Dorks: Busqueda especifica y exhaustiva

EX: 
* site:.cl ext:sql "password"

* site:.cl inurl:wp-config.txt

* site:.cl inurl:"Hacked by"


* Shodan ** Buscador de servicios (shodan.io)

Ex:

* country:CL

## Tools
Wappalizer
Whatsrun

# IoT

# Fingerprint y Scan

* Nmap
* Netcat
* Acunetix
* Nikto
* Burp Suite
* netsparker

## Busqueda subdominios

* Sublist3r
* Aquatone
* Dirsearch
* Dirbuster

Para revisar que vulnerabildad buscar
exploit DB 

# Vulnerabilidades más Comunes

## Inyección

Modificando el content-type se puede , por ejemplo subir un archivo php como si fuese una imágen

## Autenticación
Credenciales por defecto 

Robo de Cookies o Sesion con XSS

## Autorización
Carencia de validaciones 

## OWASP

DVWA


XEE (XML External entities)

Revisar Buckets abiertos S3 para escritura.
Angular XSS
http://html5sec.org/

Owasp Testing Guide
