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

(Heute habe ich... (50-100 Wörter))

## 04.09.2026

3 bis 5 klar messbare Arbeitspakete.

(Heute habe ich... (50-100 Wörter))

## 11.09.2026

3 bis 5 klar messbare Arbeitspakete.

(Heute habe ich... (50-100 Wörter))

## 18.09.2026

3 bis 5 klar messbare Arbeitspakete.

(Heute habe ich... (50-100 Wörter))

## 25.09.2026

3 bis 5 klar messbare Arbeitspakete.

(Heute habe ich... (50-100 Wörter))

## Lernperiode Reflexion

(In dieser Lernperiode habe ich... (100-150 Wörter))
