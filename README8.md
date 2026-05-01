#Trabajo Individual
Dana Sainz Rubin de Celis.
 
##Clase8
###git stash — Guardar cambios temporalmente:
git stash cuando otro PR tocó algo que tú también modificaste, y
 necesitas "limpiar" tu área de trabajo antes de actualizar.
#### Guardar cambios temporalmente
git stash

#### Guardar con un mensaje descriptivo
git stash -m "algo"

#### Ver todos los stashes guardados
git stash list

#### Recuperar el último stash guardado
git stash pop
###¿Cuándo usarlo?
Cuando se aprueba un PR distinto al tuyo que tocó los mismos archivos:

Haz git stash para guardar tus cambios
Actualiza tu rama con el nuevo estado del proyecto
Recupera tus cambios con git stash pop
Resuelve los conflictos si los hay
### git diff — Ver diferencias:
#### Ver todos los cambios sin stagear
git diff

#### Ver todos los cambios sin stagear (carpeta actual)
git diff .

#### Ver cambios de un archivo específico
git diff archivo

#### Ver lo que ya está en el staging area (listo para commit)
git diff --staged .

#### Ver staging de un archivo específico
git diff --staged archivo

#### Comparar dos ramas entre sí
git diff rama1 rama2
###Buena práctica: borrar la rama después del merge:
Una vez que el PR fue mergeado a main o develop,
 elimina la rama para mantener el repositorio limpio.
#### Borrar rama local
git branch -d feature/mi-rama

#### Borrar rama remota
git push origin --delete feature/mi-rama
En GitHub también puedes activar la opción "Delete branch" 
automáticamente después de cada merge en la configuración del repositorio.
