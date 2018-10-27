git init inicializa la carpeta para que sea compatible con git(solo se hace una vez por proyecto

despues se enlaza la carpeta con el repositorio remoto
git remote add origin http://some.github.repository/SENIOR_DESIGN_PROJ.git

git add		->agrega todos los archivos nuevos o cambiados a un area pendiente
git commit -m "Initial commit"	->Commits staging area
git push -u origin master -> git push empuja el codigo al repositorio remoto

se pueden ver los archivos que fueron cambiados con
git status

y jalar cambios de otros usuarios o computadoras con 
git pull


para copiar un repositorio se usa 
git clone


para revertir cambios se hace un rollback
git checkout <archivo>   ->reinicia el archivo quitandolo en area de actuacion
git reset HEAD --hard    ->reinicia la base de datos al commit anterior
git checkout commit-number -> reinicia todo a un commit arbitrario
		Este es muy util si deja de funcionar por cambios realizados.





----git workflow----
fork/branch
commit
pull request
collaborate
merge


git tag->anotar version
git tag -a vx.x -m "version x.x"
git tag vx.x-lw ->pone vx.x-lw de etiqueta

para subir version con etiqueta
git push origin <tag>


git branch ramanueva
git checkout ramanueva

->desde master o rama que se quiere juntar
git merge ramanueva
git branch -d ramanueva ---->borrar rama nueva una vez que ya no es necesaria
