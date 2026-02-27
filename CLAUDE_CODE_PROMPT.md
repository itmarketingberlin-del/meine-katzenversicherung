# CLAUDE CODE PROMPT – KatzenSchutz Landingpage

## Kontext
Ich bin ARAG-Versicherungsvermittler und habe eine fertige Landingpage für Katzenkrankenversicherungen. Die Seite ist eine einzelne `index.html` Datei ohne Framework. Sie soll auf GitHub Pages unter der Domain `meine-katzenversicherung.info` (IONOS) deployed werden.

## Was ich brauche

### 1. Kontaktdaten eintragen
Ersetze in `index.html` folgende Platzhalter:
- `ihre-email@beispiel.de` → **[MEINE EMAIL]** (kommt an 3 Stellen vor)
- `491234567890` → **[MEINE WHATSAPP NUMMER ohne + z.B. 4917612345678]**
- `KatzenSchutz · Ihr Versicherungsvermittler` im Footer → **[MEIN NAME]**

### 2. Impressum-Seite erstellen
Erstelle eine `impressum.html` mit folgendem Inhalt:
- Name: **[MEIN VOLLSTÄNDIGER NAME]**
- Adresse: **[STRASSE, PLZ ORT]**
- Telefon: **[TELEFONNUMMER]**
- E-Mail: **[EMAIL]**
- Berufsbezeichnung: Versicherungsvermittler (§ 34d GewO)
- Aufsichtsbehörde: IHK [MEINE STADT]
- DSGVO-konformer Hinweis zum Kontaktformular

### 3. Datenschutz-Seite erstellen
Erstelle eine `datenschutz.html` mit:
- DSGVO-konformer Datenschutzerklärung
- Hinweis auf Kontaktformular (Daten werden per E-Mail übermittelt)
- Hinweis auf Unsplash-Foto (lizenzfrei)
- Keine Cookies, kein Tracking
- Verantwortlicher: **[MEIN NAME & ADRESSE]**

### 4. Navigation anpassen
Füge in `index.html` im Footer Links zu Impressum und Datenschutz ein:
```html
<a href="impressum.html">Impressum</a> | <a href="datenschutz.html">Datenschutz</a>
```

### 5. Kontaktformular verbinden (Formspree)
Ersetze das aktuelle `mailto:`-Formular durch Formspree:
- Gehe auf formspree.io, erstelle kostenlosen Account, erstelle ein neues Formular
- Ersetze die Form-Action mit der Formspree-URL: `https://formspree.io/f/[MEIN-FORM-ID]`
- Das Formular soll bei Absenden direkt eine E-Mail an mich schicken – ohne dass der Browser des Nutzers ein E-Mail-Programm öffnet
- Nach erfolgreichem Absenden soll eine Danke-Meldung erscheinen

### 6. GitHub deployment
Deploye alle Dateien (`index.html`, `impressum.html`, `datenschutz.html`) in das Repository:
`https://github.com/itmarketingberlin-del/meine-katzenversicherung`

Dann aktiviere GitHub Pages:
- Branch: main
- Root-Verzeichnis: /

Danach füge eine `CNAME`-Datei hinzu mit dem Inhalt:
```
meine-katzenversicherung.info
```
Das verbindet die IONOS-Domain mit GitHub Pages.

## Technische Details
- Kein Framework, kein Build-Tool – reines HTML/CSS/JS
- Fonts via Google Fonts (Lora + Inter)
- Foto via Unsplash CDN (bereits eingebunden)
- Kein localStorage, keine Cookies
- Mobile-responsive bereits fertig

## Wichtig
- Kein ARAG-Logo oder ARAG-Verweis darf sichtbar sein
- Die Seite positioniert mich als unabhängigen Vermittler
- Seriöses, professionelles Design – keine Spielerei
