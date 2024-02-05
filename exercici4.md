Exercici GIT 4: Gestió de branques 

# Paso 1
git branch bibliografia
git branch

# Paso 2 - Trabajando en la rama 'bibliografia'
git checkout bibliografia

# Realizar cambios en el archivo capitol4.txt
echo "Afegir els canvis a la zona d'intercanvi temporal." > capítols/capitol4.txt
echo "Fer un commit amb el missatge \"Afegit capítol 4.\"" >> capítols/capitol4.txt

# Agregar cambios al área de preparación
git add capítols/capitol4.txt

# Realizar un commit
git commit -m "Afegit capítol 4."

# Ver el historial de commits
git log --all --graph --oneline

# Paso 3 - Trabajando en la rama 'bibliografia' nuevamente
git checkout bibliografia

# Realizar cambios en el archivo bibliografia.txt
echo "Afegeix els canvis a la zona d'intercanvi temporal." > bibliografia.txt
echo "Fer un commit amb el missatge \"Afegida primera referència bibliogràfica.\"" >> bibliografia.txt

# Agregar cambios al área de preparación
git add bibliografia.txt

# Realizar un commit
git commit -m "Afegida primera referència bibliogràfica."

# Ver el historial de commits
git log --all --graph --oneline

# Paso 4 - Fusionar la rama 'bibliografia' con 'master'
git checkout master
git merge bibliografia

# Ver el historial de commits después de la fusión
git log --all --graph --oneline

# Eliminar la rama 'bibliografia' después de la fusión
git branch -d bibliografia

# Ver el historial de commits después de eliminar la rama
git log --all --graph --oneline

# Paso 5 - Crear y trabajar en la rama 'bibliografia' nuevamente
git branch bibliografia
git checkout bibliografia

# Realizar cambios en el archivo bibliografia.txt
echo "Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge \"Afegida nova referència bibliogràfica.\"" > bibliografia.txt

# Agregar cambios al área de preparación y realizar un commit
git add bibliografia.txt
git commit -m "Afegida nova referència bibliogràfica."

# Cambiar a la rama 'master'
git checkout master

# Realizar cambios en el archivo bibliografia.txt en 'master'
echo "Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge \"Afegida nova referència bibliogràfica.\"" > bibliografia.txt

# Agregar cambios al área de preparación y realizar un commit en 'master'
git add bibliografia.txt
git commit -m "Afegida nova referència bibliogràfica."

# Fusionar la rama 'bibliografia' con 'master' y resolver conflictos si es necesario
git merge bibliografia

# Agregar cambios al área de preparación y realizar un commit después de resolver conflictos
git add bibliografia.txt
git commit -m "Resolt conflicte de bibliografia."

# Ver el historial de commits
git log --all --graph --oneline
