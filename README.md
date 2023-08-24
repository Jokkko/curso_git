# Clase 04

# Trabajo colaborativo GIT

## A traves (Open Source) - Con Pull Request y Fork

1. Hacer un fork del proyecto. Del proyecto del cual quiero contribuir (Me voy copiar en mi cuenta el repo del proyecto original)
2. Me clono el fork desde mi cuenta github
3. Trabajo normalmente. Subo los cambios (A repo propio)
4. Me voy al proyecto original en el apartado Pull Request. Creo un nuevo Pull Request. Algunas veces aparece en mi repo la posibilidad Pull Request.

# Si el repo original sufrió más modificaciones. (Commits). Voy a tener que actualizar mi fork.

1. Voy a la cuenta del proyecto original y me copio la url del repositorio

2. Y agrego en mi repositorio local, la url (el remoto) del proyecto original.

```sh
git remote add upstream <url-del-repositorio-original>
```

```sh
git remote -v
```

3. Me traigo los cambios del repositorio original a mi repo local

```sh
git pull upstream main
```

4. Subo a mi repositorio remoto (Fork) las actualizaciones del repo local

```sh
git push
```

# GitHub CLI

<https://cli.github.com/>


# ¿Cuál es la diferencia entre fetch y pull?

## FETCH
Me trae la metada (O sea me actualiza la información dentro de la carpeta .git) pero no aplica los cambios automaticamente. Nos permite ver los cambios que ocurrien en el remoto y decidir luego que quiero hacer. Si los incomporo total o parcial.

## PULL
El hacer primero un fetch y luego trae los cambios automaticamente. Es la combinación de fetch y pull. Trae la metada y trae los cambios en las ramas correspientes.


# GIT CHERRY-PICK
Me permite traerme un commit o conjunto de commit de una rama en particular a otra rama

git cherry-pick <hash>
Me incluye los commit extremos seleccionados

git cherry-pick <hash>^..<hash>
No me incluye los extremos. Los bordes

git cherry-pick <hash>..<hash>

# GIT TAG

## Crear un tag en el último commit

```sh
git tag -a v3.0.0 -m "Versión 3.0.0" # tag anotado (a)
```

## Crear un tag en un commit en especifico

```sh
git tag -a v3.0.0 <HASH> -m "Versión 3.0.0" # tag anotado (a)
```

## Listar tags

```sh
git tag
```