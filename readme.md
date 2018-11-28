# Ejercicio 1

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
    git reset --hard HEAD~1, porque así deshacemos los cambios realizandos en el working copy, perdiendo los mismos.
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
    Para rehacer el último commit que acabamos de deshacer utilicé git reflog para ver donde existia por última vez ese commit
    después haremos git reset --hard c68af4d (identificador del commit) para recuperarlo
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
    Al hacer git merge master, no da conflicto porque la rama styled se creó a partir de master, por lo tanto al absorber a master no perdería ningun cambio y no daría conflicto.
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
    Al hacer el merge, como styled absorbe a htmlify si da conflictos. Esto se produce porque en styled y htmlify se han modificado las mismas líneas en el mismo archivo.
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
    En este caso no se produce conflicto, porque la rama master está absorbiendo nuevo contenido de la rama styled, por lo tanto no da conflicto.
- ¿Qué comando o comandos utilizaste en el paso 25?
    `git log --graph`
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
    Si, podría ser fast-forward, porque a partir de la rama master creamos la rama title, en la cual se modificó el archivo y posteriormente se hizo un commit. Es decir, se podría mergear sin perder ningun cambio.
- ¿Qué comando o comandos utilizaste en el paso 27?
    `git reset HEAD~1`
- ¿Qué comando o comandos utilizaste en el paso 28?
    `git checkout -- git-nuestro.md`
- ¿Qué comando o comandos utilizaste en el paso 29?
    `git branch -D title`
- ¿Qué comando o comandos utilizaste en el paso 30?
    `git reflog`
    `git reset --hard d34c51b`
- ¿Qué comando o comandos usaste en el paso 32?
    `git log` para ver cual es
    `git checkout` (hash del commit inicial)
- ¿Qué comando o comandos usaste en el punto 33?
    `git log`
    `git checkout` (hash del ultimo commit)