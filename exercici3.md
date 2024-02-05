Exercici GIT 3: 

1
-sed -i '$d' index.txt
-git status
-git checkout -- index.txt
-git status

2
-sed -i '$d' index.txt
-git add index.txt
-git status
-git restore --staged index.txt
-git status
-git checkout -- index.txt
-git status


3
-sed -i '$d' index.txt
-rm capítols/capitol3.txt
-touch capítols/capitol4.txt
-git add index.txt capítols/capitol4.txt
-git status
-git restore --staged index.txt capítols/capitol4.txt
-git status

4
-sed -i '$d' index.txt
-rm capítols/capitol3.txt
-git add index.txt capítols/capitol3.txt
-git commit -m "Borrat accidental."
-git add index.txt capítols/capitol3.txt
-git commit -m "Borrat accidental."
-git log
-git reset HEAD~1
-git log
-git status
-git add index.txt capítols/capitol3.txt
-git commit -m "Borrat accidental."
-git reset --hard HEAD~1
-git log
-git status
