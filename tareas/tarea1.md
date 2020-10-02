# Tarea 1 Git

Clonamos el repositorio, usando el siguiente comando:

`git clone https://github.com/Cijo4/dpl_B_josejavier.git`

Haremos el primer commit para subir el documento Tarea1.md ya modificado

~~~
git add .
git commit -m "commit inicial"
~~~

Por ultimo subiremos el cambio al repositorio con push

`git push`

Creamos el archivo txt privado y la carpeta privada para 
posteriormente hacer que github los ignore.

~~~
touch privado.txt
mkdir privada
~~~

Añadimos dentro del documento .gitignore el nombre del txt y de 
la carpeta que queremos que ignore.

Ahora procedemos a creoar el archivo 1.txt y lo añadimos al 
repositorio local.

~~~
touch 1.txt
git add . 
git commit -m "commit 1.txt"
~~~
