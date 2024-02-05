Exercici GIT 4: Gestió de branques 

1
-git branch bibliografia

-git branch

2
-git checkout bibliografia

-Afegir els canvis a la zona d'intercanvi temporal.
Fer un commit amb el missatge "Afegit capítol 4."

-echo "Afegir els canvis a la zona d'intercanvi temporal." > capítols/capitol4.txt
echo "Fer un commit amb el missatge \"Afegit capítol 4.\"" >> capítols/capitol4.txt

-git add capítols/capitol4.txt

-git commit -m "Afegit capítol 4."

-git log --all --graph --oneline

3
-git checkout bibliografia

-Afegeix els canvis a la zona d'intercanvi temporal.
Fer un commit amb el missatge "Afegida primera referència bibliogràfica."

-echo "Afegeix els canvis a la zona d'intercanvi temporal." > bibliografia.txt
echo "Fer un commit amb el missatge \"Afegida primera referència bibliogràfica.\"" >> bibliografia.txt

-git add bibliografia.txt

-git commit -m "Afegida primera referència bibliogràfica."

-git log --all --graph --oneline

4
-git checkout master
git merge bibliografia

-git log --all --graph --oneline

-git branch -d bibliografia

-git log --all --graph --oneline

5
-git branch bibliografia

-git checkout bibliografia

-Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."

-echo "Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge \"Afegida nova referència bibliogràfica.\"" > bibliografia.txt

-git add bibliografia.txt
git commit -m "Afegida nova referència bibliogràfica."

-git checkout master

-Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."

-echo "Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge \"Afegida nova referència bibliogràfica.\"" > bibliografia.txt

-git add bibliografia.txt
git commit -m "Afegida nova referència bibliogràfica."

-git merge bibliografia
-Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."

-git add bibliografia.txt
git commit -m "Resolt conflicte de bibliografia."

-git log --all --graph --oneline
