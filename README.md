# Git_webXVI

Tarea de GitHub

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
    git reset --hard HEAD~1.
    reset --hard deshace el commit y tambien elimina los cambios.
    HEAD~1 hace referencia al commit que deseo restablecer, que es al anterior del que estoy. tambien podrìa hacer git reflog y buscar el commit al que me quiero restablecer.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
    1. git reflog buscamos el commit al que queremos restablecer que es el d845783.
    2. git reset --hard d845783. Para poder rehacer el commit y los cambios que se hiciero, no veo sentido hacer git reset d845783 y dejar cambios fuera del stage.


- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
    1. revisamos que estamos en styled. git branch
    2. git merge main. styled absorbe main.
    3. No , porque styled tiene el commit de main, main no puede crear ningun conflicto.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
    1. git branch.
    2. git checkout styled
    3. git merge htmlify.
        a. si
        b. Aunque ambos tiene el commit de main htmlify tiene unos cambios(commit)que styled no tiene


- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
    1. git branch
    2. git checkout main
    3. git merge styled. Se hace un commit fast-forward 
    4. No, git solo mueve el puntero hacia el ultimo commit de styled, no hemos hecho nada en main.

- ¿Qué comando o comandos utilizaste en el paso 25?
     git log --graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
    1. git checkout main
    2. git merge --no-f title
    3.Si, creo que por que es igual que el primer merge, title esta mas arriba con un commit mas que main. 
    no se crea conflicto.

- ¿Qué comando o comandos utilizaste en el paso 27?
        1.git reste HEAD~1. HEAD~1= al hash 39a6beb. 

- ¿Qué comando o comandos utilizaste en el paso 28?
    1.git status
    2. git restore git-nuestro.md.   Pierdo el titulo

- ¿Qué comando o comandos utilizaste en el paso 29?
    1. git branch
    2. git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
    1. git reflog, busco el merge 43e5946
    2. git reset --hard 43e5946. Recupero mi titulo

- ¿Qué comando o comandos usaste en el paso 32?
    Despues de haber hecho git banch -d y eliminar  las ramas en el paso 32 hago:
    1. git reflog y busco el hash a501ac6 
    2. hago git checkout a501ac6.

- ¿Qué comando o comandos usaste en el punto 33?
    1. git reflog y busco el hash 43e5946
    2. git checkout 43e5946
    3. Head esta detached. para resolver hago un checkout a main.

    
