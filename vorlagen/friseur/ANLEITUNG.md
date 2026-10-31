# Friseur-Vorlage – neuen Salon in 5 Minuten

1. Ordner kopieren: `vorlagen/friseur/index.html` → `<salon-name>/index.html` (z. B. `salon-anna/index.html`).
2. Oben in der Datei den Block **STECKBRIEF** ausfüllen (Name, Slogan, Farben, Telefon, Adresse, Öffnungszeiten, Leistungen, Google, Besonderheit, Social, Webhook). Sonst nichts anfassen.
3. Leere Felder (`""` oder `[]`) werden automatisch ausgeblendet.
4. `webhook`: Production-URL aus n8n eintragen. Leer = Demo-Modus (Bestätigung erscheint trotzdem, nichts wird gesendet).
5. Hochladen → Seite liegt unter `https://dominikreger.de/<salon-name>/`.

Das Formular sendet an den Webhook (als Formulardaten):
`salon, leistung, datum, datum_lesbar, uhrzeit, name, telefon, gesendet_am, seite`

Die Seite ist per `noindex` für Google gesperrt und trägt oben den Hinweis „Entwurf von Dominik Reger“.
