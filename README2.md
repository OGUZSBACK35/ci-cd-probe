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

# Inhaltverzeichnis
-[1.  Einrichten Readme auf HTML-Projekt](#Wdh git-Workflow)
-[2.  klone

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
Machen Sie den Quellcode für sich verfügbar undsichern Sie diesen Quelltext in einem eingenen GitHub-Repository in Ihrem Projektordner steht die Ressource noch auf der Quelle btw. dem GitHub-Repo von dem Sie geklont haben.

1.  Neues GitHub Repository erstellen
    unter ihrem GitHub-Account: Home-Ansicht: Navigationsleiste und Pluszeichen "+" Neues Repository (New Repository)
    oder Menü -> All repositories -> grüner Button "New repository
     Einstellung Private und Public berücksichtigen.

    Zum neuen Repository gehen: Anklicken und https Ressource kopieren
    Bei frischem Repo ohne Quelltext sehen Sie direkt den Link, sofort kopieren: siehe Dokument-Symbol
    Wenn schon Code drin steht gehen Sie über den grünen Code Button "<> Code"
    -
2.  Die eigene neue GitHub-Ressource in den Projektordner schreiben
    VSSCode im Terminal, Prompt zeigt auf den Projektordner
    -'git remote set-URL origin https://github.com/ihrGithubAccountName/NeuesRepoName.git
    Verbindung prüfen, hier sollte ihre GitHub-Repository Ressource zu sehen sein.

    -- git remote -c
    Dann der Dreiklang git add, git Commit, git push
    da sie Wahrscheinlich noch keine Änderungen vorgenommen haben ist git add nicht notwendig
    -'git commit -m "Original Code der Angular-Anwendung"
    da sie zum ersten Mal hier pushen, den push-Befehl komplett angeben
    - git push -u origin main
      origin bezieht sich immer auf die Github-Ressource, die im Projektordner angelegt wurde.
      dann sollten sie den Quellcode in der Cloud (ihrem Repository auf Github)
      übertragen haben.

3. Installation für um die Anwendung zum Laufen zu bringen (hier die Angular- Amwendung)
VSCODE Terminal:
Installation von Node.js LTS als middleware mit den benötigten Laufzeitumgebungen (Engine) und Bibliotheken
-'Winget install Open.NodeJS.LTS
Kontrollieren der Installation, Version von Node.js prüfen       
- `node -v`
Version des NodeJS Paketmanagers
-`npm -v`
Hier sollten Ihnen die aktuellen Versionnummern angezeigt werden
Bei Problemen: Oftmals verweigert Windows Ihnen Skripte im Betriebssystem zu schreiben
Mit dem folgenden Befehl holen Sie sich die Berechtigung:
jetzt sollte auch die Prüfung der Versionen funktionieren.

4.  Die Laufzeitumgebung, Build-Tools und Bibliotheken erstellen VSCode Terminal in ihrem Projektordner
-´npm install´
Es werden einige Warmeldungen erzeugt, die harmlos sind. Sie sollten keine Error-Meldung haben

5.   Die Anwendung starten mit dem Build, Zusammenbau aller Funktionalitäten
-`npm start`

Angular Anwendungen laufen standardmäßig auf dem Port 4200
Wenn Sie jetzt localhost: 4200 in Ihrem Browser eingeben, sehen Sie die Anwendung 

airgendwas  
fehler sdsd

wawawaw

WARUM?! WARUM? WARUUUUM?!!?!
