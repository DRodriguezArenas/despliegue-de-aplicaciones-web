## 1.Instale en una máquina virtual un sistema operativo con base Linux (se recomienda Debian o Ubuntu) e instale apache2.

![debian](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/440f31ec-c96e-4cde-a3fc-796a34871087)


![apache2](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/f698ff42-d477-4f37-9548-c8d3a48ad125)


## 2.Explique con sus palabras que es una petición GET, POST, PUT y DELETE, remarcando sus diferencias. 

- GET: se utiliza para obtener información del servidor.
- POST: se utiliza para enviar información al servidor.
- PUT: se utiliza para actualizar o modificar un recurso existente del servidor.
- DELETE: se utiliza para eliminar un recurso existente en el servidor.


## 3.Cambie del puerto 80 al puerto 4444 el servidor apache2. Muestra desde el navegador su funcionamiento adjuntando una captura de pantalla. 

![4444](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/fef380af-d8bc-4f0c-98eb-d98d4510d2f6)

![4444_](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/879f95b5-bb94-4c92-921d-9ef1eb7d9d31)

![localhost](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/52b33705-de53-49d3-9206-27d064941ed8)



## 4.Instale un certificado SSL y configure su Apache para servir contenido a través de HTTPS en el puerto 4444. Muestre desde el navegador cómo se muestra el sitio web como "seguro" (aunque sea un certificado autofirmado)

![ssl](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/5a5d8783-5b71-4267-a07d-2ef80341a0c6)

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/04d5018b-0a4f-4e13-b5e5-7960f8a03000)

##  5.¿Dónde se encuentran los ficheros de configuración de Apache2?

• Ubicación principal.
- /etc/apache2/

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/a73b7852-38b2-4bd2-b2b2-f79b889d9a76)

• Explora el archivo apache2.conf. Identifica las secciones principales y describe
su propósito.

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/7f94106d-91fe-42c6-8c0c-61f47217ea36)

- Su propósito es personalizar el comportamiento del servidor.


• sites-available y sites-enabled: Explica la diferencia entre estos dos directorios
y cómo funcionan juntos.

- "sites-available" contiene los archivos de configuración de los sitios web disponibles, mientras que "sites-enabled" contiene enlaces simbólicos a los archivos de configuración de los sitios web activos. Al crear un enlace simbólico desde "sites-available" a "sites-enabled",
se habilita un sitio web.


• mods-available y mods-enabled: Explica la diferencia entre estos dos
directorios.

- "mods-available" contiene los archivos de configuración de los módulos disponibles, mientras que "mods-enabled" contiene enlaces simbólicos a los archivos de configuración de los módulos activos. 

## 6.¿Dónde se encuentran los ficheros de ejecución de Apache2?
• Ubicación principal

- /usr/sbin

• Control del servicio: Utiliza el binario de ejecución para iniciar, detener,
recargar y reiniciar el servidor Apache2 explicando la diferencia entre cada uno
de los comandos utilizados.

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/7d4b0102-be1c-4bfb-ac05-b098f3c84e93)

- "sudo service apache2 start" inicia el servidor Apache2.
- "sudo service apache2 stop" se utiliza para detener el servidor Apache2.
- "sudo service apache2 reload" se utiliza para recargar la configuración del servidor Apache2 sin detenerlo por completo.
-  "sudo service apache2 restart" se utiliza para detener y luego iniciar nuevamente el servidor Apache2.

• Comprobación de sintaxis: Usa el binario de Apache para verificar la sintaxis
de tu configuración. Esto es útil para asegurarse de que no haya errores antes
de reiniciar el servidor.

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/ef96339a-eb09-4597-9e5f-fd5d9911e92f)


## 7.¿Dónde se encuentran los ficheros de monitorización de Apache2?
• Ubicación principal

- /var/log/apache2/

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/95b1f661-a04c-4be0-b83a-40ea709d61b9)


• error.log y access.log: Explica la diferencia entre estos dos archivos. Abre y
revisa las entradas recientes en cada uno de ellos.

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/6bd80072-8433-4031-9231-a4e5c8af8d69)

- error.log registra errores y advertencias relacionados con el servidor Apache2.
- access.log registra información sobre las solicitudes entrantes al servidor.

• Rotación de logs: Investiga cómo funciona la rotación de logs en Apache2.
¿Por qué es importante? ¿Cómo se configura?

- Es importante para ahorrar espacio en el disco.
- Se configura a través del módulo "logrotate".
  
• Monitorización en tiempo real: Utiliza herramientas como tail -f para monitorear
en tiempo real los accesos a tu servidor web y posibles errores.

- ![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/e5dd2ee9-3eb3-4cf2-9260-4341ea4905f7)


• Análisis de logs: Instala y usa herramientas como goaccess para analizar y
obtener estadísticas visuales a partir de tus logs de Apache2.

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/1e04f3cb-7931-4147-80bc-b07ac917fe48)

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/fd859109-2e82-42ff-a0b9-a46f485a336f)


## 8.¿Qué es un Firewall? ¿Para qué sirve? ¿Por qué es necesario? 
Instale y configure un Firewall en la máquina virtual para que solo permita tráfico HTTP y HTTPS. Bloqueetodo el resto de los puertos y demuestre su funcionamiento

- Un firewall es un componente de seguridad de red que protege sistemas y redes controlando el tráfico de datos entre ellos y el mundo exterior.
- Sirve para prevenir amenazas cibernéticas.
- Es necesario debido a la creciente amenaza de ataques cibernéticos.



![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/a432477e-8fd8-4f75-88df-b2b75a46637d)


![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/34db26a7-f8cb-478b-b05d-a63f4fac7603)


