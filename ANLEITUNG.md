# Ernährungs-Symptom-Tagebuch – PWA

Eigenständige Progressive Web App für das Tracking der 4 Kategorien
(Uhrzeit/Ort · Speisen/Getränke · Beschwerden · Besonderheiten) mit Diktierfunktion.

## Dateien (alle in einen Ordner / ein Repo)

- `index.html` – die App
- `manifest.webmanifest` – App-Infos (Name, Icon, Farben)
- `sw.js` – Service Worker (Offline-Betrieb)
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` – App-Icons

> Wichtig: Eine PWA braucht **HTTPS**. Direkt vom Handy als Datei (`file://`) geöffnet
> funktioniert die Installation/Offline-Funktion **nicht**. Deshalb GitHub Pages.

## Veröffentlichen über GitHub Pages

1. Auf https://github.com einloggen (oder kostenlos registrieren).
2. **New repository** → Name z.B. `tagebuch` → **Public** → *Create repository*.
3. **Add file → Upload files** → alle obigen Dateien hochladen → **Commit changes**.
4. **Settings → Pages** → unter *Branch* `main` und Ordner `/ (root)` wählen → **Save**.
5. Nach ~1 Minute erscheint oben die Adresse, z.B.
   `https://DEINNAME.github.io/tagebuch/`

## Auf dem Samsung S23+ installieren

1. Die GitHub-Pages-Adresse in **Chrome** öffnen.
2. Es erscheint oben der Knopf **„Installieren"** (oder Chrome-Menü ⋮ → **App installieren**).
3. Die App liegt danach wie eine normale App im App-Drawer / auf dem Homescreen.
4. Beim ersten **Diktieren (🎤)** fragt Chrome nach **Mikrofon-Zugriff** → *Zulassen*.

## Daten & Sicherheit

- Einträge werden **lokal auf dem Handy** gespeichert (IndexedDB + „persistente Speicherung").
  Sie verlassen das Gerät nicht und funktionieren offline.
- **Backup:** Tagebuch → *Backup* erzeugt eine `.json`-Datei. Gelegentlich sichern
  (z.B. in Google Drive). Mit *Backup laden* wieder einspielen oder auf ein neues Gerät übertragen.
- **Nach 7 Tagen exportieren:** Tagebuch → *Letzte 7 Tage (PDF)* zum Ausdrucken/Weitergeben
  an die Ernährungsberaterin, oder *Letzte 7 Tage (CSV)* für Excel.

## Hinweise

- Diktieren nutzt die Spracherkennung von Chrome (Deutsch). Falls nicht verfügbar,
  funktioniert die **Diktiertaste der Tastatur** in jedem Textfeld.
- App aktualisieren: neue Dateien ins Repo hochladen; die App lädt die neue Version
  beim nächsten Start automatisch nach.
