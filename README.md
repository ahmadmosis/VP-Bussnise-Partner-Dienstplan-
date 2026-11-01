# BP Business Plan Dienstplan

Eigenständige Web-App (PWA). Keine Anmeldung, kein Server. Die Daten bleiben im Browser des Geräts.

## Auf GitHub Pages veröffentlichen
1. Auf github.com ein neues Repository anlegen (z. B. `dienstplan`).
2. Alle Dateien aus diesem Ordner hochladen (index.html, manifest.webmanifest, sw.js und die vier PNG-Dateien) über "Add file > Upload files".
3. Settings > Pages > Source: "Deploy from a branch", Branch `main`, Ordner `/ (root)`, Save.
4. Nach 1–2 Minuten ist die App unter https://BENUTZERNAME.github.io/dienstplan/ erreichbar.

## Als App installieren
- Android/Chrome: Link öffnen > Menü > "App installieren".
- iPhone/Safari: Teilen > "Zum Home-Bildschirm".
- Windows/Mac (Chrome/Edge): Installieren-Symbol in der Adressleiste.

## Daten
- Alles wird automatisch auf dem Gerät gespeichert.
- "Sicherung speichern" legt eine .json-Datei an, "Sicherung laden" spielt sie auf einem anderen Gerät ein.

## Optional: Excel-Export ganz ohne Internet
Die Bibliothek für den Excel-Export lädt beim ersten Export aus dem Internet und liegt danach im Cache. Wer sie lieber selbst hostet: `exceljs.min.js` (Version 4.4.0, aus dem npm-Paket `exceljs`, Ordner `dist`) in dasselbe Verzeichnis legen.

## Hinweis zum Datenschutz
Die Namen der Fahrer stehen als Startwerte im Code (index.html). Bei einem öffentlichen Repository kann jeder mit dem Link sie lesen.

## Neue Version veröffentlichen
Dateien im Repository ersetzen und in `sw.js` die Zahl bei `dienstplan-v6` erhöhen (z. B. `dienstplan-v7`).
