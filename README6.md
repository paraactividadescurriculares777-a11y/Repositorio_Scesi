#Trabajo Individual
Dana Sainz Rubin de Celis
##Clase6

rama= caso limpio con hacer merch, cuando hay conflictos
###Git merge=
 significa fusion y permite fucionar ramas empezando a
 escribir sin afectar la rama principal 
###Merge a develove=
```
git checkout  develop (se mueven a la rama develop)
#git fech (mira las ramas de develop y todas las rams que tienen cambios) 
#git pull origin develop (trae todas las rams de develop a el repo local)
(trae todo lo que tiene develop en tu maquina, todas las de los demas tambien...se suben a develop)
(siempre git fech junto a develop para ver todos los trabajos de otros)
(si trabajo sin hacer eso se crean conflictos)
git merge --on-ff feature/header-landing (despues de / el nombre de tu rama)
(el comando de arriba hace un commit con el merch)
git log
git branch -D feature/header-landing (borrando la rama que ya esta en maina0)
git swich develop 
git merge --no-ff feature/footer-landing (si hay conflicos significa que han sobreescrito y no sabe sobre cual aplicar cambios )
nano index.html (entrar a los archivos con nano)
te muestra el HEAD el que tenemos nosotros en el develop antes del igual
es el codigo original y debajo hasta donde se cierra el >>> es el codigo que estas tratando de poner desde tu rama
```
####primero borro los simbolos extraños y borro lo que quiero
boror el codigo que no me sirve
*lo vemos con git status y nos muestra los que tuvieron conflictos
comflictos suceden cuando tocamos el archivo que difiere de otro que habian editado
*Una vez hacemos el arreglo manual debemos crear un commit
*luego eliminamos la rama 
*Si haces git pull no se soluciona 
forward(lo une todo plano, mergea sin un commit y desaparece mi rama)
 not fast forw
####git fech=
 Es el mirón, va a mi servidor con el repositorio remoto y si has hecho
git fech entonces ve todas las ramas viendo si hay cambios
(*informa si hubieron cambios o no*)
```
git pull origin develop 
git swich (te mueves a la rama y luego la traes)
git remote -v
git config --list
git config user.name "name"
git config --list
git fech (para checkear si subieron cambios)
git push origin develop (subir cambios)
git pull origin develop (traer todos los cambios para mi)
git checkout -b feature/name (ejemplo: feature/'update readme')
(las ramas se crean en feature ... ...)
git commit -m "docs:updare README.md"(documentamos)
!(*ruta...* ./assets?logo_scesi_dark_mode.svd)[logo SCESI]
git commit -m "Docs: Add picture"
///
```
####Otro participante
```
git feach
git switch -c "feature/hero-section"(esta creando un hero menu)
(toco el README)
(hizo su commit)
git add index


```
si tu no creas el repositorio creas git push -u origin feature/..
 para añadir sin pedir permiso al creador la primera vez que lo subas
ya de ahi en adelante no es necesario
``` 
se hace fech y pull primero cuando cambiemos la rama antes de subir
si hicieron un push antes de hacer fech pull no tengo dos cambios y se crean conflictos de linea de tiempo
y anunciemos el fech develop

git swich develop 
(mostrando cambios )
git swich feature/'update-readme' 
antes de crear avance fucionar develop 
si hemos hecho en una version vieja he ir suviendo a develop 
para no sufrir tanto en el develop
```
*el develop es el nombre de la rama principal antes de subir a produccion*
trabajar sin pull recuest si son pequeños grupos

