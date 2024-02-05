# Exercici GIT 2: Ús de l'historial de canvis

## 1
```bash
# Veure l'historial de commits
git log

# Crear un directori "capítols" i afegir contingut al fitxer "capitol1.txt"
mkdir capítols
echo "Afegeix els canvis a la zona d'intercanvi temporal (staging area)" > capítols/capitol1.txt

# Afegir canvis a la zona d'intercanvi temporal
git add capítols/capitol1.txt

# Realitzar un commit amb el missatge "Afegit capítol 1."
git commit -m "Afegit capítol 1."

# Veure l'historial de commits després de l'afegiment
git log
# Afegir contingut al fitxer "capitol2.txt" i afegir a la zona d'intercanvi temporal
echo "Afegeix els canvis a la zona d'intercanvi temporal." > capítols/capitol2.txt
git add capítols/capitol2.txt

# Realitzar un commit amb el missatge "Afegit capítol 2."
git commit -m "Afegit capítol 2."

# Veure les diferències amb la versió anterior
git diff HEAD HEAD~1

# Veure les diferències amb la versió abans de l'anterior
git diff HEAD HEAD~2
# Afegir contingut al fitxer "capitol3.txt" i afegir a la zona d'intercanvi temporal
echo "Afegeix els canvis a la zona d'intercanvi temporal." > capítols/capitol3.txt
git add capítols/capitol3.txt

# Realitzar un commit amb el missatge "Afegit capítol 3."
git commit -m "Afegit capítol 3."

# Veure les diferències amb la primera versió
git diff HEAD HEAD~2
# Afegir contingut al fitxer "index.txt" i afegir a la zona d'intercanvi temporal
echo "Afegir els canvis a la zona d'intercanvi temporal." >> index.txt
git add index.txt

# Realitzar un commit amb el missatge "Afegit capítol 5 a l'índex."
git commit -m "Afegit capítol 5 a l'índex."

# Veure qui va fer l'últim canvi a cada línia del fitxer "index.txt"
git blame index.txt

