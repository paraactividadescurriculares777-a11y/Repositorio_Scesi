#Trabajo Individual 
Dana sainz Rubin de Celis

##Clase2
###Los estados de Git
Directorio de trabajo: Creas modificas o eliminas ficheros
Area Temporal(stage Area):
Repositorio Local:
###Directorio de Trabajo (modificado): 
Es la carpeta común 
####Untracked:
Lo ve pero no tiene una version antigua (cuando se habre un nuevo archivo sin seguimiento)
####Modified:
Edita ya teniendo una version previa
###Comando para ver la fase:
git status:Estados de mis archivos 
###Comandos Usados:

```
git restore <archivo>(borra todo sin guardar y si se aplica a un archivo borrado con seguimiento este se restablece)
 git add README.md
 git status
gitignore (para ignorar archivos con el git)
git add <archivo> (guardar archivos y que se guarden en el auxiliar)
git add . (todo)
git restore --staged README.md (mandarlos a la fase de atras con staged o sino borra todo)
git add .gitignore
git log 
git reset --soft Nombre~1  (hace que el archivo retroceda en este caso 1) 
```
git commit: los arcivos que estan en staighet crea un punto de guardado de ese archivo en
 tu repositorio y ahora como estamos en main se guarda en main y sino en la rama en la que estamos
###Buenas practicas:
(hacer gits cortos con cambios simples, puesto que es la funcion de guardado)
(verbos descriptivos add,change.etc) (git commits en inglés)
(usa como maximo 50 caracteres)
(Usa un prefijo para los commits)
```
git commit -m "Add"
(git commit -amend -m "Creado el .gitignore"cambia el id )
