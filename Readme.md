Examen COD

Primero hacemos fork del repositorio y lo clonamos en local, lo abrimos en la interfaz y comprobamos que tenga las 3 ramas necesarias

Después creamos una nueva rama con git branch llamada readme y cambiamos a esa rama con git checkout readme, y creamos este archivo Readme.md y hacemos commit

Seguidamente tenemos que eliminar el ultimo commit de la rama interface, por lo que vamos a la rama interface y hacemos git reset interface para borrar el ultimo commit

Luego necesitamos hacer el git merge para juntar todo el codigo de las ramas interface y datos en la main (menos la rama readme), para ello hacemos git merge --squash y las clases interface y datos

