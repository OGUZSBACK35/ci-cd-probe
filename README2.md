# Wie Erstellt und verbindet man eine Repository mit Projekt aus dem Lokalen Gerät

1. Create Repo bei Github
2. installiere Git --> öffne Terminal und schreibe winget install --id Git.Git

3. Jetzt beim Projekt in Terminal folgendes angeben:

1.  git init // instatziere eine Lokale Repo
2.  git commit -m "Name"
3.  git status // nur zum Überprüfen
4.  git config user.name "Tom"
5.  git config user.email "Tom"
// jetzt wichtig beide Repos  (Local und GitHub) verbinden
6.  git remote add origin "Code des Repos"
7.  git branch -m main
8.  git push -u origin main

// Wichtige befehle  
**git switch -c "name of branch" //erstelle einen neuen branch und** wechsele zu ihm.  -c steht für Create 
git switch "name of branch " // wechsele nur zum branch ohne ihn zu erstellen
man kann auch mit git checkout feature-login arbeiten

## Schreibweise
1.  "#" macht überschrifte und jemehr "###" in folge du schreibst, desto kleiner ist der Text.
2.  "** Example **" fettDruck