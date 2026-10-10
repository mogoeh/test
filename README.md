# Produktivitätsplan

Wochenplan Mo–Fr mit To-dos und Wochenzielen, Bedienung angelehnt an Outlook. Läuft komplett im Browser, ohne Konto und ohne Server, auch offline. Installierbar auf PC und Handy (Progressive Web App).

## Dateien
- `index.html` – die App
- `manifest.webmanifest`, `icon*.png`, `icon.svg` – für „Als App installieren“
- `sw.js` – Offline-Betrieb (bei Änderungen an der App `VERSION` hochzählen)

## Speicherung
Alle Daten liegen **nur im Browser des jeweiligen Geräts** (localStorage). PC und Handy haben getrennte Datenstände.
Sichern und Übertragen über **Einstellungen → Backup herunterladen / einspielen** (JSON-Datei). Oben rechts zeigt die App, wie alt das letzte Backup ist.

## Funktionen
- Wochenraster 05:00–20:00 Uhr, 30-Minuten-Takt, KW-Anzeige, Sprung zu Datum, Tasten ← / → / T
- Zeitraum markieren, Titel tippen, Enter; Doppelklick = Details
- Ganztags-Zeile (auch mehrtägig), „Anzeigen als“ (Gebucht, Mit Vorbehalt, Außer Haus, An anderem Ort tätig, Frei)
- Eigene Kategorien mit Farbe, Ort, Notiz, Serien (täglich Mo–Fr, wöchentlich, 14-tägig, monatlich)
- Verschieben per Drag & Drop, Dauer über die Unterkante, Duplizieren, Rückgängig
- Wochenbilanz in Stunden je Kategorie, Wochenziele je KW
- To-dos mit Priorität, Fälligkeit, Kategorie, Notiz, Filter; Einplanen per Ziehen oder Kalender-Symbol
- **Erinnerungen** 15 Min. vorher (einstellbar) und bei Beginn: Hinweis in der App, Ton und Systemmeldung – nur solange die App geöffnet ist
- **Export als .ics** je Termin (inkl. Serie und Erinnerungen) für Handy- oder Outlook-Kalender
