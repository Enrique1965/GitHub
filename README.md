## GitHub

Pasos para usar Github

git config --global user.email "you@example.com"<br>
git config --global user.name "Your Name"<br>
git config --list<br>

Github<br>
[Github Tutorial For Beginners - Github Basics for Mac or Windows & Source Control Basics][sa-1]

* git clone https://github.com/Enrique1965/GitHub.git
* git clone https://github.com/Enrique1965/testrepo.git

* git status
* git add README.md o * git add -A (add all) o git add --all
* git commit -m "agregue README.md comentario" o
* git commit -m "Hice cambios"
* git push
* [Basic Git commands][sa-2]

**workflow**
* *git pull* (para actualizar nuestro repositorio local)
* hacer cambios los archivos que queramos
* *git add -A*
* *git commit -m "cambio generico o especifico hasta mensinar la linea"*
* se puede estar haciendo git commit todo el dia y despues hacemos sync
* si hacemos commit sin -m nos abre vim para editar comentario largo
* y lo podemos grabar con esc:wq
* *git push*

**para borrar un repositorio**
> Entrar al repositorio que queremos borrar
  ir a settings arriba a la derecha
  y hasta abajo hay un Danger Zone donde podemos borrar dando el
  nombre del repositorio.

  Para no tener que dar user y clave cada vez que hagamos push a git usar ssh key
    * [Eliminate Password on git push by Generating SSH keys for Github][sa-4]
  Para subir y tener hospedada un static website para nuestro blog en github
    * [GitHub Pages and Jekyll Beginner Video][sa-3]

  [sa-1]: https://www.youtube.com/watch?v=0fKg7e37bQE
  [sa-2]: https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html
  [sa-3]: https://www.youtube.com/watch?v=nN6QuNqmAwk
  [sa-4]: https://www.youtube.com/watch?v=6oTzYnQY17Q
  ---
