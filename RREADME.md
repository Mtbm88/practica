repaso

```sh 
git status #ver el estado de la carpeta 

#agregar a la zona de staging area o idex (AREA DE CONFIRMACION)
git add nombre- archivo
git add . #todos los archivos 

## PERSISTIR LOS ARCHIVOS QUE COLOCO EN EL STAGING AREA - HACER COMMIT 
git commit  -m "mensaje"
git commit #abre un editor de texto 
 

 ## VER LOS COMMITS 
  git log #forma larga
  git log --online #forma corta
  git log -3 #ultimos 3 

### como veo la diferencia entre lo que tengo en el working directory y el local repo 

git diff

###diferencia entre dos ramas
 git diff nombre-rama
            git switch main 
            git diff dev

#como arreglo el mensaje del ultimo commit
**IMPORTANTE ademas de corregir el mensaje puedo agregar archivos que olvide dentro del commit** 
git add archivoquemeolvide 
git commit --amend 

## crear una rama 
git branch nombreRama
## cambiar rama
git switch nombreRama
## fusionar 2 ramas
git merge nombre-rama
** head en la rama desde la que queremos llamar a la rama que queremos fusionar **
## 
git switch main
git merge dev
```

## hacer un commit sin cambiar el mensaje pero agregando archivos o linea de codigo 

```sh 
gir add. 
git commit --amend --no- edit 
```

## Agregar modificaciones de archivos granularmente, Agregar partes del codigo agregado en un archivo

```sh
git add --patch
```


