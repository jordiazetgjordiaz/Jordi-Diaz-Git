Exercici GIT 2: Ús de l'historial de canvis
1 
-git log
-mkdir capítols
echo "Afegeix els canvis a la zona d'intercanvi temporal (staging area)" > capítols/capitol1.txt
-git add capítols/capitol1.txt
-git commit -m "Afegit capítol 1."
-git log



2
-echo "Afegeix els canvis a la zona d'intercanvi temporal." > capítols/capitol2.txt
-git add capítols/capitol2.txt
-git commit -m "Afegit capítol 2."
-git diff HEAD HEAD~1  # Per veure les diferències amb la versió anterior
git diff HEAD HEAD~2  # Per veure les diferències amb la versió abans de l'anterior


3
-echo "Afegeix els canvis a la zona d'intercanvi temporal." > capítols/capitol3.txt
-git add capítols/capitol3.txt 
-git commit -m "Afegit capítol 3."
-git diff HEAD HEAD~2  # Per veure les diferències amb la primera versió


4
-echo "Afegir els canvis a la zona d'intercanvi temporal." >> index.txt
-git add index.txt
-git commit -m "Afegit capítol 5 a l'índex."
-git blame index.txt
