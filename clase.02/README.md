# Clase 02

# ADD : otras formas de colocar en el staging area archivos

```sh
git add -p git add --patch
```

* y: agregar el hunk: (tocito de codigo) al stage
* s: dividir el hunk en varios (automatico)
* n: descartar hunk
* e: editar manualmente el hunk (comentar la linea que no quiero pasar a stage)
* ?: ayuda

# CLONE : me permite clonar un repositorio completo, con los commits

```sh 
git clone <url-del-repo> git clone https://github.com/twbs/bootstrap.git . #punto le digo no crees una carpeta, hacelo en esta
```
