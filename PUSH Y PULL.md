# PUSH Y PULL

En esta pestaña veremos la manera de modificar tu repositorio local y tu repositorio remoto localizado en GITHUB. 

## PUSH

Para hacer un push hay que seguir **los siguientes comandos**:

### GIT ADD

Este comando se utiliza cuando queremos guardar los cambios realizados dentro del repositorio de forma local.
Para agregar un único archivo utilizamos git add <ruta del archivo>, si queremos agregar todos los archivos que incluye el directorio sobre el que estoy parado,

**utilizamos:**

` git add .`

### GIT COMMIT
Una vez que los cambios se hicieron y se añadieron con git add localmente, el siguiente paso es hace un "commit". Un commit guarda el estado actual de la rama del proyecto sobre el que se está haciendo en un momento dado de manera local y nos permite regresar a su versión en el futuro si fuera necesario.

**Lo utilizamos llamando:**

`git commit -m "<mensaje explicativo sobre los cambios>"`

### GIT PUSH

Cuando hacemos $ git push, Git se encarga de subir al repositorio remoto los cambios que hayamos commiteado localmente, pero si existen cambios en el repositorio remoto que aun no tenemos, el comando será rechazado y nos pedirá que realicemos primero un git pull.
Si el push es aceptado, Git intentará de fusionar los cambios automáticamente.

**El comando utilizado es:**

`git push`

Si reconociera que hubo cambios de dos fuentes diferentes sobre un mismo archivo y línea, esto generaría lo que se conoce como [MERGE CONFLICT](MERGE CONFLICT.md) y nos pediría que revisemos manualmente la diferencia entre ambos opciones y aceptemos la modificación que corresponda. Luego de arreglar un conflicto, el resultado debe ser incluido con git add seguido de git commit.

## PULL

Este comando nos permite traer todos los cambios que existen en el repositorio remoto que todavía no tengo de forma local en la rama actual.
Lo ejecutamos simplemente corriendo $ git pull.