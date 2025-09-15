# Comandos basicos
git --version version de git

## Comandos para configuracion inicial del repositorio Para ingresar con nuestro usuario y email, se necesita cuenta en github o alguna palataforma simila con git

git config --global user.name
git config --global user.email

## Inicializar el repositorio.

-- git init

## Al usarlo se crea el stagging area

## Conocer el area stagging

-- git status

-- git log(conocer los commits anterirores, fecha y correos)

## anadir archivos al stagging area y repositorio logal

-- git add . o git commit nombre nombre 

## Subir lo cambios

-- git commit -m "Mensaje"

## Con este comando no saltamos el area de stagginga (no recomendado)

-- git commit -am "Mensaje"

// enviar al repositorio remoto

## Ingresar repositrorio remoto

-- git remote add origin (origen)
-- git remote remove origin

## Cambiar el nombre de la rama

-- git branch -m MAIN

## Este solo se ejecuta una ves, cuando cambiamos de remoto le damos el parametro -u origin main, despues solo sera git push

-- git push -u origin main


-- git push origin head (creara una nueva rama)

## Modificar y ver diferencias

-- git diff

@@ -1,12 +10,8 @@
-- mitad izquierda es el archivo original
-- linea de inicio y final

-- la derecha significa desde que linea hasta que linea
aplico el cambio

## cambios en el area de stage
-- git diff --staged

## mostrar lineas que cambiaron sin ver contenido
-- git diff stat

-- git show (commit id)

## ver el archivo que se agrego con ese commit id

-- git show (commit id):rama

## Ramificacion
>Las ramas solo pueden crearse desde una rama existente.
al momento de crearse se posan en el ultimo commit iD de la rama principal, el HEAD le indica en que reama estamos actualmente

-- git branch (nombre de la rama)

-- git branch -r (ver ramas remotas de repos clonados)

-- git branch -d (nombre) para eliminar rama

-- git checkout o git switch para cambiar entre ramas

-- git branch --merged ramas funcinadas

-- git branch --no merged no fuincionadas

-- git branch --all

## Fusionar

--Git merge (ramas)

funcion de avance rapido

al momento de fusionarse se recimienda eliminar la rama 
cuando se crea una rama, esta rama es una copia del ultimo commit id, es decir tendra su contenido

## Al momento de la clonacion, git crea otra rama llamada origin main

origin/main(solo seguimiento remoto)

## Sincronizar

-- git fetch (alcanzar sin aplicar cambios)

-- git pull (alcanza y aplicar cambios)

## Mostrar commits

-- git log --oneline

-- git log --graph

-- git log --all

-- git log --all --stat (que archivos fueron impactados)

-- git log --graph --oneline --all


## Eliminar archivo del worksplace y del stagging

-- git rm (file)


## Trabjar en conjunto

-- fork (accion de github solamente) crear una copia personal de un repositorio sin afectar al principal(es util cuando no podemos crear ramas en el principal)


## Que es un pull request

>un pull request es una solicitud para extraer los cambios de una rama hacias otra, pueden ser del mismo repositorio o en distintos. de esta manera se permite verificar cambios antes de aplicarse en main.
