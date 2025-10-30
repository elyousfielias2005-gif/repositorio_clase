# Repaso Linux

## Capitulo 2 - Ficheros y directorios

Directorios mas importantes de un fichero Linux

![image-20250925170330802](./imagenes/image-20250925170330802.png)





## Ejercicios

### 1. ¿En qué directorio se encuentran los ficheros de configuración del sistema?

Primero hay que usa el`cd /etc` y al presionar "Enter" hay que escribir `ls`

```
cd /etc
ls
```

![Captura de pantalla 2025-09-29 161233](./imagenes/Captura%20de%20pantalla%202025-09-29%20161233.png)

### 2. Para entrar en un sistema Linux hace falta a) nombre de usuario, contraseña y dirección IP, b) nombre de usuario y contraseña o c) únicamente una contraseña.

B) Nombre de usuario y contraseña



### 3. Muestra el contenido del directorio actual.

En este caso valdría con escribir `pwd` y ejecutarlo una vez hecho

```bash
pwd
```

![Captura de pantalla 2025-09-29 162940](./imagenes/Captura%20de%20pantalla%202025-09-29%20162940.png)

### 4. Muestra el contenido del directorio que esta justo a un nivel superior

En este caso hay que escribir `cd ..` y al ejecutar escribir `ls` 

```bash
cd ..
ls
```

![Captura de pantalla 2025-09-29 163555](./imagenes/Captura%20de%20pantalla%202025-09-29%20163555.png)



### 5. ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo

Nací un viernes

```bash
sudo apt install ncal
cal 12 2005
```





### 6. Muestra los archivos del directorio /bin



### 7. Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin a) con una sola línea de comando, b) moviéndote paso a paso por los directorios y c) con dos líneas de comandos.



### 8. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

En este caso hay que escribir este comando:

```bash
ls -R /etc/
```



### 9. Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.





###  10. Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

Este caso se hará de esta manera:

```bash
ls -Slh /etc
```

![Captura de pantalla 2025-10-02 163622](./imagenes/Captura%20de%20pantalla%202025-10-02%20163622.png)



### 11. Muestra todos los archivos del directorio /bin ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc

```bash
ls -Sshr /bin


```

![Captura de pantalla 2025-10-02 164033](./imagenes/Captura%20de%20pantalla%202025-10-02%20164033.png)



### 12. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta absoluta.

```bash
ls /
```

![Captura de pantalla 2025-10-02 164303](./Captura%20de%20pantalla%202025-10-02%20164303-1761850677106-17.png)

### 13. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta relativa. Suponemos que el directorio actual es /home/elena/documentos.

(Este lo copie)![Captura de pantalla 2025-10-02 164303](./imagenes/Captura%20de%20pantalla%202025-10-02%20164303.png)

```bash
ls ../../..
```





### 14. Crea un directorio gastos dentro del directorio personal 

```bash
mkdir gastos
```

![Captura de pantalla 2025-10-02 170131](./imagenes/Captura%20de%20pantalla%202025-10-02%20170131.png)



### 15. ¿Qué sucede si se intenta crear un directorio dentro de /etc?

Se recibirá un error de permiso denegado o acceso denegado diría yo.



### 16. Muestra el contenido del fichero.

```bash
cat /etc/fstab
```

![Captura de pantalla 2025-10-02 170710](./imagenes/Captura%20de%20pantalla%202025-10-02%20170710.png)



###  17. Muestra las 10 primeras lineas del fichero /etc/bash.bashrc

```bash
head /etc/bash.bashrc
```

![Captura de pantalla 2025-10-02 171337](./imagenes/Captura%20de%20pantalla%202025-10-02%20171337.png)



### 18. Crea la estructura de directorios del pdf dentro del directorio de trabajo personal

Hay que hacerlo con esta estructura

```bash
mkdir multimedia
cd multimedia
mkdir musica imagenes video presentaciones
cd imagenes
mkdir personales otras
```

![Captura de pantalla 2025-10-02 171656](./imagenes/Captura%20de%20pantalla%202025-10-02%20171656.png)

### 19. Crea un fichero vacío dentro del directorio **música** con nombre **estilos_favoritos.txt**

```bash
cd
cd multimedia
touch estilos_favoritos.txt
```

![Captura de pantalla 2025-10-06 155619](./imagenes/Captura%20de%20pantalla%202025-10-06%20155619.png)



###  20. Utiliza tu editor preferido para abrir el fichero 'estilos_favoritos.txt' e introduce los estilos de música que mas te gusten.

Usare en este caso Nano

```bash
nano estilos_favoritos-txt
//Escribir lo que tienes que escribir. Ctrl+o para guardar y ctrl+x para salir

```

![Captura de pantalla 2025-10-06 155952](./imagenes/Captura%20de%20pantalla%202025-10-06%20155952.png)

### 21. Muestra todo el contenido de estilos_favoritos.txt

```bash
cat estilos_favoritos.tx![image-20251006160705044](./../../AppData/Roaming/Typora/typora-user-images/image-20251006160705044.png)
```

![Captura de pantalla 2025-10-06 160702](./imagenes/Captura%20de%20pantalla%202025-10-06%20160702.png)

### 22. Muestra las 3 primeras líneas de estilos_favoritos.txt

```bash
head -n3 estilos_favoritos.txt
```

![image-20251006161052641](./../../AppData/Roaming/Typora/typora-user-images/image-20251006161052641.png)

![Captura de pantalla 2025-10-06 161046](./imagenes/Captura%20de%20pantalla%202025-10-06%20161046.png)



## Capitulo 3



### 1. Muestra todos los archivos del directorio actual que son imágenes jpg.

```bash
ls *.jpg
```



### 2. Muestra todos los archivos del directorio /usr/bin que empiecen por la letra j.

```bash
ls /usr/bin/j*
```

![Captura de pantalla 2025-10-06 162347](./imagenes/Captura%20de%20pantalla%202025-10-06%20162347.png)

### 3. Muestra los archivos que empiecen por k y tengan una a en la tercera posición, dentro del directorio /usr/bin.

```bash
ls /usr/bin/k?a*
```



### 4,  Muestra los archivos del directorio /bin que terminen en n.

```bash
ls /bin/*n
```

![Captura de pantalla 2025-10-06 163254](./Captura%20de%20pantalla%202025-10-06%20163254-1761850858689-37.png)

### 5. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva.

```bash
ls -R /etc
```



![Captura de pantalla 2025-10-06 163659](./imagenes/Captura%20de%20pantalla%202025-10-06%20163659.png)





### 6. Crea un directorio en tu directorio de trabajo con nombre prueba. Copia el archivo gzip del directorio /bin al directorio prueba. Crea un duplicado de gzip con nombre gzip2 dentro de prueba.



```bash
mkdir prueba
cp /bin/gzip prueba
cd prueba/
cp gzip gzip2
```

![Captura de pantalla 2025-10-06 165342](./imagenes/Captura%20de%20pantalla%202025-10-06%20165342.png)



### 7. Cambia el nombre de prueba a prueba2. Crea prueba3 en el mismo nivel que prueba2 y mueve todos los ficheros de prueba2 a prueba3. Borra prueba2.

```bash
cd ..
mv prueba prueba2
mkdir prueba3
mv prueba2/* prueba3/
rmdir prueba2

```

![Captura de pantalla 2025-10-06 165403](./imagenes/Captura%20de%20pantalla%202025-10-06%20165403.png)

### 8. Crea un fichero vacío con nombre “*?Hola caracola?*”. ¿Se puede? En caso de que se pudiera, ¿sería recomendable poner nombres así? Razona la respuesta.

Técnicamente se podría, pero no es lo mas recomendable

```bash
touch \*\?Hola\ caracola\?\*
```

![Captura de pantalla 2025-10-06 170630 - copia](./imagenes/Captura%20de%20pantalla%202025-10-06%20170630%20-%20copia.png)

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































