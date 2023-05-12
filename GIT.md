# GIT

### ¿Que Es GIT?

Git es un **sistema de control de versionado** que, trabajando con otras personas sobre el mismo código, nos permite mantener un historial sobre los cambios realizados diciéndonos quién, cuándo y qué se realizó sobre un proyecto en común.

### ¿Que Es Un Repositorio?

Un repositorio podría considerarse un lugar virtual en el que se van a guardar todos los commits asociados a un proyecto. **Un commit** es un conjunto de cambios en tu proyecto y está asociado a un momento dado del mismo, **a una versión**. Git nos permite controlar los cambios y, de ser necesario, retornar a una versión anterior (o un commit anterior).

Con Git, trabajaremos con un repositorio local y un repositorio remoto. Pero, *¿qué significa esto?*

### Repo Local VS Remoto

Cuando hablamos de **repositorio remoto**, nos referimos al proyecto y sus versiones que se encuentran hospedados en internet como, por ejemplo, en GitHub, en cambio cuando hablamos de **repositorio a nivel local**, nos referimos al proyecto hospedado dentro de nuestra máquina.

Siempre que hagamos un cambio en nuestro proyecto, el mismo será local. Esto significa que, salvo que los subamos al repositorio remoto, nuestros compañeros no podrán verlo ni accederlo.
Por otro lado, cuando nuestros compañeros hagan sus propios cambios y los suban al repositorio remoto, nuestro proyecto no verá esos cambios localmente de forma automática. Es por eso, que tendremos que encargarnos de mantenerlo actualizado.

## INSTALACION DE GIT

Lo Primero que tenemos que hacer para **instalar GIT** es entrar a este link:

https://git-scm.com/download

Luego darle a **"Download For *sistema operativo que tengas*"** y luego a **"Click here to download"** y se les descargara la version ultima de git con formato .EXE, le damos click y la **instalamos de la manera que viene default**.

### CONFIGURACION DE GIT

Luego de haber instalado GIT toca configurarlo, para esto hay que **abrir la CMD y poner estos dos comandos**

```
git config --global user.name "TUNOMBRE"
git config --global user.email "TUEMAIL"
```

## CLONAR REPO

Para clonar el Repositorio vamos a el REPO que queremos clonar y **clickeamos donde dice "<> CODE"** y de ahi se desplegara un url que tendremos que copiar.

Luego de esto vamos a la CMD y ponemos git clone y pegamos el url:

EJEMPLO

`git clone https://github.com/GelabertLucas/RWCPrueba.git`

Ahi **nos saldra una pestaña de Git que nos dira que nos tenemos que loguear**. En esa pestaña vamos a token y pegamos ahi el [token](TOKEN.md) y le damos en aceptar.

Listo, Ya tenemos el repositorio clonado en la carpeta "C:/usuarios/TUUSUARIO/NOMBREREPO"