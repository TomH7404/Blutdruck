# Blutdruck-Tagebuch (PWA)

Blutdruck und Puls mehrmals täglich erfassen, Verlauf ansehen, Bericht für einen Zeitraum als PDF oder CSV ausgeben. Alle Daten bleiben im Browser des Geräts (localStorage). Es gibt keinen Server, keine Schriftarten oder Skripte von Dritten.

## Auf GitHub Pages veröffentlichen

1. Neues Repository anlegen, zum Beispiel `blutdruck`.
2. Alle Dateien aus diesem Ordner ins Hauptverzeichnis des Repositorys hochladen (`index.html`, `manifest.webmanifest`, `sw.js`, die vier PNG-Icons).
3. Im Repository unter Settings → Pages: Branch `main`, Ordner `/ (root)` wählen und speichern.
4. Nach etwa einer Minute ist die App unter `https://<benutzername>.github.io/blutdruck/` erreichbar.

## Auf dem Handy installieren

- iPhone: Seite in Safari öffnen, Teilen → Zum Home-Bildschirm.
- Android: Seite in Chrome öffnen, Menü → App installieren.

Die Daten gehören zu genau dieser Adresse und diesem Gerät. Auf einem zweiten Gerät beginnt die App leer.

## Datensicherung

Unter „Bericht“ gibt es „Sicherung speichern“ und „Sicherung laden“. Die Sicherung ist eine JSON-Datei und lässt sich auch auf ein anderes Gerät übertragen. Wer die App nicht als Icon installiert, riskiert auf dem iPhone, dass Safari Daten nach längerer Nichtnutzung löscht. Als installierte App passiert das nicht.

## Update einspielen

Geänderte Dateien hochladen und in `sw.js` die Versionsnummer in `CACHE` erhöhen (`blutdruck-v3`), sonst liefert der Offline-Cache noch die alte Version aus.

## Einstufung

Die Farben und Begriffe folgen der ESC/ESH-Leitlinie (optimal unter 120/80, ab 140/90 erhöht). Sie dienen nur der Orientierung und ersetzen keine ärztliche Beurteilung.
