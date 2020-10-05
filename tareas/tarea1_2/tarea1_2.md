
# Tarea 1.2 Trabajando con Git

## José Sánchez 2 DAW

## Crear una rama

Para crear una rama usaremos el comando git branch mas el nombre de la rama.
Posteriormente listaremos las ramas disponibles con git branch.

~~~~

git branch v0.1
git branch

~~~~

![nueva rama](rama1.png)

## Añadir fichero 2.txt

Para crear el fichero 2.txt usaremos el comando touch

~~~~
touch 2.txt
~~~~

![2.txt](2txt.png)

## Crear una rama remota

Para crear la rama remota y subirla al repositorio remoto usamos git push [nombre del repositorio]
y luego [el nombre de la rama]

`git push origin v0.2`

![push rama remota](subirRama.png)

## Merge directo

Para hacer el merge primero nos pasamos a la rama master con git checkout y luego usamos
git merge v0.2.

~~~~
git checkout master
git merge v0.2
~~~~

![merge](merge.png)

## Merge con conflicto

Añadimos hola en el txt de la rama master y hacemos commit, luego hacemo lo mismo en el 
txt de la rama v0.2 pero poniendo adios en el txt y hacemos el commit.
Veremos que al intentar hacer el merge nos dara un fallo ya que estan en conflicto dado
que los dos documentos estan modificados en las dos ramas.

![conflicto](mergeHyA1.png)

Despues de este error si accedemos al txt con nano veremos el documento de la siguiente forma

![conflicto2](mergeHyA.png)

Para solucionarlo debemos borrar el contenido que queremos descartar y luego hacer el 
commit correspondiente.

![conflicto3](arregloConflicto.png)
