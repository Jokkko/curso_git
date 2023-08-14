# Clase 01

## Extensiones VSC

* GitLens
* Git Graph
* Material Icon Theme

## Verificar tener instalado git

```sh
git --version # git -v
```

## Configurar el nombre y el mail para poder realizar commits

```sh
git config --global user.name "User"
git config --global user.mail "Mail"
```

## Para saber si tengo todo configurado

```sh
git config --global --get-regexp user.keyg
```

## Para quitar alguna propiedad dentro del config

```sh
git config --global
```

## Para Inicializar un repositorio de git

```sh
git init
```

## Para saber el estado de los archivos

```sh
git status
```

## Estados de los archivos

* Untracked (Sin seguimiento) => archivos que no se agregaron al Index y por consecuente no se les da un seguimiento.
* Staged => Archivos agregados al Index y cuyos cambios van a ser incorporados al repositorio
* Unmodified => Archivos que se encuentran en el repositorio y no fueron modificados (con respecto al repo)
* Modified => Archivos que se encuentrar en el repositorio pero que difieren con el directorio de trabajo
