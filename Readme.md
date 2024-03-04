Examen COD

Primero hacemos fork del repositorio y lo clonamos en local, lo abrimos en la interfaz y comprobamos que tenga las 3 ramas necesarias

Después creamos una nueva rama con git branch llamada readme y cambiamos a esa rama con git checkout readme, y creamos este archivo Readme.md y hacemos commit

Seguidamente tenemos que eliminar el ultimo commit de la rama interface, por lo que vamos a la rama interface y hacemos git reset interface para borrar el ultimo commit

Luego necesitamos hacer el git merge para juntar todo el codigo de las ramas interface y datos en la main (menos la rama readme), para ello hacemos git merge --squash interface datos

Al hacer esto, tendremos que hacer commit del merge con git add Main.java Interface.java BD.java

Ahora tendremos que hacer la release v1.0, para ello hacemos git tag -a v1.0 -m “Tag v1.0" 4ff1d (estos ultimos caracteres son los 5 primeros del codigo del commit del merge del que quiero hacer la etiqueta v1.0) y luego subirlos al repositorio tanto el codigo como las tags con git push origin v1.0 y git push origin main

Pero antes hay que completar y añadir el .gitignore

Y por ultimo hacemos push de la rama main con su tag y readme, y en GitHub hacemos la release mediante la interfaz
