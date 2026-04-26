
##Clase 3
###GitHub y SSH

###Que es GitHub?
Es una plataforma en la nube que funciona como red social para devs,
permite alojar y gestionar proyectos usando Git como base.
No es lo mismo que Git, Git es la herramienta que crea los "checkpoints"
y GitHub es simplemente donde esos checkpoints viven y se comparten.

###SSH vs HTTPS
Con HTTPS cada vez que quieras subir algo te va a pedir autenticación,
token, contraseña... básicamente un martirio cada vez.
Con SSH configuras una key en tu máquina una sola vez y la registras en
GitHub, después de eso ya no te molesta más. Por eso siempre se usa SSH.

###Configurar SSH
....
....
Copias el output del cat, vas a GitHub → Settings → SSH and GPG Keys →
New SSH Key, le pones un nombre (ej: "mi-laptop") y pegas la key.
....
#Generar la key
```ssh-keygen -t ed25519 -C "tu-correo@email.com"
#Ver la key pública para copiarla
cat ~/.ssh/id_ed25519.pub
#Verificar que la conexión funciona
ssh -T git@github.com
....
```
###Crear un repositorio en GitHub
Vas a github.com/TuUser?tab=repositories → New → le pones nombre
(y descripción si quieres) → Create Repository. Eso es todo.

###Conectar tu repo local con GitHub
Ojo: ya debes tener git init y al menos un commit antes de esto.
....
```git remote add origin git@github.com:TuUser/TuRepo.git
#"origin" es simplemente el apodo que le da git a esa URL por defecto
git branch -M main
git push -u origin main
....

###Clonar un repo
....
#La forma correcta (SSH)
git clone "git@github.com:TuUser/TuRepo.git"
#Si lo clonaste con HTTPS por accidente, cámbialo con:
git remote set-url origin "git@github.com:TuUser/TuRepo.git"
#Ver a qué remoto está conectado tu repo
git remote -v
....

###Subir y bajar cambios
....
#Subir tus commits a GitHub
git push origin <rama>
#Traer los commits que hay en GitHub a tu máquina
git pull origin <rama>
```
....
