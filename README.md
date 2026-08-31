# MLT Lektionsplan

Interaktiver Editor für den Lektionsplan der Schweizer Armee
(Form 10.095 dfi / ALN 293-2389 / SAP 2526.0931) im **A5-Format**.

Eine einzige HTML-Datei – kein Server, keine Installation, keine Internetverbindung nötig.
`index.html` herunterladen und im Browser öffnen.

## Funktionen

- **Zweigeteilte Oberfläche** – links die Eingabefelder, rechts die Live-Vorschau in A5 (148 × 210 mm)
- **Seite 1** mit vollständigem Kopf (Wappen, Thema, Ausbildungsort, Zielsetzung, Teilnehmer,
  Material, Vorgehen-Block, Fusszeile); **Folgeseiten** nur mit der Tabelle Zeit / Ablauf /
  Methodische Hinweise – wie im Originalformular
- **Automatischer Seitenumbruch** – Abschnitte fliessen selbständig auf weitere Seiten
- **Verfasser** frei editierbar, oben rechts
- **Sprachen** der Feldbeschriftungen einzeln zuschaltbar (Deutsch / Français / Italiano)
- **Bilder** in der Ablauf-Spalte: Button, Drag & Drop oder Einfügen mit `Ctrl/Cmd + V`;
  Grösse pro Bild regelbar, Reihenfolge änderbar
- **Farbwähler** für den selbst geschriebenen Text – hebt Eingaben von den fixen
  Formularbeschriftungen ab
- **PDF-Export** direkt per Knopfdruck, echtes A5, ohne Druckdialog
- **Projektdatei `.lpx`** zum Speichern und späteren Weiterbearbeiten (inkl. eingebetteter Bilder)

## Bedienung

| Aktion | Weg |
|---|---|
| PDF erzeugen | Button **PDF** |
| Projekt speichern | Button **Speichern** oder `Ctrl/Cmd + S` → `.lpx` |
| Projekt öffnen | Button **Öffnen …** oder `.lpx` aufs Fenster ziehen |
| Bild einfügen | Button **Bild einfügen**, Drag & Drop oder `Ctrl/Cmd + V` im Ablauf-Feld |

## Hinweise

- Es wird **nichts im Browser gespeichert**. Zwischenstände als `.lpx` sichern – beim Schliessen
  warnt die Seite vor ungespeicherten Änderungen.
- Die Datei ist rund 590 KB gross, weil jsPDF und html2canvas eingebettet sind. Das ist der
  Preis dafür, dass der PDF-Export ohne Internetverbindung funktioniert.
- Warnt ein Abschnitt, dass er länger als eine Seite ist: aufteilen, Bild verkleinern oder
  die Schriftgrösse reduzieren.

`Beispiel_Lektionsplan_A5.pdf` zeigt eine mit dem Editor erzeugte Ausgabe.

## Verwendete Bibliotheken

- [jsPDF](https://github.com/parallax/jsPDF) 2.5.2 (MIT)
- [html2canvas](https://github.com/niklasvh/html2canvas) 1.4.1 (MIT)

Beide sind in `index.html` eingebettet.
