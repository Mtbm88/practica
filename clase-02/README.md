## Repaso
Git init -> inicia el repo
Git add -> lo pasa al  staging area
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

## Como ver el commit? 
Tenemos el  git show

```sh
git show <hash>

git show 22232c9s
```


Para salir del show en mac apretar solo q, no ctrl+q o cmd +q. Solo q. 

## Repaso comandos básicos 
### Marcar archivos que quiero que sean parte del próximo commit

Marcar archivos que estan en el working directory terminado y quiero llevarlos al area de confirmacion para que sean parte del próximo commit.
```sh
git add <nombre-archivo1> <nombre-archivo2>
git add README.md
```
## Git log

Info obtenida de la IA de google: 
git log: Muestra el historial completo de commits, incluyendo el identificador único (SHA), autor, fecha y mensaje de cada commit.
Opciones Comunes para Personalizar la Salida 
git log --oneline: Condensa cada commit en una sola línea, mostrando el SHA y el mensaje del commit, lo que es útil para una visión rápida.
git log --stat: Incluye información sobre qué archivos fueron modificados en cada commit y cuántas líneas fueron añadidas o eliminadas.
git log --patch o git log -p: Muestra el detalle de los cambios (los diffs) para cada archivo en un commit.
git log --graph: Agrega líneas para visualizar el historial de commits como un gráfico, mostrando la estructura de las ramas.
Filtros y Búsquedas
git log -n <N>: Limita el número de commits mostrados a los últimos N. 
git log --author="<patrón>": Filtra los commits por el nombre o correo electrónico del autor que contenga el patrón. 
git log --grep="<patrón>": Busca commits cuyo mensaje contenga el patrón especificado. 
git log <archivo>: Muestra solo los commits que han realizado cambios en el archivo especificado. 
git log <inicio>..<fin>: Lista los commits que están entre un punto de inicio y un punto de fin (pueden ser IDs de commit, nombres de rama, etc.). 
Navegación en la Salida
Cuando la salida de git log es muy extensa, se usa el paginador less. Para navegar: 
Presiona la barra espaciadora o Page Down para bajar una página.
Presiona la tecla b para subir una página.
Presiona j o la tecla de flecha hacia abajo (↓) para bajar una línea.
Presiona k o la tecla de flecha hacia arriba (↑) para subir una línea.
Presiona q para salir.

## Guardar los cambios en el repositorio

```sh
git commit -m "mensaje"
git commit # se abre el editor para escribir el mensaje
git commit -a # se hace un add de los archivos modificados, no se hace un add de los archivos untracked y se abre el editor para escribir el mensaje
git commit -am "mensaje" #Se agregan los archivos modificados y no se abre el editor para escribir el mensaje 

```

**Note** Los mensajes idealmente pueden tener como maximo 80 caracteres. 

*idealmente hay que dividir las tareas*