# Clase 03

# git merge
Para fusionar las ramas tengo que usar **git merge**
IMPORTANTE: tengo que estar en la rama destino. Ejemplo, quiero fusionar la rama **footer** a  la rama **main** tengo que pararme en la rama **main** y ejecutar el comando **git merge footer**

```sh
git merge <rama-que-quiero-fusionar>
```

## abortar la fusion (cancela la integracion de ramas)
> Si quiero parar el merge, puedo hacer --abort
```sh
git merge --abort
```

## tipos de fusiones 

* Fast-fodward (No hay ningun conflicto se hace de manera automatica)
* Recursivo (ort-strategy) (No hay ningun conflicto se hace de manera automatica)
* Manual (Hay conflictos y hay que resolverlos de forma manual, indicandole a git que lo hicimos con un nuevo commit)

## Git stash
Permite registrar temporalmente los cambios que aun no fueron comiteados (guardados dentro del repo) (cambios que no estar en el working directory ni en el staging area) para guardarlos dentro de un area temporal y seguir trabajandolos luego.
los stash se guardan de manera local en la carpeta .git
tipo de estructura de datos de PILA (apilar y desapilar)

### crear un stash

```sh
git stash
```

### Sacar el elemento de la parte superior del stash
```sh
git stash pop
```

### Para eliminar un stash 

```sh
git stash drop # Borra el ultimo
git stash drop stash@{2} # Borra el stash con indice dos
```

### Aplico un stash en particular y no lo borro
```sh
git stash apply # desapila el primero de la pila
git stash apply stash@{5} # desapila el quinto de la pila    
```

> No borra el stash recuperado de la lista de stashes

### Puedo a partir de stash  crear una rama

```sh
git stash branch <nombre-de-la-rama>
```