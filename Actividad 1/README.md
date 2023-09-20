3. Analiza los headers de las peticiones cuando inicias sesión en el Moodle y comprende
cómo se obtiene el token. Para ello, necesitamos saber de dónde salen TODOS los
datos sensibles que se envían.


![token](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/7dabd206-f6db-4a31-8c9f-64d7ef39c304)

Acceder a la página web del moddle, F1, "NETWORK", inicias sesión, "index.php" y opción de "payload".

4. ¿A qué puerto se reciben normalmente las peticiones del protocolo HTTP? ¿A qué
capa del modelo TCP/IP se encuentra el protocolo HTTP? ¿Y los protocolos TCP,
UDP, e IP?

- Se reciben normalmente en el puerto 80. El protocolo HTTP se encuentra en la capa 4 del modelo TCP/IP.
- Los protocolos TCP y UDP en la capa 4.
- Los protocolos IP en la capa 3.


5. ¿Cuál es el significado de la siguiente respuesta de un servidor?
HTTP/1.1 302 Found
- Se utiliza para informar al cliente que la página solicitada se ha movido temporalmente a una ubicación diferente.
Location: http://www.example.com/test/index2.php
- El serivodr está dndo la orden al cliente a redirigir su solicitud a la URL especificada en el encabezado "Location" para obtener el recurso deseado.
