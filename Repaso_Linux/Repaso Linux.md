# Repaso Linux

## Capitulo 2 - Ficheros y directorios

Directorios mas importantes de un fichero Linux

![image-20250925170330802](C:/Users/2dawv10/AppData/Roaming/Typora/typora-user-images/image-20250925170330802.png)





## Ejercicios

### 1. ¿En qué directorio se encuentran los ficheros de configuración del sistema?

Primero hay que usa el`cd /etc` y al presionar "Enter" hay que escribir `ls`

```
cd /etc
ls
```

![image-20250929161236710](./../../AppData/Roaming/Typora/typora-user-images/image-20250929161236710.png)



### 2. Para entrar en un sistema Linux hace falta a) nombre de usuario, contraseña y dirección IP, b) nombre de usuario y contraseña o c) únicamente una contraseña.

B) Nombre de usuario y contraseña



### 3. Muestra el contenido del directorio actual.

En este caso valdría con escribir `pwd` y ejecutarlo una vez hecho

```bash
pwd
```



<img src="./../../AppData/Roaming/Typora/typora-user-images/image-20250929162940881.png" alt="image-20250929162940881" style="zoom:80%;" />

### 4. Muestra el contenido del directorio que esta justo a un nivel superior

En este caso hay que escribir `cd ..` y al ejecutar escribir `ls` 

```bash
cd ..
ls
```

![image-20250929163628489](./../../AppData/Roaming/Typora/typora-user-images/image-20250929163628489.png)

### 5. ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo

Nací un viernes

```bash
sudo apt install ncal
cal 12 2005
```

![image-20250929165738560](./../../AppData/Roaming/Typora/typora-user-images/image-20250929165738560.png)



### 6. Muestra los archivos del directorio /bin

```bash
cd /bin
ls
```





![Captura de pantalla 2025-09-29 170543](./../../Pictures/Screenshots/Captura%20de%20pantalla%202025-09-29%20170543.png)



### 7. Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin a) con una sola línea de comando, b) moviéndote paso a paso por los directorios y c) con dos líneas de comandos.



### 8. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

En este caso hay que escribir este comando:

```bash
ls -R /etc/
```

![image-20250929171754170](./../../AppData/Roaming/Typora/typora-user-images/image-20250929171754170.png)



### 9. Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.





###  10. Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

Este caso se hará de esta manera:

```bash
ls -Slh /etc
```

![image-20251002163625127](./../../AppData/Roaming/Typora/typora-user-images/image-20251002163625127.png)



### 11. Muestra todos los archivos del directorio /bin ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc

```bash
ls -Sshr /bin


```

![image-20251002164035716](./../../AppData/Roaming/Typora/typora-user-images/image-20251002164035716.png)



### 12. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta absoluta.

```bash
ls /
```

![image-20251002164308691](./../../AppData/Roaming/Typora/typora-user-images/image-20251002164308691.png)



### 13. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta relativa. Suponemos que el directorio actual es /home/elena/documentos.

(Este lo copie)

```bash
ls ../../..
```

![image-20251002165729591](./../../AppData/Roaming/Typora/typora-user-images/image-20251002165729591.png)



### 14. Crea un directorio gastos dentro del directorio personal 

```bash
mkdir gastos
```

![image-20251002170121094](./../../AppData/Roaming/Typora/typora-user-images/image-20251002170121094.png)

![image-20251002170133765](./../../AppData/Roaming/Typora/typora-user-images/image-20251002170133765.png)



### 15. ¿Qué sucede si se intenta crear un directorio dentro de /etc?

Se recibirá un error de permiso denegado o acceso denegado diría yo.



### 16. Muestra el contenido del fichero.

```bash
cat /etc/fstab
```

![image-20251002170712366](./../../AppData/Roaming/Typora/typora-user-images/image-20251002170712366.png)



###  17. Muestra las 10 primeras lineas del fichero /etc/bash.bashrc

```bash
head /etc/bash.bashrc
```

![image-20251002171349499](./../../AppData/Roaming/Typora/typora-user-images/image-20251002171349499.png)



### 18. Crea la estructura de directorios del pdf dentro del directorio de trabajo personal

Hay que hacerlo con esta estructura

```bash
mkdir multimedia
cd multimedia
mkdir musica imagenes video presentaciones
cd imagenes
mkdir personales otras
```



![image-20251002171659351](./../../AppData/Roaming/Typora/typora-user-images/image-20251002171659351.png)

### 19. Crea un fichero vacío dentro del directorio **música** con nombre **estilos_favoritos.txt**

```bash
cd
cd multimedia
touch estilos_favoritos.txt
```



![image-20251006155619457](./../../AppData/Roaming/Typora/typora-user-images/image-20251006155619457.png)



###  20. Utiliza tu editor preferido para abrir el fichero 'estilos_favoritos.txt' e introduce los estilos de música que mas te gusten.

Usare en este caso Nano

```bash
nano estilos_favoritos-txt
//Escribir lo que tienes que escribir. Ctrl+o para guardar y ctrl+x para salir

```

![image-20251006155954423](./../../AppData/Roaming/Typora/typora-user-images/image-20251006155954423.png)



### 21. Muestra todo el contenido de estilos_favoritos.txt

```bash
cat estilos_favoritos.tx![image-20251006160705044](./../../AppData/Roaming/Typora/typora-user-images/image-20251006160705044.png)
```



### 22. Muestra las 3 primeras líneas de estilos_favoritos.txt

```bash
head -n3 estilos_favoritos.txt
```

![image-20251006161052641](./../../AppData/Roaming/Typora/typora-user-images/image-20251006161052641.png)





## Capitulo 3



### 1. Muestra todos los archivos del directorio actual que son imágenes jpg.

```bash
ls *.jpg
```



### 2. Muestra todos los archivos del directorio /usr/bin que empiecen por la letra j.

```bash
ls /usr/bin/j*
```

![image-20251006162348382](./../../AppData/Roaming/Typora/typora-user-images/image-20251006162348382.png)

### 3. Muestra los archivos que empiecen por k y tengan una a en la tercera posición, dentro del directorio /usr/bin.

```bash
ls /usr/bin/k?a*
```



### 4,  Muestra los archivos del directorio /bin que terminen en n.

```bash
ls /bin/*n
```

![image-20251006163254919](./../../AppData/Roaming/Typora/typora-user-images/image-20251006163254919.png)

### 5. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva.

```bash
ls -R /etc
```



![image-20251006163700551](./../../AppData/Roaming/Typora/typora-user-images/image-20251006163700551.png)





### 6. Crea un directorio en tu directorio de trabajo con nombre prueba. Copia el archivo gzip del directorio /bin al directorio prueba. Crea un duplicado de gzip con nombre gzip2 dentro de prueba.



```bash
mkdir prueba
cp /bin/gzip prueba
cd prueba/
cp gzip gzip2
```

![image-20251006165343900](./../../AppData/Roaming/Typora/typora-user-images/image-20251006165343900.png)



### 7. Cambia el nombre de prueba a prueba2. Crea prueba3 en el mismo nivel que prueba2 y mueve todos los ficheros de prueba2 a prueba3. Borra prueba2.

```bash
cd ..
mv prueba prueba2
mkdir prueba3
mv prueba2/* prueba3/
rmdir prueba2

```

![image-20251006165405606](./../../AppData/Roaming/Typora/typora-user-images/image-20251006165405606.png)

### 8. Crea un fichero vacío con nombre “*?Hola caracola?*”. ¿Se puede? En caso de que se pudiera, ¿sería recomendable poner nombres así? Razona la respuesta.

Técnicamente se podría, pero no es lo mas recomendable

```bash
touch \*\?Hola\ caracola\?\*
```

![image-20251006170645407](./../../AppData/Roaming/Typora/typora-user-images/image-20251006170645407.png)

### 9. Crea un directorio con nombre multimedia_pruebas y copia en él todo el contenido del directorio multimedia. A continuación crea en multimedia/video/ dos ficheros, uno con nombre peliculas.txt y otro con nombre actores.txt. Edita el fichero peliculas.txt e introduce el nombre de tu película favorita. A continuación, crea en multimedia_pruebas/video/ otro fichero que también tenga por nombre peliculas.txt, edítalo y esta vez escribe el nombre de tus cinco películas favoritas. Ahora haz una copia de todo el contenido de multimedia en multimedia_prueba de tal forma que sólo se copien los contenidos nuevos, es decir, si hay coincidencia en el nombre de un archivo se respetará el que se haya modificado más recientemente. Para comprobar que se ha hecho todo correctamente, basta mirar si en multimedia_prueba/video está el archivo vacío actores.txt y además el archivo peliculas.txt debe contener 5 películas y no 1.

```bash
mkdir multimedia_pruebas
cp -R multimedia/* multimedia_pruebas/
cd multimedia /video/
multimedia/video touch peliculas.txt actores.txt
multimedia/video$ vi peliculas.txt
~/multimedia/video$ cd
cd multimedia_pruebas/video/
multimedia_pruebas/video$ vi peliculas.txt
multimedia_pruebas/video$ cd
 cp -Ru multimedia/* multimedia_pruebas/
```



### 10. Borra el directorio multimedia/imagenes/otras

```bash
rm -Ri multimedia/imagenes/otras/
```



### 11.  Mueve el archivo peliculas.txt, que está dentro de multimedia/video, al directorio que está justo a un nivel superior. Ahora el archivo debe llamarse mis_peliculas.txt en lugar de películas.

```bash
~$ cd multimedia/video/
~/multimedia/video$ mv peliculas.txt ../mis_peliculas.txt 
```



## Capitulo 4



|      |           |
| ---- | --------- |
| 654  |           |
|      | rwxrw-rw- |
|      | rwxrwxrwx |
| 520  |           |
| 764  |           |
|      | r--r----- |































