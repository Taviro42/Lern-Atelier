# Roadmap – Eigene Webseite bauen

Ursprünglich erarbeitet für ein Japan-Reise-Webseiten-Projekt (April 2026).
Diese Roadmap dient als Orientierung und muss nicht 1:1 übernommen werden.

---

## Phasen

### Phase 1 – Projekt-Skeleton und erste HTML-Seite `[Core Learning]`
`index.html` erstellen. Grundstruktur eines HTML-Dokuments verstehen: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`. Noch kein CSS oder JS.
**Konzept:** Was ein HTML-Dokument ist und wie der Browser es in eine Seite umwandelt.

### Phase 2 – Webserver einrichten `[Core Learning]`
Einen lokalen Webserver (z. B. Apache) so konfigurieren, dass er das Projektverzeichnis ausliefert. Neustart und Überprüfung.
**Konzept:** Wie ein Webserver eine URL auf eine Datei auf der Festplatte abbildet.

### Phase 3 – HTML-Inhaltsstruktur `[Core Learning]`
Überschriften (`<h1>`–`<h3>`), Absätze (`<p>`), Listen (`<ul>`, `<ol>`) und Links (`<a>`) hinzufügen.
**Konzept:** Semantisches HTML – Tags beschreiben *Bedeutung*, nicht Aussehen.

### Phase 4 – CSS: erstes Stylesheet `[Core Learning]`
`style.css` erstellen, aus `<head>` einbinden, einige Elemente selbst stylen.
**Konzept:** Selektoren, Eigenschaften, Werte und die Kaskade.

### Phase 5 – Seitenlayout mit Navigationsleiste `[Core Learning]`
`<header>` mit Nav-Links und `<main>`-Bereich hinzufügen. Flexbox einsetzen.
**Konzept:** Box-Modell, Block- vs. Inline-Elemente, Flexbox-Layout.

### Phase 6 – Visuelles Design: Farben, Schriften, Abstände `[Can Skip / AI handles]`
Genaue Hex-Farben, Schriftfamilien, Schatten, Abstands-Skalen. Die KI wählt die Werte – du verstehst nur, *wo* sie in der CSS stehen.

### Phase 7 – Zweite Seite und Verlinkung `[Core Learning]`
Eine zweite HTML-Seite erstellen und aus der Navigation verlinken.
**Konzept:** Relative vs. absolute Pfade, Struktur einer mehrseitigen Webseite.

### Phase 8 – Erstes JavaScript `[Core Learning]`
`<script>`-Tag und kleine `main.js` hinzufügen. Mit dem DOM interagieren.
**Konzept:** Das DOM, `document.querySelector`, Event-Listener.

### Phase 9 – Eine Markdown-Datei mit `fetch()` laden `[Core Learning]`
Eine `.md`-Datei erstellen, sie per `fetch()` laden und rohen Text anzeigen.
**Konzept:** Async/await, Promises, Browser-zu-Server-Kommunikation nach dem Seitenload.

### Phase 10 – Markdown mit `marked.js` rendern `[Core Learning]`
`marked.js` via CDN-`<script>`-Tag einbinden, den geladenen Text in HTML umwandeln und einfügen.
**Konzept:** Third-Party-Bibliotheken, `.textContent` vs. `.innerHTML`.

### Phase 11 – Linke Sidebar mit automatisch generierten Überschriften `[Core Learning]`
DOM nach Überschriften durchsuchen und dynamisch eine klickbare Sidebar-Liste aufbauen.
**Konzept:** DOM-Traversierung, Elemente per JS erstellen, Anker-Links (`id` + `#fragment`).

### Phase 12 – Sidebar-Design `[Can Skip / AI handles]`
Breite, Einrückung, Hover-Farben, Highlight der aktiven Sektion. KI übernimmt das Look-and-Feel.

### Phase 13 – Animierter Unterstrich in der Navigationsleiste `[Can Skip / AI handles]`
CSS-Keyframes und Übergänge. Das Konzept (ein Element, dessen Position sich je nach aktivem Nav-Link ändert) kurz verstehen; die CSS-Mathematik macht die KI.
**Konzept (leicht):** CSS-Übergänge vs. Animationen – nur genug, um den Code lesen zu können.

### Phase 14 – LAN-Zugriff `[Core Learning, schnell]`
Apache-Direktiven `Listen` und `Require` anpassen, damit andere Geräte im Heimnetz die Seite erreichen.
**Konzept:** Unterschied zwischen `localhost`, `0.0.0.0` und einer LAN-IP.

### Phase 15 – Finaler Feinschliff `[Can Skip / AI handles]`
Typografie, responsive Breakpoints, kosmetische Anpassungen. Alles von der KI erledigt.

---

## Wie die kreative Aufgabenteilung in der Praxis funktioniert

Bei jeder **[Can Skip / AI handles]**-Phase sieht man trotzdem, *wo* die Werte stehen und *warum* sie dort hingehören. Man kann jede Zeile des finalen Codes lesen und sagen: «Ja, ich verstehe, was das macht» – auch wenn man die genauen Zahlen nicht selbst gewählt hat.
