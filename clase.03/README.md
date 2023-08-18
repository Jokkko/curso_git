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
