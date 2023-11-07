
## 1. Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos para acceder a ellos. El nombre del primer dominio será daw.gimbernat.eug.es y el segundo tunombreyapellidos.gimbernat.eug.es, donde “tunombreyapellidos” contiene la inicial de tu nombre, el primer apellido, y la inicial de tu segundo apellido. De esta manera, si tu nombre es: Francisco Mesas Cervilla, el domino quedaría: fmesasc.gimbernat.eug.es. 
## • En el primer caso, daw.gimbernat.eug.es tendrá su directorio base en /var/www/daw/ conteniendo una página llamada index.html que ponga el nombre de la clase como título con un archivo css para aplicarle estilos al título. 
## • En el segundo caso, fmesasc.gimbernat.eug.es tendrá su directorio base en /var/www/fmesasc/ (el equivalente para vuestros nombres), conteniendo una página llamada index.html que contenga vuestro currículum aplicándole un estilo css para que se visualice correctamente. 
## Para ello, tendrás que crear un archivo de configuración (copiado de 000-default.conf) para cada uno de los dominios. Recuerda que con a2ensite puedes crear los enlaces simbólicos necesarios para añadir esta configuración a la ejecución de apache.


- daw

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/f71b254d-923e-4004-b796-be6cd65ddc5f)

- drodrigueza

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/77675b40-8578-4214-a239-1cbb30e31641)

- archivo configuración para cada uno de los dominios

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/4c71cba2-635d-4c5e-9a93-bc82027a6459)


- editar los archivos de configuración

-> daw.conf

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/e7cce794-e3af-4abb-84b2-a38d569015a0)

-> drodrigueza.conf

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/0dcff8ca-5a80-435b-bb08-0d729b1f79cc)


- habilitar los sitios y reiniciar apache

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/95d80b2e-414e-481d-8cc4-89e405e5d824)


- añadir los puertos

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/6886e9ce-6ab6-40d4-895c-eada70e84d72)


- acceder a cada web

- daw

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/4cdf00b8-640f-4b58-8e51-2df2ebcbf38b)

-drodrigueza  

![image](https://github.com/DRodriguezArenas/despliegue-de-aplicaciones-web/assets/144775859/3e6fa611-50d4-4174-a7c0-520cd5950f2d)

