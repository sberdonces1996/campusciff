#COMANDOS UTILIZADOS EN LA PRACTICA BASICA
===

####Clonamos nuestro repositorio y nos movemos a él
git clone https://github.com/sberdonces1996/campusciff.git
cd campusciff

####Creamos el README.md, lo añadimos y hacemos un commit
git add .
git commit -m "commit inicial"

####subimos los cambios al repositorio
git push origin master

####Creamos el fichero privado.txt y luego la carpeta privada
echo > privado.txt
mkdir privada

####Hacemos que el gitignore ignore la carpeta y el archivo
echo "privado.txt" > .gitignore
echo "privada" > .gitignore


