1,  Exercice 1 : Création et navigation entre branches

git adog
* 2e3aa7c (feature-1) Modification dans feature-1
* f349749 (HEAD -> main, feature-2) Premier commit : création du README

2, Exercice 2 : Fusion simple

git adog
* 811c01a (HEAD -> main, dev) création du notes.txt
| * 2e3aa7c (feature-1) Modification dans feature-1
|/  
* f349749 (feature-2) Premier commit : création du README
yushan9293@yushandeMacBook-Pro tp3 % git branch -d dev
Deleted branch dev (was 811c01a).

3, Exercice 3 : Gestion des conflits

git adog                                      
* b44122f (HEAD -> main) Fusion de main et conflit-test
* dd9c134 (feature-rebase) changement dans le branch main
| * 8703daa (confit-test) changement dans le branch confit-test
|/  
* 811c01a création du notes.txt
| * 2e3aa7c (feature-1) Modification dans feature-1
|/  
* f349749 (feature-2) Premier commit : création du README
yushan9293@yushandeMacBook-Pro tp3 % git branch -d feature-rebase
Deleted branch feature-rebase (was dd9c134).
yushan9293@yushandeMacBook-Pro tp3 % git adog
* b44122f (HEAD -> main) Fusion de main et conflit-test
* dd9c134 changement dans le branch main
| * 8703daa (confit-test) changement dans le branch confit-test
|/  
* 811c01a création du notes.txt
| * 2e3aa7c (feature-1) Modification dans feature-1
|/  
f349749 (feature-2) Premier commit : création du README

4, Exercice 4 : Rebase

 git adog
* a4530c8 (HEAD -> feature-rebase) rebase sur main dans la feature-rebase
* d7fab49 (main) modification dans la branch main
* b44122f Fusion de main et conflit-test
* dd9c134 changement dans le branch main
| * 8703daa (confit-test) changement dans le branch confit-test
|/  
* 811c01a création du notes.txt
| * 2e3aa7c (feature-1) Modification dans feature-1
|/  
f349749 (feature-2) Premier commit : création du README

5,Exercice 5 : Branches et historique
 git adog
*   2a426a5 (HEAD -> main) Merge branch 'feature-c'
|\  
| * f0e4e5b (feature-c) modification de b.txt
| * ed8a5b0 céation du c.txt
* |   d3fec7c Merge branch 'feature-b'
|\ \  
| * | f6d94e2 (feature-b) modification du b.txt
| * | 4129f5d création du b.txt
| |/  
* | cc56317 (feature-a) modificaiton de a.txt
* | d1edd63 création du a.txt
|/  
| * a4530c8 (feature-rebase) rebase sur main dans la feature-rebase
|/  
* d7fab49 modification dans la branch main
* b44122f Fusion de main et conflit-test
* dd9c134 changement dans le branch main
| * 8703daa (confit-test) changement dans le branch confit-test
|/  
* 811c01a création du notes.txt
| * 2e3aa7c (feature-1) Modification dans feature-1
|/  
f349749 (feature-2) Premier commit : création du README


git branch --merged
  feature-2
  feature-a
  feature-b
  feature-c
* main


git branch --no-merged
  confit-test
  feature-1
  feature-rebase


