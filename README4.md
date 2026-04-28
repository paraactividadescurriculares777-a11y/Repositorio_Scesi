#Trabajo Individual
##Clase4
Dana Sainz Rubin de Celis.
###Remote SSH Multiple y Chackout
###Git Remote:
Nos permite mover nuestra informacion con repositorios remotos.
####Comandos Utiles:
```
git remote -v (Nos permite ver las URLs exactas donde apunta nuestro repo)
git remote add <apodo> "url"(Vincula el repo local con el de la nube)
git remote set-url<apodo>"url" (Cambia el url donde apunta nuestro repo)
```
###Multiples SSH:
Nos permite compartir nuestros archivos con varias cuentas teniendo en cuenta que las claves serán diferentes para cada 
cuenta.
####Configurar Multiples SSH
1) Generamos la llave con otro nombre:
```
ssh-keygen -t ed25519 -C
"micorreo@gmail.com" -f ~/.ssh/id_miname
```
1)Creamos un archivo conf para que no se choquen las llaves
```
#### Cuenta Personal (la de siempre)
Host github.com
HostName github.com
User git
IdentityFile ~/.ssh/id_ed25519
#### Cuenta del otro correo
Host github-miname
HostName github.com
User git
IdentityFile ~/.ssh/id_miname
```
###Configurar Multiples SSH:
####Host: 
El apodo que le pones a la conexion.
git@........
####HostName: 
La direccion real de nuestro servidor 
github.com
####User:
El nombre de usuario del sistema remoto.
git.
####IdentityFile: 
Es la llave privada para ese Host especifico
3) Cerciorar que funciona:
```
ssh-T git@github-miname
```
###Configuraciones Locales:
Las configuraciones locales tienen preferencia a las globales, y estas solo funcionan dentro de su repositorio.
Para configuraciones locales (lo mismo pero sin flag --global:)
```
git config user.name "Mi nuevo Name"
git config user.email "micorreo@gmail.com"
```
(Haz el git Clen con el nombre del HOST correcto para la cuenta que estás usando)
###Git Checkout:
Head: Nuestro puntero o "lector" actual.
El Git Checkout es un comando con el cual podemos desplazar el HEAD hacia un punto en la historia o inclusive una
 rama distinta.
####Para que sirve?:
*Inspeccionar (ver el codigo de un commit antiguo)
*Restaurar (probar camvios sin alterar la rama principal)
*Experimentar (sin arruinar la rama principal)
*Cambiar (saltar de una rama a otra)
###El Estado "Detsched HEAD"
El Head apunta a una Raama (que puede moverse). Estando desacoplado apunta a un Commit directamente (que es fijo)
####Que quiere decir?
*Eres un espectador en el pasado.
*Puedes cambiar, escribir pero no tienes cuerpo "rama"
*Si te vas al presente sin "encarnar" en una rama nuestros cambios se pierden en el vacio.
###Cómo ir y volver de un commit?
hacia atrás:
```
git checkout<hash_antiguo>
```
Ultimo has de la rama:
git checkout<rama>
*Importante:* Si hiciste algo en este estado como ser un commit este desaparece salvo que lo guardes de esta forma:
```
git checkout<hash_commit_creado>
git checkout -b rama_nueva
```
###Buenas practicas para el Checkout:
####No trabajes mucho tiempo en 'Detached HEAD'
Procura no trabajar mucho mas de pocas lineas de código estando en 'Detached HEAD', es mejor crear una rama.
####Limpia tu directorio de trabajo:
Guarda los cambios que estas añadiendo en el presente antes de viajar a una rama antigua.
####Úsalo para aprender:
Aplicar Checkout con grandes proyectos es buena oportunidad para entenderlos.

SSH= (Secure Shell)

