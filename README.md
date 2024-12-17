# Github: comandos basicos

### Clonar el repositorio de github en tu ordenador

`git clone <URL_DEL_REPO_EN_GITHUB>`

Te lo crea si no tenias nada en tu local. La URL_DEL_REPO_EN_GITHUB esta en Github, en la pag del repo dandole al boton verde de Codigo


### Descargar los cambios nuevos que haya en Github (el remoto) a tu ordenador

`git pull`

(Esto es cuando ya tienes el repo en tu local)


------------------------


### Ver el estado de tu local

`git status`

En rojo salen los archivos con cambios sin añadir al indice y en verde los cambios que ya estan añadidos y listos para commitear (a esos los llama *staged for commit* = *añadidos al indice* = *marcados para commitear*)

(este comando no hace na, solo te da informacion)


------------------------


### Añadir cambios al indice

 El indice es el punto intermedio antes de commitear, esto los marca para que se guarden cuando hagas tu siguiente commit
 
`git add -A`

Ahi, -A sirve para decirle que marque todo lo que estuviera en rojo cuando haces `git status` . Si solo quieres marcar alguno en particular puedes hacer

`git add <PATH_DEL_ARCHIVO>` 

PATH_DEL_ARCHIVO es lo que sale en rojo para cada archivo con cambios al hacer `git status`


### Commitear cambios

Este es el comando que te guarda los cambios que tengas marcados para commitear y crea un checkpoint

`git commit -m '<MENSAJE_QUE_DESCRIBA_LOS_CAMBIOS>'`


### Subir todo lo que tengas commiteado a Github

`git push`
