## GitHub

### Pasos para usar Github

git config --global user.email "you@example.com"<br>
git config --global user.name "Your Name"<br>
git config --list<br>

Github<br>
[Github Tutorial For Beginners - Github Basics for Mac or Windows & Source Control Basics][1]

Ej.
* git clone https://github.com/Enrique1965/GitHub.git
* git clone https://github.com/Enrique1965/testrepo.git

* git status
* git add README.md o * git add -A (add all) o git add --all
* git commit -m "agregue README.md comentario" o
* git commit -m "Hice cambios"
* git push
* [Basic Git commands][2]

**workflow**
* *git pull* (para actualizar nuestro repositorio local)
* hacer cambios los archivos que queramos
* *git add -A*
* *git commit -m "cambio generico o especifico hasta mensinar la linea"*
* se puede estar haciendo git commit todo el dia y despues hacemos sync
* si hacemos commit sin -m nos abre vim para editar comentario largo
* y lo podemos grabar con esc:wq
* *git push*

**Delete repository**
> Entrar al repositorio que queremos borrar
  ir a settings arriba a la derecha
  y hasta abajo hay un Danger Zone donde podemos borrar dando el
  nombre del repositorio.

**Rename repository**  
[How to rename a git repository?][5]
On the server side, just rename the repository with mv command as usual.
or goto thr repository Ej. *Enrique1965/GitHub* goto Settings and rename.
  * mv oldName.git newName.git
Then on the client side, change the value of the [remote "origin"] url into the new one. In the file /.git/config
  * url=example.com/newName.git
  * My case: url = https://github.com/Enrique1965/GitHub_Notes.git
Lastly rename de local client directory

**Edit Description, or Topic**    
  On the server side goto the top of the repository and Edit topic

**Make Global Edits and sync repository's**    
  * To sync and update all changes in all repositorys
  * On the client side change to the git root directory
  * ej. /git
  * do all the git *workflow*
    * git init
    * git status
    * git add -A
    * git commit -m "Changes ..."
    * git push all

no se pudo!
es mas complicado hacer un git multiple.

In the *.git/config* file you can add multiple urls to a defined remote:
[remote "all"]
    url=ssh://user@server/repos/g0.git
    url=ssh://user@server/repos/g1.git

Ej.
[remote "all"]
    url=https://github.com/Enrique1965/GitHub_Notes.git
    url=https://github.com/Enrique1965/Hola-Mundo.git
    url=https://github.com/Enrique1965/testrepo.git

**Git multi options**]
  * [git multiple repository management][6]
  * [git multi][7]

**solucion con script sh**<br>
nano gitpush.sh<br>

```Bash
  git add -A
  echo 'Enter the commit message:'
  read commitMessage
  git commit -m "$commitMessage"
  git push
  read
```


>  chmod +x gitpush.sh <br>
   ./gitpush.sh


**Use SSH**    
Para no tener que dar user y clave cada vez que hagamos push a git usar ssh key
  * [Eliminate Password on git push by Generating SSH keys for Github][4]
Para subir y tener hospedada un static website para nuestro blog en github
  * [GitHub Pages and Jekyll Beginner Video][3]


[1]: https://www.youtube.com/watch?v=0fKg7e37bQE
[2]: https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html
[3]: https://www.youtube.com/watch?v=nN6QuNqmAwk
[4]: https://www.youtube.com/watch?v=6oTzYnQY17Q
[5]: https://stackoverflow.com/questions/2041993/how-to-rename-a-git-repository
[6]: https://stackoverflow.com/questions/12700575/git-multiple-repository-management
[7]: https://github.com/grahamc/git-multi
---
