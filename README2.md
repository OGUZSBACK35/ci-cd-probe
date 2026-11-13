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


## Wichtige Kommandos Commits suchen switchen und Branches auch
1.  git Log // Zeigt alle Commits. du kannst auch schreiben git Log -5 --oneline  zeigt die letzten 5 Commits
2.  git Log -1 --oneline // zeigt dein aktueller commit
3. git switch --detach Hash // switch commit just find the hashtag of your commits with git Log than copy the one you want and write it where hash is
4.git switch -c nameofBranch // erstelle neuen Branch zum Commit wo ich mich jetzt befinde
5. git switch -c nameofbranch HASHofCommit // erstelle neuen Branch zu einem bestimmten Commit
6.  git push -u origin branchName // origin is remote Verbindung zwischen Github und Lokal. Man muss diesen Schritt machen um den Neuen erstellten Branch mit GitHub zu verbinden
7.  git branch -D branchname // delete local  branch
8.  git push origin --delete branch name // delete a branch on GitHub   
9. git branch // zeigt Alle Branches und wo man jetzt ist
10  git switch branchName // swich branches.


## Workshop Abläufe 12.11.2026
1.  Einrichtung auf HTML-Projekt
VSCode: Menü -> Datei -> Neue Datei -> Dateiname eingeben: Readme.md
VSCODE erkennt automatisch die .md Markdown-Datei

Arbeit mit Markdown, einer Dokumenten-Sprache
Zeichen: # steht für Überschrift mit der größten Schriftgöße in Fettschrift
## wie oben nur kleiner, sinnvoll nur bis ###
`text` Hervorheben von Text, grauer Kasten mit Schrift in Monospace
-- Runde Aufzählungszeichen
Speichern der Readme lokal
strg K S für den gesamten Projektordner
Strg S für die geöffnete Datei
Strg Shift S unter einem bestimmten Pfad, Dateinamen abspeichern
Wegschreiben der Readme an das zuvor angelegt Github-Repository

--git Status 
zeigt die Änderungen in ihre Projektordner an

--git add Readme.md
wenn sie sich im Projektordner befinden und nur die Readme erstellt habe (Info über git Status)
--git add .
wenn alle Dateien im Projektordner als Snapshot vorgemerkt (Staged) werden sollen

--git commit -m " Readme erstellt, Arbeitsabläufe in Git, GitHub und VSCode "
Lokaler Schnapsschss für das lokale Repository

--git push
Übertragung des lokalen Repositorys auf das Github-Repository
Vorraussetzung ist ein Komplett konfigurerter Projektordner btw. lokales Repository (Readme.md btw txt-Datei im Modulordner)
2.Klonen einer Remote-Ressource von GitHub über den Link zur GitHub Ressource
neuen Projektordner erstellen
VSCode -> Menü -> Datei -> Ordner öffnen (z. B Dokumente)
Menü in VSCode -> Terminal -> Neues Terminal

Prompt im Terminal steht sofort auf Dokumente

Eingabe im Terminal 
mkdir Ordnername
Neuen Ordner erstellen der später der Projektordner ist.

cd Ordnername
im Prompt zum Ordnername Wechseln

Neue Ressource von GitHub holen, Link wird Ihnen zu geschickt, oder ist im System abrufbar
git clone https://github.com/usern 

3. Einrichtung der Anwendung über den geklonten Quelltext und Ausführen der Anwendung
Hier Beschreibung
