## Cuestionario

- ¿Qué comando utilizaste en el paso 11? ¿Por qué? 
    - He utilizado el comando git reset —hard HEAD ~ 1, porque quiere que 
me 
deshaga el ultimo cambio por eso le decimos HEAD ~ 1 baja 1 commit 
anterior 
y —hard para que este mismo efecto se haga en el working directory.
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
    - Entonces para rehacer el último commit el que acabamos de deshacer, 
necesitamos revisar todo el historial de navegación de HEAD para esto 
usamos el comando git reflog. Ahora buscamos el hash del commit y lo 
copiamos. Luego con git reset —hard {hash}, movemos el HEAD hacia ese 
commit, y su vez —hard rehace esos cambios en el working directory.
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 
    - No causó conflictos, cuando se ejecuta git merge main desde styled 
para que styled pueda absorber a main, por consola nos muestra que todo 
está al día en todos los commit. Already up to date.
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
    - Sí, causó conflictos porque en ambas ramas tenemos diferencias sobre 
el mismo contenido y debemos decidir qué cambios quedarnos o descartar.
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
    - No causó conflictos porque en main no habían elementos adicionales, 
contaba solo con los cambios base o los iniciales. 
- ¿Qué comando o comandos utilizaste en el paso 25? 
    - El comando para tener una salida de consola gráfica para el 
historial de commit es git log —graph
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
    - No, el merge anterior es no fast forward, porque se ha creado un 
commit indicando que se ha hecho un merge entre las dos ramas.
- ¿Qué comando o comandos utilizaste en el paso 27? 
    - En este paso usé el comando git reflog para obtener el hash de un 
cambio que halla navegado HEAD antes del merge de title en main, luego 
hice un git reset {hash} para indicar al puntero HEAD ir hasta ese cambio, 
pero sin el —hard porque no queremos que nos afecte el working directory 
sino únicamente en el repositorio virtual.
- ¿Qué comando o comandos utilizaste en el paso 28? 
    - Los comando fueron git status para revisar el estado del archivo, 
luego usé un git diff para corroborar si hay cambios vigentes cuales son y 
observe que los cambios efectivamente era reemplazar el titulo por el que 
yo había escrito. Ahora ejecute el comando git restore git-nuestro.md para 
descartarlos. De esta manera estamos en el punto antes del merge.
- ¿Qué comando o comandos utilizaste en el paso 29? 
    - Me aseguro de no estar en la rama title, y luego ejecuto el comando 
git branch -D title para eliminar la rama title.
- ¿Qué comando o comandos utilizaste en el paso 30?
    - Para el paso 30 uso git reflog para copiar el hash del cambio o 
rastro en donde se hizo el merge, luego hago un git reset —hard {hash} 
para que me devuelva hasta el punto del merge y poder rehacer todo hasta 
este punto.
- ¿Qué comando o comandos usaste en el paso 32? 
    - Usé el comando git reset —hard {hash} para ir hasta el momento 
inicial cuando se creaba el poema.
-  ¿Qué comando o comandos usaste en el punto 33?
    - De la misma forma ejecuté un git reset —hard {hash} para ir hasta el 
momento en donde le coloqué un titulo al poema.

