# Lern-Periode 5

- Name: Timon Studer
- Zeitraum: 14.08.2026 bis 25.09.2026

## Grob-Planung

### Noten

> Die Noten sind stabil im Vergleich zur letzten Lernperiode. Zwei LPs sind noch nicht benotet. Ungenügende Noten gibt es noch keine. Mit dem Notenschnitt bin ich alles in allem zufrieden.

### Veränderungen

> In der vergangenen Lernperiode habe ich viel gelernt, jedoch entstand das Projekt für einen persönlichen Nutzen, was es für das Portfolio weniger nützlich macht. Dieses Mal möchte ich mir mehr Zeit für die Planung des Projekts nehmen und etwas wählen, was ich gut im Portfolio nutzen kann.

### Projekte / neue Technologien

Ich möchte mich im OOP üben, um allgemein schneller im Programmieren zu werden.

Dazu baue ich ein terminalbasiertes Roguelike-Spiel in **C#** (.NET Console-App, ohne Game-Framework), inspiriert von NetHack. C# habe ich gewählt, weil es OOP strukturell erzwingt und es einfach ist, die Tasten vom Spieler zu lesen.

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
- [x] Git-Repo erstellen
- [x] Working Directory aufsetzen

Heute habe ich die Planung für mein neues Projekt ausgearbeitet. Ich konnte mir eine ziemlich genaue Vorstellung bilden und das Gerüst ist aufgebaut. Danach hatte ich Probleme mit GitHub, was mich leider viel Zeit gekostet hat. Deshalb konnte ich noch nicht beginnen, Code zu schreiben.

## 21.08.2026

- [x] Die Entity-Klasse schreiben
- [x] Die erste statische Karte schreiben
- [x] Die Karte im Terminal anzeigen lassen

Heute habe ich die Entity-Klasse und die erste Karte hinzugefügt. Ich habe eine Funktion geschrieben, um den Player auf dieser Karte zu bewegen. Diese funktioniert noch nicht vollständig, was nächstes Mal das Hauptziel sein wird.

## 28.08.2026

- [ ] Die moveEntity-Funktion zum Laufen bringen
- [ ] Die Bewegung mit den Pfeiltasten zum Laufen bringen
- [ ] Ein Entity daran hindern, gegen eine Wand zu laufen

Heute bin ich etwas vom Weg abgekommen. Als ich meinen Code wieder anschaute, merkte ich, dass dieser überhaupt nicht gut lesbar war und den Konventionen nicht folgte. Dies begann ich dann zu lösen und zur gleichen Zeit die Funktionen, die ich letztes Mal nicht zum Laufen gebracht habe, zu debuggen. Damit bin ich noch nicht fertig. Ich werde nächstes Mal mit dem Refactoring fortfahren.

## 04.09.2026

- [x] Die Refactoring-Liste abarbeiten, die ich mit AI geschrieben habe, damit der Code wieder lesbar ist
- [x] Bugfix: Bei der Bewegung den Player an der alten Position erfolgreich löschen
- [ ] Feature: Ein Entity daran hindern, gegen ein Hindernis zu laufen

Heute habe ich alle Probleme auf der Refactoring-Liste abgearbeitet und der Code hat somit sehr viel an Qualität gewonnen. Es war viel einfacher, das Problem mit der Bewegungsfunktion zu lösen, weil der Code einfacher zu lesen war. Das neue Feature funktioniert noch nicht ganz, ist aber fast fertig implementiert.

## 11.09.2026

- [x] Bugfix: Bei einem Hindernis wird die target-Variable trotzdem verändert.
- [x] Bugfix: Die Logik, um herauszufinden, ob das target ein Hindernis ist, funktioniert noch nicht
- [ ] 1 neue Karte erstellen (in einer neuen Datei)
- [ ] Feature: Die Möglichkeit haben, eine zweite Karte zu laden.

Heute habe ich wieder viel Zeit mit Refactoring verbracht. Ich habe die Map-Klasse statisch gemacht. Die Logik, die ein Entity bewegt, ist nun in der Entity-Klasse und nicht mehr in Map. Die Render()-Funktion cleared nun die Console, bevor sie die Karte schreibt.

## 18.09.2026

- [x] 1 neue Karte erstellen (in einer neuen Datei)
- [ ] Feature: Die Möglichkeit haben, eine zweite Karte zu laden.
- [ ] Feature: Tür ('+') lädt den nächsten Raum

Die Karte ist erstellt, aber mit den beiden neuen Features bin ich noch nicht fertig geworden. Sie brauchen mehr Zeit als gedacht, weil ich sie richtig mit einer StateMachine implementieren möchte. Ausserdem habe ich noch etwas Zeit benötigt, um etwas aus einem Modul nachzuholen.

## 25.09.2026

- [x] Feature: Die Möglichkeit haben, eine zweite Karte zu laden.
- [x] Feature: Tür ('+') lädt den nächsten Raum
- [x] StateMachine fertig implementieren mit einer festen Reihenfolge für die Räume, in der der Spieler hin- und zurückgehen kann

Ich habe die Tür implementiert. Dazu habe ich eine statische Klasse für die Pfade zu den Dateien mit den Karten geschrieben. Die StateMachine ist simpler, als ich gedacht habe: ein Field in der Map-Klasse. Den Auslöser habe ich in die Move-Funktion der Entity-Klasse geschrieben.

## Lernperiode Reflexion

Ich bin alles in allem ziemlich zufrieden mit dieser Lernperiode. Das Spiel ist noch lange nicht "fertig", aber das war auch nicht wirklich das Ziel. Ich konnte sehr viele neue Erfahrungen sammeln. Für ein nächstes Mal nehme ich mir vor, von Anfang an mehr Zeit für die Planung zu nutzen. Ich hatte sehr viele Probleme, die ich damit einfach hätte vermeiden können. Zumindest möchte ich die grobe Klassenstruktur aufzeichnen, damit ich etwas habe, nach dem ich mich richten kann, ohne dass ich die Funktionen mehrmals zwischen den Klassen hin- und herschieben muss.
