## Repaso
Git init -> inicia el repo
Git add -> lo pasa al  c
## Notes


# Clase 02 git- desarrollo colaborativo 
## .gitkeep
Git no lee las carpetas, para que existan en Git hay que generar un archivo .gitkeep este archivo me permite hacer un commit para guardarla, sirve para indicarle a git que la carpeta se tiene que guardar en el repositorio. 
Cuando tenga algun archivo se puede borrar, pero, generalmente no se hace. Es parte de la comunidad, no está dentro de la documentación de git. 

## .gitignore

Se crea siempre en la raiz del proyecto, pero se puede colocar en cualquier lado.  

Es un archivo que me permite ignorar archivos o carpetas completas que no quiero que se guarden en el repositorio 

Puedo escribirlos en el archivo, escribiendo por ejemplo *.log para que ignore todos los archivos .log

Si quiero ignorar una carpeta, por ejemplo node_modules/ 
.env entonces no va a poder enviarlo 

node_modules no se suben, y el . env tampoco. 

## 

