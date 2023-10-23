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


