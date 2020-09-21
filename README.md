---
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
##### Añadimos los cambios y hacemos un commit
 > + **git add .**
 > + **git commit -m "añadido el fichero .gitignore"**

#### Añadimos el fichero 1.txt
 > + **echo 1.txt**
 > + **git add .**
 > + **git commit -m "añadido 1.txt"**

#### Creamos y subimos al repositorio remoto el tag v0.1
 > + **git tag v0.1**
 > + **git push --tag origin master**

#### Creación de la tabla
```
| Nombres  |  Github |
|---|---|---|
|Alejandro Guerra| https://github.com/aguerra952 
|Rafael Dominguez | https://github.com/rafadominguez71  
|Juan Manuel Castillo  | https://github.com/JuanMaCasGod  

```


---
# COMANDOS UTILIZADOS EN LA PRÁCTICA AVANZADA

#### Creamos una rama y nos posicionamos en ella
