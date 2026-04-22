#Trabajo Individual

Dana Sainz Rubin de Celis
 
##Clase 1
###Que es GIT?
Es un sistema que nos permite controlar Versiones permitiendonos guardar 
archivos hacer ramas y formar puntos de retorno como "checkpoints"(lleva un historial de cambios) para 
conservar y modificar de manera local.
###Cómo nació GIT? 
Linus Toevalds fue el creador de Git que fue creado con el objetivo de 
gestionar el desarrollo del kernel de Linux al perder el acceso a la
 herramienta de BitKeeper. (Se presume que Linus desarrolló esta herramienta en dos semanas en cuanto se entero de la perdida del acceso a BitKeeper)
añadimos a esta informacion el hecho de que Bitkeeper era una herramienta de codigo cerrado "No usarás ni tu ni tus colaboradores otros además de mi".
 
###Cómo instalar GIT?
....
``` 
En mi caso usé los comandos:
sudo apt install git
git --version
sudo apt upgrade git
```
....
###Configuraciones Básicas
....
```
git config --global user.name "Dana Sainz Rubin"
git config --global user.email "202503425@est.umss.edu"
git config --list
git config --global --list
```
....
###Archivos que todo repo deberia tener 
####READMI.md
Es el manual de usuario (es lo primero que se lee al entrar a tu repositorio)
####.gitignome
Dicta que archivos no deben guardarse, sirve para subir archivos innecesarios
archivos temporales,contraseñas y configuraciones privadas.


