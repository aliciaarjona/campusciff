# EJERCICIO 1

1. Crear repositorio

	![Repositorio] (https://github.com/aliciaarjona/campusciff/blob/master/1.png)
	![Repositorio] (https://github.com/aliciaarjona/campusciff/blob/master/2.png)


2. Clonar

   git clone https://github.com/aliciaarjona/campusciff
   
3. Crear README.md 

   touch README.md
   
4. Hacer commit

   git add .
   git commit -m "inicio ejercicio"
   
5. Subir cambios al repositorio remoto

   git push origin master
   
6. - Crear fichero 

   touch privado.txt
   
   - Crear en repositorio local carpeta privada
   
   mkdir privada
   
7. - Ignorar archivos y la carpeta privada

   echo "privada.txt" > .gitignore
   echo "/Users/AliciaArjona/Desktop/MASTER/CURSO_NIVELACION/ENTREGA_EJER/GIT/campusciff/privada" >.gitignore
   
   - Añado los cambios
   
   git add .
   git commit -m "ignoro carpeta y fichero privada"
   
   Salida en pantalla:
   	[master b07ffd0] ignoro carpeta y fichero privada
 	3 files changed, 1 insertion(+)
 	create mode 100644 .README.md.swp
 	create mode 100644 .gitignore
 	create mode 100644 privado.txt 
 	
8. Añado fichero

    touch 1.txt
    git add .
    git commit -m "añado 1.txt"
    
9. Crear tag

    git tag v0.1
    
10. Subir cambios tag al repositorio remoto

    git push --tag origin master
    
11. Cuenta GitHub

    ![Foto] (https://github.com/aliciaarjona/campusciff/blob/master/3.png)
    ![Autentficación] (https://github.com/aliciaarjona/campusciff/blob/master/4.png)
    ![Autentficación] (https://github.com/aliciaarjona/campusciff/blob/master/5.png)
    ![Llave] (https://github.com/aliciaarjona/campusciff/blob/master/6.png)
    
12. rhuergo 

    ![Compañero] (https://github.com/aliciaarjona/campusciff/blob/master/7.png)

13. Crear tabla

    | NOMBRE | GITHUB |
    | ------ | ------:|
    | Roberto Huergo Burgos | https://github.com/rhuergo |
    
14. Colaborador a asanzdiego

    ![Nuevo colaborador] (https://github.com/aliciaarjona/campusciff/blob/master/8.png)
    ![Nuevo colaborador] (https://github.com/aliciaarjona/campusciff/blob/master/9.png)   

# EJERCICIO 2

1. - Crear una rama

   git branch v0.2
   
   - Posicionamiento a esa rama

   git checkout v0.2
Switched to branch 'v0.2'

2 y 3.  Añadir fichero a esta rama

    touch 2.txt
    git add .
    git commit -m "añadimos fichero 2.txt"

4. Subir cambios al repositorio remoto

   git push origin v0.2

   ![Branch] (https://github.com/aliciaarjona/campusciff/blob/master/10.png)

5. Merge directo

   git checkout master 
6, 7 y 8. Merge con conflicto
    
   vi 1.txt
   git add .
   git commit -m "hola en 1.txt"
   git checkout v0.2
   git add . 
   git commit -m "adios en 1.txt" 
   git checkout master
   git merge v0.2
    Auto-merging 1.txt
    CONFLICT (content): Merge conflict in 1.txt
    Automatic merge failed; fix conflicts and then commit the result.

9. listado con merge y no merge

   git branch --merged
    * master
   git branch --no-merged
    v0.2

10. Arreglar conflicto 

     Abrimos 1.txt y borramos lineas y dejamos hola y adios
     vi 1.xtx
     git add .
     git commit -m "cambios en 1.txt"
     
11. Borrar rama

    git tag v0.2
    git branch -d v0.2
        Deleted branch v0.2 (was 3ffc588).
        
12. Listado de cambios

    git list 
       *   5aeec88 (HEAD -> master) cambios en 1.txt
    |\
    | * 3ffc588 adios en 1.txt
    * | 444dec3 hola en 1.txt
    |/
    * b135ff8 (origin/master, origin/HEAD) update README_github.md
    * 77e8893 (origin/v0.2) añadimos fichero 2.txt
    * ed3c325 Update README_github.md
    * 407d82e Update README_github.md
    * a8f3a14 Add files via upload
    * bbfb0db Update and rename README.md to README_github.md
    * 7bdd8aa (tag: v0.1) añado 1.txt
    * b07ffd0 ignoro carpeta y fichero privada
    * 63a6f7c inicio ejercicio
    
13 y 14. Crear una organización

    ![Organización] (https://github.com/aliciaarjona/campusciff/blob/master/11.png)
    ![Organización] (https://github.com/aliciaarjona/campusciff/blob/master/12.png)
    
15. - En github he creado un repositorio "Customize pinned repositories" -> New llamado
    aliciaarjona.github.io.
    
    - Lo he clonado a mi local y ahi he creado un fichero index.html 
    
    MacBook-Pro-de-Alicia:GIT AliciaArjona$ cd aliciaarjona.github.io/
    MacBook-Pro-de-Alicia:aliciaarjona.github.io AliciaArjona$ echo "Hello World" > index.html
    MacBook-Pro-de-Alicia:aliciaarjona.github.io AliciaArjona$ git add --all
    MacBook-Pro-de-Alicia:aliciaarjona.github.io AliciaArjona$ git commit -m "Initial commit"
    MacBook-Pro-de-Alicia:aliciaarjona.github.io AliciaArjona$ git push -u origin master
