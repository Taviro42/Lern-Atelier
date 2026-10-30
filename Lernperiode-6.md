# Lern-Periode 6
<!--
**ANLEITUNG**

Dies ist die Vorlage für die Dokumentation einer Lernperiode. Hinweise an Sie
als Lernende:n stehen in solchen HTML-Kommentaren. Sie sind nur in der
Quellcode-Ansicht sichtbar.
Diese Blöcke können Sie entfernen oder zur Orientierung stehen lassen.

1.  Passen Sie die Nummer der Lernperiode an.
2.  Passen Sie den Namen an.
3.  Passen Sie den Zeitraum an. Achten Sie auf das Datumsformat tt.mm.jjjj
4.  Füllen Sie die Grobplanung aus in den Abschnitten Noten, Veränderungen,
    Projekte und Generelle Ziele. Behalten Sie alle Abschnitte bei.
5.  Erstellen Sie Platzhalter für die Tagesplanungen der Lernperiode.
6.  Planen Sie den ersten Arbeitstag.
7.  Löschen Sie allfällige Anweisungs-Blöcke, die Sie nicht mehr haben wollen.
8.  Speichern Sie die Datei und publizieren Sie sie (`git push`).
-->

- Name: Timon Studer
- Zeitraum: 23.10.2026 bis 18.12.2026

## Grob-Planung

### Noten
<!--
Wo stehen Sie mit Ihren Noten? In welchen Modulen waren Sie besonders stark;
in welchen sind die ungenügend? Welche davon sind besonders wichtig?
-->

Ich stehe gut mit meinen Noten. Die Note, die ich bereits zurückerhalten habe, war sehr gut. Bei den anderen LBs habe ich ebenfalls ein gutes Gefühl.

### Veränderungen
<!--
Was möchten Sie generell im Vergleich zur letzten Lernperiode anpassen?
-->

Ich möchte versuchen, generell weniger KI zu nutzen.

### Projekte / neue Technologien
<!--
Was für Projekte/neue Technologien möchten Sie gerne in dieser Lernperiode lernen?
Verlinken Sie zu den GitHub Repos Ihrer Projekte.
(Können Sie später nach und nach einfügen.)
-->

Repo: [Taviro42/maze-solver](https://github.com/Taviro42/maze-solver)

Das Projekt schreibe ich in C# als Console-App. Das Labyrinth speichere ich als 2D-Array, und den kürzesten Weg suche ich mit einer Breitensuche (BFS), die mit einer Queue arbeitet. Mein Ziel ist, dass ich am Ende einen funktionierenden Solver habe und verstehe, wie BFS funktioniert und warum sie den kürzesten Weg findet.

### Generelle Ziele
<!--
Was haben Sie für klare und messbare Ziele in dieser Lernperiode?
-->

- Das Programm liest ein Labyrinth aus einer Textdatei in ein 2D-Array ein und gibt es im Terminal aus
- Eine selbst geschriebene Breitensuche findet den kürzesten Weg vom Start zum Ziel
- Die Ausgabe zeigt das Labyrinth mit dem markierten kürzesten Weg und die Länge des Wegs
- Der Solver funktioniert mit mindestens 5 verschiedenen Test-Labyrinthen, darunter eines ohne Lösung, bei dem eine verständliche Meldung erscheint
- Ich kann im README in eigenen Worten erklären, wie BFS funktioniert und warum sie den kürzesten Weg findet
- Den gesamten Code schreibe ich selbst, ohne KI-generierten Code zu übernehmen

## Tagesplanungen
<!--
Planen Sie die Lernperiode. Dazu planen Sie Arbeitspakete (jeweils für den
kommenden Arbeitstag) und erstellen am Ende jedes Tages eine kurze Reflexion.

Wenn Sie an einem Tag gefehlt haben, schreiben Sie direkt unter die
Tagesüberschrift eines dieser Schlüsselwörter allein auf eine Zeile:
absence, absent, Absenz, abwesend, krank, Krankheit.
-->

### Planung 23.10.2026
<!--
Planen Sie 3 bis 5 **klar messbare** Arbeitspakete.
Umfang: ca. 30 - 60 Minuten je Arbeitspaket
Markieren Sie beendete Arbeitspakete mit einem x.

Beispiele:
- [ ] noch nicht erledigte Aufgabe
- [x] erledigte Aufgabe
-->

- [x] Das neue Projekt grob planen
- [x] Die Test-Labyrinthe erstellen
- [ ] Einlesen der Dateien, Speichern als 2D-Array und Ausgabe im Terminal


#### Tagesreflexion
<!--
Mögliche Themen: Was lief erstaunlich gut/schlecht? Wo ging der Plan nicht auf
und wieso? Was konnten Sie daraus für Ihr Vorgehen lernen?
Nicht wiederholen, was die Checkboxen schon aussagen.
Umfang: 50 - 100 Wörter (ungefähr 3 - 6 Sätze)
-->

Die Test-Labyrinthe sind erstellt. Ich habe mit der Funktion ReadMazeFile() begonnen, komme aber bei der Konvertierung zu einem 2D-Array nicht weiter. Der aktuelle Fehler ist: System.IndexOutOfRangeException.

### Planung 30.10.2026

- [x] Konvertierung zum 2D-Array fertigstellen
- [ ] Recherche, um die Frage "Ist BFS der Algorithmus, den ich für dieses Projekt nutzen möchte?" zu beantworten
- [ ] Recherche, um die Frage "Wie funktioniert der Algorithmus, den ich für dieses Projekt nutzen möchte, und wie implementiere ich ihn in .NET?" zu beantworten
- [ ] Die Ergebnisse der Recherche in eigenen Worten aufschreiben

- [x] Unit-Test für die ReadMazeFile()-Methode


#### Tagesreflexion

Die ReadMazeFile()-Methode funktioniert. Die Solution ist nun in ein App- und ein Test-Projekt aufgeteilt. Ausserdem habe ich die '.gitignore' geschrieben und einen Unit-Test für ReadMazeFile(maze1.txt) erstellt.

Der Unit-Test hat ziemlich lange gedauert: zum einen wegen des Setups der Solution, damit die beiden Projekte richtig referenziert sind, und zum anderen, um herauszufinden, wie ich die beiden Arrays in der Test-Methode richtig vergleiche (Assert.AreSequenceEqual()).

Mit der Recherche bin ich noch nicht fertig geworden. Ich setze sie nächstes Mal fort.

### Planung 06.11.2026

- [ ] Recherche, um die Frage "Ist BFS der Algorithmus, den ich für dieses Projekt nutzen möchte?" zu beantworten
- [ ] Recherche, um die Frage "Wie funktioniert der Algorithmus, den ich für dieses Projekt nutzen möchte, und wie implementiere ich ihn in .NET?" zu beantworten
- [ ] Vollständige Planung, wie ich den Algorithmus im Code implementiere
- [ ] Die Ergebnisse der Recherche in eigenen Worten aufschreiben

#### Tagesreflexion

...Ihr Text...


### Planung 20.11.2026

- [ ] ...Ihr Text...
- [ ] ...Ihr Text...
- [ ] ...Ihr Text...


#### Tagesreflexion

...Ihr Text...


### Planung 27.11.2026

- [ ] ...Ihr Text...
- [ ] ...Ihr Text...
- [ ] ...Ihr Text...


#### Tagesreflexion

...Ihr Text...


### Planung 04.12.2026

- [ ] ...Ihr Text...
- [ ] ...Ihr Text...
- [ ] ...Ihr Text...


#### Tagesreflexion

...Ihr Text...


### Planung 11.12.2026

- [ ] ...Ihr Text...
- [ ] ...Ihr Text...
- [ ] ...Ihr Text...


#### Tagesreflexion

...Ihr Text...


### Planung 18.12.2026

- [ ] ...Ihr Text...
- [ ] ...Ihr Text...
- [ ] ...Ihr Text...


#### Tagesreflexion

...Ihr Text...


<!--
Fügen Sie hier die weiteren Tage der Lernperiode ein.
-->

## Lernperiode Reflexion
<!--
Am Ende der Lernperiode schreiben Sie eine Reflexion über die gesamte Lernperiode.
Mögliche Themen: Wie gut passt Ihr Endresultat zu dem, was Sie sich vorgenommen
hatten? Unterm Strich, was ist Ihr grösstes Lernresultat? Was nehmen Sie für die
Zukunft mit aus dieser Lernperiode?
Umfang: 100 - 200 Wörter (ungefähr 6 - 12 Sätze)
-->

...Ihr Text...
