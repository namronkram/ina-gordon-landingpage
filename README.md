# Landingpage-Template — Ina Gordon

Eine fertige, **einfach zu bearbeitende** Ein-Seiten-Website für Online-Coaching / Therapie.
Alle Texte sind an **einer zentralen Stelle** gesammelt – Sie müssen **kein HTML/Programmierwissen** haben.

---

## Was ist in diesem Ordner?

| Datei        | Zweck                                                    |
|--------------|----------------------------------------------------------|
| `index.html` | Die fertige Seite **und** zugleich die Vorlage zum Bearbeiten |
| `portrait.png` | Das Portrait-Foto (oben rechts) – einfach ersetzen     |
| `logo.png`   | Das runde Logo – einfach ersetzen                         |
| `README.md`  | Diese Anleitung                                          |

---

## So schauen Sie sich die Seite an

Doppelklicken Sie auf **`index.html`**. Sie öffnet sich im Browser.
(Sie brauchen Internet, damit die Schriftarten von Google geladen werden. Foto, Logo und Farben funktionieren auch offline.)

---

## So ändern Sie Texte (z. B. Angebote, Kontakt, Über mich)

1. Öffnen Sie **`index.html`** mit einem Texteditor. Auf dem Mac am einfachsten: Rechtsklick auf `index.html` → „Öffnen mit“ → **TextEdit** (oder besser: **VS Code**, falls vorhanden).
2. Ganz oben im Dokument (nach dem Hinweis-Block) beginnt der große Abschnitt **`KONFIGURATION`**. Er ist mit Kommentaren wie `/* ---------- Angebote ---------- */` beschriftet.
3. Ändern Sie nur die Texte **zwischen den Anführungszeichen** `" ... "`.

   Beispiel – so steht es in der Datei:
   ```js
   knopf1: "Erstgespräch vereinbaren",
   ```
   So ändern Sie es:
   ```js
   knopf1: "Kostenloses Erstgespräch",
   ```
4. **Speichern** (Cmd + S) und `index.html` im Browser neu laden.

### Wichtige Regeln beim Bearbeiten
- **Anführungszeichen** `" ... "` NICHT löschen – nur den Text dazwischen ändern.
- **Kommas** zwischen den Zeilen NICHT löschen.
- Die geschweiften Klammern `{ ... }` und die eckigen Klammern `[ ... ]` bitte stehen lassen – sie halten die Bausteine zusammen.
- Für **Zeilenumbruch** im Text einfach einen eigenen Absatz in die Liste `abschaetzeUeber: [ ... ]` ergänzen (jeder Eintrag in Anführungszeichen, durch Komma getrennt).

---

## So ändern Sie das Foto

- Das aktuelle Foto ist **`portrait.png`**.
- Tauschen Sie die Datei einfach durch Ihr neues Foto aus – **wichtig: der Name muss `portrait.png` bleiben** (oder die Zeile `src="portrait.png"` in `index.html` anpassen).
- Empfehlung: Hochformat, schönes warmes Licht, möglichst 4:5. Das Foto wird oben als abgerundetes Portrait angezeigt.

## So ändern Sie das Logo

- Gleiches Prinzip: ersetzen Sie **`logo.png`** (Name beibehalten).
- Aktuell ist darin „Ina Gordon / Systemisch integratives Coaching, Vorträge, Workshops“ – falls sich die Ausrichtung geändert hat, lassen Sie das Logo am besten neu zeichnen und ersetzen die Datei.

---

## So ändern Sie die Farben (fortgeschritten)

Ganz oben in `index.html`, im Bereich `:root { ... }`, stehen alle Farben als Variablen:
```css
--rose:#EC9D8F;   /* Akzentfarbe (Rosen/Terrakotta) – Buttons */
--gold:#D9A82A;   /* Gold – Halbkreis & Nummern */
--sage:#6F8B72;   /* Salbeigrün – Beschriftungen */
--ink:#3E3A35;    /* Haupttext */
```
Tauschen Sie einfach die Hex-Werte (z. B. `#EC9D8F`) durch andere Farben aus. Farb-Codes finden Sie z. B. unter color-hex.com.

---

## Tipps
- **Eine Änderung nach der anderen** machen und nach jedem Speichern neu laden – so finden Sie Fehler leichter.
- Falls nach dem Bearbeiten etwas „kaputt“ aussieht: Sie haben vermutlich ein Anführungszeichen oder Komma entfernt. Schauen Sie in der Zeile, die Sie zuletzt geändert haben, ob die Anführungszeichen `"` noch da sind.
- Eine **Sicherungskopie** von `index.html` aufheben, bevor Sie größere Änderungen machen.
- Kontaktdaten (E-Mail, Telefon, Web) stehen im Abschnitt `kontakt: { ... }` – dort auch die Links („E-Mail schreiben“, Telefon) automatisch angepasst.

Viel Erfolg!
