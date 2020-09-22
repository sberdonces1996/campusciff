
# COMANDOS UTILIZADOS EN LA PRÁCTICA BÁSICA


#### Clonamos nuestro repositorio y nos movemos a él
 > + **git clone https://github.com/sberdonces1996/campusciff.git**
> + **cd campusciff**

#### Creamos el README.md, lo añadimos y hacemos un commit
 > + **git add .**
 > + **git commit -m "commit inicial"**

#### Subimos los cambios al repositorio
 > + **git push origin master**

#### Creamos el fichero privado.txt y luego la carpeta privada
 > + **echo > privado.txt**
 > + **mkdir privada**

#### Hacemos que el gitignore ignore la carpeta y el archivo
 > + **echo "privado.txt" > .gitignore**
 > + **echo "privada" > .gitignore**
 
#### Añadimos los cambios y hacemos un commit
 > + **git add .**
 > + **git commit -m "añadido el fichero .gitignore"**

#### Añadimos el fichero 1.txt
 > + **echo 1.txt**
 > + **git add .**
 > + **git commit -m "añadido 1.txt"**

#### Creamos y subimos al repositorio remoto el tag v0.1
 > + **git tag v0.1**
 > + **git push --tag origin master**

#### Uso social de Github
![Mi Github](https://github.com/sberdonces1996)

#### Creación de la tabla

| Nombres |  Github |
|---|---|---|
|Alejandro Guerra| [enlace a Github 1](https://github.com/aguerra952) 
|Rafael Dominguez | [enlace a  Github2](https://github.com/rafadominguez71)  
|Juan Manuel Castillo  | [enlace a Github 3](https://github.com/JuanMaCasGod) 




# COMANDOS UTILIZADOS EN LA PRÁCTICA AVANZADA

#### Creamos una rama y nos posicionamos en ella
 > + **git branch v0.2**
 > + **git checkout v0.2**

#### Añadimos el fichero a la rama anteriormente creada y hacemos commit
 > + **echo 2.txt**
 > + **git add .**
 > + **git commit -m "archivo 2.txt añadido"**

#### Subimos los cambios al repositorio remoto
 > + **git push origin v0.2**

#### Nos posicionamos en la rama maestra y hacemos un merge directo
 > + **git checkout master**
 > + **git merge v0.2 -m "merge v0.2 sin conflictos"**

#### Ahora hacemos merge en conflicto
##### escribimos hola en el fichero 1.txt y hacemos commit
 > + **echo "Hola" >> 1.txt**
 > + **git add .**
 > + **git commit -m "hola en 1.txt"**
##### Ahora nos posicionamos en la rama v0.2 y escribimos adios y hacemos un commit
 > + **git checkout v0.2**
 > + **echo "Adios" >> 1.txt**
 > + **git add .**
 > + **git commit -m "Adios en 1.txt"**

#### Posicionarse en la rama master y hacer un merge
 > + **git checkout master**
 > + **git merge v0.2**
##### Al hacer merge nos sale el error de conflicto con el siguiente mensaje
>CONFLICT (add/add): Merge conflict in 1.txt
Auto-merging 1.txt
Automatic merge failed; fix conflicts and then commit the result.
##### Borramos el adios y volvemos a hacer un merge
 > + **git merge v0.2**
 > + **git add .**
 > + **git commit -m "conflicto arreglado 1.txt"**

#### Hacemos un listado de las ramas con merge y sin merge
 > + **git branch --merged**
 > + **git branch --no-merged**

#### Borramos la rama v0.2
 > + **git tag v0.2**
 > + **git branch -d v0.2**

#### Listamos los commits y los tags
 > + **git tag**
 > + **git log**