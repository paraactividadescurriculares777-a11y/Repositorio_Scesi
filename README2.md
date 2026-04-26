#Trabajo Individual 
Dana sainz Rubin de Celis

##Clase2
###Los estados de Git
####Directorio de trabajo:
Mi targeta local (La carpeta común), Creas modificas o eliminas ficheros,
 pero git aún no lo tiene asegurado.
####Area Temporal(stage Area):
Significa area de espera (preparado), añadiendo 
a tus archivos
####Repositorio Local(Confirmado):
 Son los archivos ya guardados que tienen su ID
(hash) y son parte de la historia.

###Directorio de trabajo (Modificado):

####Untracked:
Lo ve pero no tiene una version antigua (cuando se habre un nuevo archivo sin seguimiento)
####Modified:
Edita ya teniendo una version previa
###Comando para ver la fase:
git status:Estados de mis archivos 
###Repositorio Local (Confirmado):
Esta es la ultima fase que es la de guardado 
```git commit -m "mensaje"
```
Deshace el ultimo commit:
```
gir reset --solf HEAD-1
```

###Comandos Usados:
gitignore:Para que Git ignore el archivo y no lo supervise ni lo comparta.
gitAdd <archivo>: Agrega todos los archivos que esten observados por GIT
git restores --staged <archivo> (si quieres sacar un archivo des stage area para volveral estado anterior) 
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
(verbos descriptivos add,change,Fix, Remove, etc) (git commits en inglés)
(usa como maximo 50 caracteres)
(Usa un prefijo para los commits)
(No uses punto final ni suspensivos en tus mensajes)
```
git commit -m "Add"
(git commit -amend -m "Creado el .gitignore"cambia el id )
