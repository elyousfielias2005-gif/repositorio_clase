# Ejercicios de creación y actualización de repositorios

### Ejercicio 1

```bash
git config --global user.name "Elias El Yousfi Aoudar"
git config --global user.email "Wjo94412@educastur.es"
```



![image-20251009165836184](./../../AppData/Roaming/Typora/typora-user-images/image-20251009165836184.png)



### Ejercicio 2

```bash
mkdir libro
cd libro
git init
ls -la
```

![image-20251009170627119](./../../AppData/Roaming/Typora/typora-user-images/image-20251009170627119.png)



### Ejercicio 3

```bash
git status
cat > indice.txt
Capítulo 1: Introducción a Git
Capítulo 2: Flujo de trabajo básico
Capítulo 3: Repositorios remotos
Ctrl+D
git status
git add indice.txt
git status
```



![image-20251009170931866](./../../AppData/Roaming/Typora/typora-user-images/image-20251009170931866.png)



### Ejercicio 4

```bash 
git commit -m "Añadido indice del libro"
git status
```

![image-20251009171118193](./../../AppData/Roaming/Typora/typora-user-images/image-20251009171118193.png)



### Ejercicio 5

```bash
cat > indice.txt
Capítulo 1: Introducción a Git
Capítulo 2: Flujo de trabajo básico
Capítulo 3: Gestión de ramas
Capítulo 4: Repositorios remotos
Ctrl+D
git diff
git add indice.txt
git commit -m "Añadido capítulo 3 sobre gestión de ramas"
```

![image-20251009171506325](./../../AppData/Roaming/Typora/typora-user-images/image-20251009171506325.png)



### Ejercicio 6

```bash
git show
git commit --amend -m "Añadido capitulo 3 sobre las ramas al indice."
git show
```



![image-20251009171700707](./../../AppData/Roaming/Typora/typora-user-images/image-20251009171700707.png)



# Ejercicios de manejo del historial de cambios

```bash
git log
mkdir capitulos
cat > capitulos/capitulo1.txt
Git es un sistema de control de versiones ideado por Linus Torvalds.
Ctrl+D
git add .
git commit -m "Añadido capítulo 1."
git log
```





