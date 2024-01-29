EJERCICIO PREVIO
git clone https://github.com/asalber/libro-git.git
cd libro-git
git reset --hard 48ed8
git remote remove origin
EJERCICIO 1
notepad indice.txt
# Eliminar la última línea y guardar el fichero.
git status
git checkout -- indice.txt
git status
EJERCICIO 2
notepad indice.txt
# Eliminar la última línea y guardar el fichero.
git add .
git status
git reset indice.txt
git status
git checkout -- indice.txt
git status
EJERCICIO 3
notepad indice.txt
# Eliminar la última línea y guardar el fichero.
rm capitulos/capitulo3.txt
touch capitulos/capitulo4.txt
git add .
git status
git reset
git status
git checkout -- .
git status
git clean -f
git status
EJERCICIO 4
notepad indice.txt
# Eliminar la última línea y guardar el fichero.
rm capitulos/capitulo3.txt
git commit -a "Borrado accidental."
git status
git log
git reset --soft HEAD~1
git status
git commit -m "Borrado accidental."
git status
git log
git reset --hard HEAD~1
git log
git status
