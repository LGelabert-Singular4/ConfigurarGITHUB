# PUSH Y PULL

En esta pestaña veremos la manera de modificar tu repositorio local y tu repositorio remoto localizado en GITHUB. 

## PUSH

Para hacer un push hay que seguir **los siguientes comandos**:

### GIT ADD

Este comando se utiliza cuando queremos guardar los cambios realizados dentro del repositorio de forma local.
Para agregar un único archivo utilizamos git add *ruta del archivo*, si queremos agregar todos los archivos que incluye el directorio sobre el que estoy parado.

**Utilizamos:**

` git add .`

### GIT COMMIT
Una vez que los cambios se hicieron y se añadieron con git add localmente, el siguiente paso es hace un "commit". Un commit guarda el estado actual de la rama del proyecto sobre el que se está haciendo en un momento dado de manera local y nos permite regresar a su versión en el futuro si fuera necesario.

**Lo utilizamos llamando:**

`git commit -m "mensaje explicativo sobre los cambios"`

### GIT PUSH

Cuando hacemos git push, Git se encarga de subir al repositorio remoto los cambios que hayamos commiteado localmente. Si existen cambios en el repositorio remoto que aun no tenemos, el comando será rechazado y nos pedirá que realicemos primero un git pull.
Si el push es aceptado, Git intentará de fusionar los cambios automáticamente.

**El comando utilizado es:**

`git push`

Si GIT reconoce que hubo cambios de dos fuentes diferentes sobre un mismo archivo y línea, esto generaría lo que se conoce como [MERGE CONFLICT](MERGECONFLICT.md) y nos pediría que revisemos manualmente la diferencia entre ambos y aceptemos la modificación que corresponda. Luego de arreglar un conflicto, el resultado debe ser incluido con git add seguido de git commit.

Es decir, como conclucion **la secuencia para hacer un push seria**:

```
git add .
git commit -m "Cambios Ejemplo"
git push
```

## PULL

Este comando nos permite **traer todos los cambios que existen en el repositorio remoto** que todavía no tengo de forma local en la rama actual. Se utiliza cuando **en un proyecto se trabaja de manera conjunta con otras personas**, es decir, que **lo recomendable es hacer un pull siempre antes de empezar a trabajar** para estar sincronizado con el repositorio remoto si alguien mas lo modifico.

### PULL

Para hacer un pull lo primero que hay que hacer es **subir nuestro proyecto a nuestro repositorio local** como hicimos anteriormente. Esto se hacia con los comandos:

```
git add .
git commit -m "Cambios Ejemplo"
```

Luego de esto lo que tenemos que hacer es **ejecutar el comando**:

`git pull`

**Y listo**, ya trajimos todo lo que estaba en el **repositorio remoto de GITHUB a tu repo local**.