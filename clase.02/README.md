# Clase 02

# ADD : otras formas de colocar en el staging area archivos

```sh
git add -p git add --patch
```

* y: agregar el hunk: (tocito de codigo) al stage.
* s: dividir el hunk en varios (automatico).
* n: descartar hunk.
* e: editar manualmente el hunk (comentar la linea que no quiero pasar a stage).
* ?: ayuda.

# CLONE : me permite clonar un repositorio completo, con los commits

```sh 
git clone <url-del-repo> 
git clone https://github.com/twbs/bootstrap.git . #punto le digo no crees una carpeta, hacelo en esta
```

# .gitignore: Me permite descargar archivos que no quiero que formen parte del repo
Para eso tengo que crear un archivo llamado .gitignore y colocarle el nombre del directorio a ignorar.

# Amend: me permite enmendar un commit
Arreglar el mensaje del commit o agregar archivos o partes de un archivo que me quedaon fuera del commit.
```sh 
git amend -m "mensaje"
```

## gitkeep: me permite subir carpetas vacias
Git no versiona carpetas, si quisiera subir una carpeta tengo que crearle dentro un archivo llamado. **.gitkeep**

## REMOTE: me permite agregar la url del repo remoto en el local para subir los cambios

```sh 
git remote add <url-del-repo>
```

> Visualizar donde esta el remoto de mi repo

```sh 
git remote -v
```

# crear una branch

```sh
git branch <nombre-branch>
```
## listar ramas

```sh 
git branch
```

## moverme a una rama

```sh 
git switch <nombre-branch>
```

## borrar una rama que ya no se va a utilizar

```sh 
git branch -d <nombre-de-la-branch>
git branch -D <nombre-de-la-branch> # Mandale, borrala estoy seguro
```
