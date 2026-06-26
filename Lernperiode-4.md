# Lern-Periode 4

Name: Timon Studer

24.04.2026 bis 03.07.2026

## Grob-Planung

### Noten

Ich bin algemein sehr zufrieden mit meinen Noten bisher. 
Im Modul 162 war ich bisher am schlechesten, jedoch trotzdem noch genügend. Bei den beiden nachfolgenden Modulen bin ich auch gut nachgekommen.

### Veränderungen

Von der Lernperiode 3 gibt es leider keine Planungs-Datei. 
Ich habe einigermassen Effizient gearbeitet und sehr viel gelernt über Linux und Networking. Ausserdem habe ich zwei kleine Projekte programmiert: 1. Blackjack in c# 2. Word frequency counter in Python (Nicht fertig). Jedoch hatte ich Probleme konsistent zu bleiben und bin immer wieder von Projekt zu Projekt hin und her gewechselt. Dies habe ich vor in Lernperiode 4 zu verbessern. 

### Projekte / neue Technologien

Das Ziel dieser Lernperiode ist es, eine eigene statische Webseite von Grund auf selbst zu bauen.
Der Fokus liegt auf dem Verstehen der grundlegenden Web-Technologien HTML, CSS und JavaScript – nicht auf dem kreativen Design.

Als Referenz und Leitfaden dient die [Roadmap](Roadmap-Webseite.md), die 15 Phasen von der einfachen HTML-Seite bis hin zu dynamischen JS-Features (Markdown-Rendering, automatische Sidebar) umfasst. Diese ist generiert von einem KI Assistent.

### Generelle Ziele

- Eine funktionierende, mehrseitige statische Webseite selbst gebaut haben
- Die Grundkonzepte von HTML, CSS und JavaScript verstanden haben 
- Die Phasen 1–11 der [Roadmap](Roadmap-Webseite.md) (ungefähr) abgeschlossen haben 

## 24.04.2026

- Die Aufgabe 'ArduinoKennenlernen' erledigt
- Experimente mit dem Arduino
- Planung der neuen Lernperiode

## Planung 08.05.2026

- [x] Phase 1 – Projekt-Skeleton: `index.html` mit Grundstruktur (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`) erstellen (~30 min)
- [x] Phase 2 – Webserver einrichten: lokalen Server aufsetzen, Seite im Browser laden (~45 min)
- [x] Phase 3 – HTML-Inhalte: Überschriften, Absätze, Listen und Links einfügen (~45 min)
- [x] Phase 4 – Erstes CSS: `style.css` erstellen, einbinden, erste Elemente stylen (~75 min)
- [x] Phase 5 – Nav-Layout mit Flexbox *(Stretch-Ziel, falls Zeit bleibt)*

## 08.05.2026

Heute habe ich alle geplanten Phasen 1–5 abgeschlossen und sogar das Stretch-Ziel erreicht. Ich habe das Projekt `mysite/` mit `index.html` aufgesetzt, Apache als lokalen Webserver konfiguriert und die Seite im Browser geladen. Dann habe ich das erste Stylesheet hinzugefügt. In Phase 5 habe ich eine fixe Navigationsleiste mit Flexbox gebaut (dunkler Hintergrund, weisse Links, Drop Shadow). Gelernt habe ich auch den Unterschied zwischen Flex- und Block-Layout sowie die Wirkung von `position: fixed`.

## Planung 22.05.2026

- [x] Phase 6 abschliessen – Google Fonts via `@import` einbinden und auf Nav, Headings und Body anwenden (~45 min)
- [x] Phase 7 – Zweite Seite (`plan.html`) erstellen und aus der Nav verlinken (~60 min)
- [ ] Phase 8 – Erstes JavaScript: `main.js` einbinden, mit `document.querySelector` und einem Event-Listener experimentieren (~75 min)
- [ ] Phase 9 – Markdown-Datei mit `fetch()` laden und rohen Text anzeigen (~75 min)
- [ ] Phase 10 – Markdown mit `marked.js` rendern *(Stretch-Ziel, falls Zeit bleibt)*

- [x] Working directory optimieren

## 22.05.2026

Heute bin ich etwas vom plan abgekommen weil ich das Betriebssystem gewechselt und dadurch ein paar Dinge neu installieren musste. Ausserdem war ich sehr unzufrieden mit meinem Dateisystem und habe deshalb mir Zeit genommen ein sinnvolles Konzept auszuarbeiten. Mit der Webseite bin ich am Schluss doch noch voran gekommen. 

## Planung 29.05.2026

- [ ] Den Text und die Struktur von `index.html` finalisieren. (<-- noch nicht möglich)
- [x] Phase 8 – Erstes JavaScript: `main.js` einbinden, mit `document.querySelector` und einem Event-Listener experimentieren (~75 min)
- [x] Phase 9 – Markdown-Datei mit `fetch()` laden und rohen Text anzeigen (~75 min)
- [ ] Phase 10 – Markdown mit `marked.js` rendern *(Stretch-Ziel, falls Zeit bleibt)*

## 29.05.2026

Heute habe ich zum ersten Mal JavaScript benutzt. Ich habe die basis Syntax gelernt und mit async ein markdownfile als text auf der Webseite angezeigt. Ich habe zwar grundsätzlich nach Plan gearbeitet aber weniger erreicht als ich wollte.

## Planung 05.06.2026

- [x] Phase 10 – Markdown mit `marked.js` rendern: `marked.js` via CDN-`<script>`-Tag einbinden, geladenen Text in HTML umwandeln und einfügen (~60 min)
- [ ] Phase 11 – Linke Sidebar: DOM nach Überschriften durchsuchen, dynamisch eine klickbare Sidebar-Liste aufbauen (~75 min)
- [ ] Phase 12 – Sidebar-Design *(Stretch-Ziel, KI übernimmt Look-and-Feel)*

## 05.06.2026

Heute habe ich viel mit JavaScript gearbeitet. Ich habe sehr viel gelernt über async und wie ich HTML modifiziere mit JavaScript. Ich habe Phase 10 abgeschlossen aber die anderen Ziele nicht erreicht weil ich es richtig machen wollte. Es sind einige unerwartete Probleme aufgetretten weil meine Markdown im Obsidian Flavor geschrieben ist. Darum musste einige Dinge die Marked nich parsen konnte selbst implementieren. 

## Planung 12.06.2026

- [x] Phase 11 – Linke Sidebar: DOM nach `<h1>`–`<h3>` durchsuchen, für jede Überschrift ein `<a>`-Element mit `id`-Anker erzeugen und in eine Sidebar-Liste einfügen (~75 min)
  - Konzept: DOM-Traversierung (`querySelectorAll`), Elemente per JS erstellen (`createElement`, `appendChild`), Anker-Links (`id` + `#fragment`)
- [x] Phase 12 – Sidebar-Design: Breite, Einrückung, Hover-Farben, Highlight der aktiven Sektion *(Stretch-Ziel, KI übernimmt Look-and-Feel)* (~45 min)
- [ ] Phase 13 – Animierter Unterstrich in der Nav *(nur falls viel Zeit bleibt, KI-gestützt)* (~30 min)

## 12.06.2026

Heute habe ich den ganzen Nachmittag an der Sidebar gearbeitet. Der JavaScript Code war eine echte Herrausforderung und ich bin auch nach dem ich das Hauptproblem in Theorie gelöst hatte bei der Umsetzung noch auf viele andere Probleme gestossen. Ich konnte sehr vieles lernen bin jedoch immernoch etwas unsicher bei der Arbeit mit async.

## Planung 19.06.2026

- [x] Phase 13 – Animierter Unterstrich in der Nav: CSS-Keyframes/Transitions selbst schreiben, ein Element dessen Position sich je nach aktivem Nav-Link ändert (~90 min)
  - Konzept: CSS-Übergänge vs. Animationen, Positionierung relativ zum aktiven Link
- [ ] `index.html` finalisieren – Text und Struktur des Inhalts fertigstellen (~60 min)
- [ ] neue Seite für Tickets hinzufügen

- [x] CSS für mobile
- [x] Hamburger menu für sidebar auf mobile
- [x] CSS für sidebar fertig

## 19.06.2026

Heute habe ich die sidebar komplett fertig gestellt. Hiermit ist die seite Plan.html komplett und das auch für mobile. Das setup für den apache server ist auch schon fertig. Ich habe weiterhin viel mit JavaScript gearbeitet merke aber so langsam das das script ein wenig 'refactoring' benötigt. 

## Planung 26.06.2026

- [x] (optional) `index.html` finalisieren – Text und Struktur des Inhalts fertigstellen (~60 min)
- [x] Webseite auf den Apache server hochladen
- [x] neue Seite für Tickets hinzufügen

## 26.06.2026

Ich konnte das Projekt so gut wie abschliessen. Die grösste Herrausvorderung war die grösse der Iframes auf der Ticket-Seite. Die Webseite ist auf dem Server hochgeladen. Es fehlen noch letzte kleine Änderungen welche ich in meiner Freizeit erledigen werde. 

## Lernperiode Reflexion

Ich bewerte diese Lernperiode als sehr erfolgreich. Während dieser Lernperiode konnte ich am bis jetzt effizientesten arbeiten. Ich habe nicht immer ganz nach Plan gearbeitet und bin auch einige Male nicht mit allem fertig geworden, was ich erledigen wollte. Jedoch konnte ich das Projekt, das ich mir vorgenommen hatte, bis auf ein paar Details abschliessen weshalb ich es als einen Erfolg zähle. 
Für das nächste Mal möchte ich mir noch ein wenig mehr Zeit nehmen für die Planung des Projekts selbst damit ich es einfacher habe, die Planungen während der Lernperiode umzusetzen. 
