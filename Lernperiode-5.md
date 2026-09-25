# Lern-Periode 5

- Name: Timon Studer
- Zeitraum: 14.08.2026 bis 25.09.2026

## Grob-Planung

### Noten

> Die Noten sind stabil im Vergleich zur letzten Lernperiode. Zwei LPs sind noch nicht benotent. Ungenügende Noten gibt es noch keine. Mit dem Notenschnitt bin ich alles in allem zufrieden.

### Veränderungen

> In der vergangenen Lernperiode habe ich viel gelernt, jedoch entstand es zu einem persönlichen Nutzen was es weniger nützlich für das Portfolio macht. Dieses Mal möchte ich mir mehr Zeit für die Planung des Projekts nehmen und etwas wählen was ich gut im Portfolio nutzen kann.

### Projekte / neue Technologien

Ich möchte mich üben im OOP um schneller allgemein im Programmieren zu werden.

Dazu baue ich ein terminalbasiertes Roguelike-Spiel in **C#** (.NET Console-App, ohne Game-Framework), inspiriert von NetHack. C# habe ich gewählt, weil es OOP strukturell erzwingt und es einfach ist die Tasten vom Spieler zu Lesen.

Ich starte bewusst klein: eine Karte, auf der sich der Spieler bewegen kann. Items, Gegner und weitere NPCs kommen schrittweise dazu, sobald der Kern funktioniert. Statt jedes Feature im Voraus zu planen, arbeite ich in Meilensteinen und entscheide unterwegs, was als Nächstes sinnvoll ist.

Architektur-Entscheidungen aus der Planung:

- **Rundenbasiert** – nichts bewegt sich, bis der Spieler einen Zug macht.
- **Karte aus Textdatei** laden. Prozedurale Generierung ist ein möglicher Ausbau, wenn der Rest läuft.
- **Alles ist eine `Entity`** – `Player` und Gegner erben von einer gemeinsamen abstrakten Basisklasse. 

### Generelle Ziele

- Ein spielbarer Prototyp: Karte wird aus einer Textdatei geladen und der Spieler kann sich mit den Pfeiltasten darauf bewegen, ohne durch Wände zu laufen
- Eine `Entity`-Basisklasse mit mindestens zwei Unterklassen (`Player` und ein Gegner)
- Mindestens ein Gegner, der eigene Züge macht, und ein einfaches Kampf-System
- Mindestens ein aufnehmbares Item mit einem simplen Inventar

## 14.08.2026

- [x] Projekt finden
- [x] Git repo erstellen
- [x] Working directory aufsetzen

Heute habe ich die Planung ausgearbeitet für mein neues Project. Ich konnte mir eine ziemlich genaue Vorstellung bilden und das Gerüst ist aufgebaut. Dannach hatte ich probleme mit github was mir leider viel Zeit gekostet hat. Deshalb konnte ich noch nicht beginnen Code zu schreiben.

## 21.08.2026

- [x] Die Entity Klasse schreiben
- [x] Die erste statische Karte schreiben
- [x] Die Karte im Terminal anzeigen lassen

Heute habe ich die Entity Klasse und die erste Karte hinzugefügt. Ich habe eine Funktion geschrieben um den Player auf dieser Karte zu bewegen. Diese funktioniert noch nicht vollständig was nächstes Mal das Hauptziel sein wird.

## 28.08.2026

- [ ] Die moveEntity Funktion zum laufen bringen
- [ ] Die Bewegung mit den Pfeil-Tasten zum laufen bringen
- [ ] Ein Entity daran hindern gegen eine Wand zu laufen

Heute bin ich etwas vom Weg abgekommen. Als ich meinen Code wider anschaute merkte ich das dieser überhaupt nicht gut lesbar war und den Conventionen nicht folgt. Dies begann ich dann zu lösen und zur gleichen Zeit die Funktionen die ich letztes Mal nicht zum laufen gebracht habe zu Debuggen. Mit dem bin ich noch nicht fertig. Ich werde nächstes mal mit dem Refactoring fortfahren.

## 04.09.2026

- [x] Die Refactoring Liste abarbeiten die ich mit AI geschrieben habe, damit der Code wider lesbar ist
- [x] Bugfix: Bei der Bewegung den Player an der alten Position erfolgreich löschen
- [ ] Feature: Ein Entity daran hindern gegen ein Hinderniss zu laufen

Heute habe ich die alle Probleme auf der Refactoring Liste abgearbeitet und der Code hat somit sehr viel an Qualität gewonnen. Es war viel einfacher das Problem mit der Bewegungsfuntion zu lösen weil der Code einfacher zu lesen war. Das neue Feature funktioniert noch nicht ganz ist aber fast fertig implementiert.

## 11.09.2026

- [x] Bugfix: Bei einem Hinderniss wird die target Variable trotzdem verändert.
- [x] Bugfix: Die Logic um herrauszufinden ob das target ein Hinderniss ist funtioniert noch nicht
- [ ] 1 Neue Karte erstellen (in einer neuer Datei)
- [ ] Feature: Die Möglichkeit zu haben eine zweite Karte zu laden.

Heute habe ich wieder viel Zeit mit Refactoring verbracht. Ich habe die Map Klasse statisch gemacht. Die Logik die ein Entity bewegt ist nun in der Entity Klasse und nicht mehr in Map. Die Render() Funktion cleared nun die Console befor sie die Karte schreibt. 

## 18.09.2026

- [x] 1 Neue Karte erstellen (in einer neuer Datei)
- [ ] Feature: Die Möglichkeit zu haben eine zweite Karte zu laden.
- [ ] Feature: Tür ('+') lädt den nächsten Raum

Die Karte ist erstellt aber mit den beiden neuen Features bin ich noch nicht fertig geworden. Sie brauchen mehr Zeit als gedacht weil ich es richtig mit einer StateMachine implementieren möchte. Ausserdem habe ich noch etwas Zeit benötigt um etwas aus einem Modul nachzuholen.

## 25.09.2026

- [x] Feature: Die Möglichkeit zu haben eine zweite Karte zu laden.
- [x] Feature: Tür ('+') lädt den nächsten Raum
- [x] StateMachine fertig implementieren mit einer festen reihenfolge für die Räume in der der Spieler hin und zurück gehen kann

Ich habe die Tür implementiert. Dazu habe ich eine statische Klasse mit für die Pfade zu den Dateien mit den Karten geschreiben. Die StateMachine ist simpler als ich gedacht habe ein Field in der Map Klasse. Den Auslöser habe ich in die Move funktion der Entity Klasse geschrieben.

## Lernperiode Reflexion

Ich bin alles in allem ziemlich zufrieden mit dieser Lernperiode. Das Spiel ist noch lange nicht "fertig" aber das war auch nicht wirklich das Ziel. Ich konnte sehr viele neue Erfahrungen sammeln. Für ein nächstes Mal nehme ich mir vor von Anfang an mehr Zeit für die Planung zu nutzen. Ich hatte sehr viele Probleme die sich damit einfach vermeiden hätte können. Zummindest möchte ich die gerobe Klassenstrucktur aufzeichen das ich etwas habe an dem ich mich richten kann ohne das ich die Funktionen mehrmals zwischen den Klassen hin und her schieben muss. 
