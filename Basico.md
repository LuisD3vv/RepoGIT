# Comandos basicos
git --version version de git

## Comandos para configuracion inicial del repositorio Para ingresar con nuestro usuario y email, se necesita cuenta en github o alguna palataforma simila con git

git config --global user.name
git config --global user.email

## inicializar el repositorio.

-- git init

## al usarlo se crea el stagging area

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
## ingresar repositrorio remoto
-- git remote add origin (origen)
-- git remote remove origin
## cambiar el nombre de la rama principal

git branch -m MAIN

## Este solo se ejecuta una ves, cuando cambiamos de remoto le damos el parametro -u origin main, despues solo sera git push

git push -u origin main

## Modificar y ver diferencias

-- git diff

-- git diff --staged