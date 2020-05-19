# Anleitung zur Bearbeitung

Denke daran, dass das Mitarbeiter*innenhandbuch öffentlich ist.

## Vorschläge machen

1. Suche die Textstelle, die du bearbeiten willst. Am besten, du klickst dazu auf das Bearbeitungs-Icon oben rechts:
   ![](images/anleitung/1-edit.png)

2. Ändere die Textstelle. Wenn du fertig bist, kannst du deine Änderungen speichern ("committen"):
   ![](images/anleitung/2-commit.png)
   Es ist hilfreich für die Reviewer*innen, wenn du den Änderung einen sinnvollen Titel verpasst. Jedoch nicht zwingend notwendig.

3. Erstelle den Pull Request, um deine gespeicherten Änderungen vorzuschlagen:
   ![](images/anleitung/3-pull-request.png)
   Du hast in diesem Formular rechts die Möglichkeit, Reviewers für deinen Vorschlag auszuwählen. Dies ist eine gute Idee, wenn du gerne Feedback von bestimmten Menschen hättest, oder auch einfach verhindern willst, dass deine Änderung vergessen geht.


## Vorschläge akzeptieren

1. Öffne die [Liste der Vorschläge](https://github.com/feinheit/handbuch/pulls)

2. Wähle einen Vorschlag aus, und schau dir die Änderungen im Detail an. Wähle dazu die Files changed Ansicht:
   ![](images/anleitung/11-diff.png)

3. Falls du mit den Änderungen einverstanden bist, kannst du deine Review abgeben. Aktuell ist mindestens eine positive Review notwendig, damit ein Vorschlag akzeptiert werden kann.

4. Wenn genügend positive Reviews zusammengekommen sind, kannst du den "Merge pull request" Button klicken. Falls die gleiche Textstelle in der Zwischenzeit eine inkompatible Änderung erhalten hat, muss der Edit-Konflikt von Hand behoben werden.


## Auflösen von Edit-Konflikten

_Fehlt noch_


## Für Fortgeschrittene

Alternativ kannst du Änderungen am Mitarbeiter*innenhandbuch natürlich auch lokal vorbereiten. Dazu musst du das Projekt klonen und den Server starten:

    git clone https://github.com/feinheit/handbuch
    cd handbuch
    ./serve

Am besten, du erstellst einen eigenen Branch für die Änderung:

    git checkout -b mk/neuer-abschnitt

Anschliessend die Änderungen committen und pushen:

    git commit -m "Neuer Abschnitt" -a
    git push origin mk/neuer-abschnitt

Nun musst du nur noch auf Github [einen Pull Request erstellen](https://github.com/feinheit/handbuch/compare) und eine Reviewer*in finden 😃
