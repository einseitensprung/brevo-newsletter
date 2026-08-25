# Brevo Newsletter Template — einseitensprung.at

E-Mail-Newsletter-Vorlage für Brevo-Kampagnen von [einseitensprung.at](https://einseitensprung.at), im visuellen Theme der bestehenden Newsletter-Ausgaben (siehe [Archiv](https://einseitensprung.at/newsletter/)).

🔗 [Web-Preview der Vorlage (GitHub Pages)](https://einseitensprung.github.io/brevo-newsletter/newsletter-template.html)

## Inhalt

- `newsletter-template.html` — fertiges, bulletproof E-Mail-HTML zum Import in Brevo (Kampagne → Code-Editor importieren)
- `assets/demo-image-1.svg` — funktionierendes Demo-/Platzhalterbild im Brand-Look (der alte `via.placeholder.com`-Link ist offline), gehostet über GitHub Pages

## Design-Tokens

| Element | Wert |
|---|---|
| Text / Überschriften | `#1F2D3D` (Navy) |
| Marken-Streifen | `#B5E479` (Grün) · `#F5A9D0` (Pink) · `#6FE3E8` (Cyan) |
| CTA-Button | `#8E1963` (Magenta) |
| Footer-Fläche | `#EFF2F7` |
| Schrift | [Josefin Sans](https://fonts.google.com/specimen/Josefin+Sans) (Fallback: Arial/Helvetica) |
| Badges / Footer-Links | Courier New (Monospace, terminal-artiger Look wie auf der Archivseite) |

## Aufbau der Vorlage

1. Mirror-/Browser-Link (`{{ mirror }}`)
2. Marken-Streifen + Logo-Wortmarke
3. Ausgaben-Badge (z. B. `NEWSLETTER #013`)
4. Begrüßung mit Personalisierung (`{{ contact.FIRSTNAME }}`)
5. Beliebig viele Themenblöcke (Bild, Überschrift, Text, CTA-Button)
6. Signatur
7. Footer mit Adresse, Social-Links und Pflicht-Abmeldelink (`{{ unsubscribe }}`)

## Verwendung in Brevo

1. Kampagne anlegen → **Code-Editor importieren** → `newsletter-template.html` hochladen
2. Platzhalterbild(er) durch echte, in Brevo hochgeladene Bilder ersetzen (Demo-SVG dient nur der Vorschau — SVG wird nicht von allen E-Mail-Clients unterstützt, für den Versand PNG/JPG verwenden)
3. Themenblöcke duplizieren/löschen und mit Inhalt befüllen
4. Testmail verschicken und in mehreren Clients (Outlook, Gmail, Apple Mail) prüfen

## Merge-Tags

- `{{ contact.FIRSTNAME }}` — Vorname des Empfängers
- `{{ contact.EMAIL }}` — E-Mail-Adresse des Empfängers
- `{{ mirror }}` — Link „Im Browser ansehen"
- `{{ unsubscribe }}` — Pflicht-Abmeldelink
