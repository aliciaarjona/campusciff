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

   ![Nuevo colaborador] (https://github.com/aliciaarjona/campusciff/blob/master/10.png)

5. Merge directo

   git checkout master 
