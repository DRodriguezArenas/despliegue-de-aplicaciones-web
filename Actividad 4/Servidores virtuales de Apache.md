
## 1. Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos para acceder a ellos. El nombre del primer dominio será daw.gimbernat.eug.es y el segundo tunombreyapellidos.gimbernat.eug.es, donde “tunombreyapellidos” contiene la inicial de tu nombre, el primer apellido, y la inicial de tu segundo apellido. De esta manera, si tu nombre es: Francisco Mesas Cervilla, el domino quedaría: fmesasc.gimbernat.eug.es. • En el primer caso, daw.gimbernat.eug.es tendrá su directorio base en /var/www/daw/ conteniendo una página llamada index.html que ponga el nombre de la clase como título con un archivo css para aplicarle estilos al título. • En el segundo caso, fmesasc.gimbernat.eug.es tendrá su directorio base en /var/www/fmesasc/ (el equivalente para vuestros nombres), conteniendo una página llamada index.html que contenga vuestro currículum aplicándole un estilo css para que se visualice correctamente. Para ello, tendrás que crear un archivo de configuración (copiado de 000-default.conf) para cada uno de los dominios. Recuerda que con a2ensite puedes crear los enlaces simbólicos necesarios para añadir esta configuración a la ejecución de apache.


- daw
![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/f71b254d-923e-4004-b796-be6cd65ddc5f)

- drodrigueza
![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/77675b40-8578-4214-a239-1cbb30e31641)

- archivo configuración para cada uno de los dominios
![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/4c71cba2-635d-4c5e-9a93-bc82027a6459)
