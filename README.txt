BRINGIO – Dual Order System (Version 2)

DATEIEN
- index.html: deutsche Website mit zwei Bestellwegen
- icon.svg, manifest.webmanifest, sw.js: PWA/App-Grundfunktionen

BESTELLWEGE
1) Persönliche Einkaufsliste: Kunde wählt Supermarkt, schreibt Liste und schätzt Warenbudget.
2) Online-Shop: Kunde legt Beispielartikel in den Warenkorb.

WICHTIG – ZAHLUNG
Diese Version versendet eine Anfrage per WhatsApp an die bisher angegebene BRINGIO-Nummer.
Sie nimmt NOCH KEINE Zahlung entgegen. Nach Prüfung der Anfrage muss BRINGIO den endgültigen Betrag bestätigen und dem Kunden einen sicheren Stripe-Zahlungslink senden. Erst nach erfolgreicher Zahlung wird eingekauft.
Kartendaten niemals per WhatsApp abfragen.

STRIPE / AUTOMATISCHE ZAHLUNG
Für eine automatische Zahlung direkt von der Website wird ein Server-Backend benötigt. GitHub Pages ist nur statisches Hosting und kann keine serverseitigen Stripe-Schlüssel sicher speichern. Stripe Checkout muss serverseitig erstellt werden; geheime API-Schlüssel gehören in sichere Server-Secrets, niemals in index.html oder GitHub.
Offizielle Grundlagen:
- Stripe Checkout: https://docs.stripe.com/payments/checkout
- Cloudflare Workers Secrets: https://developers.cloudflare.com/workers/configuration/secrets/
- GitHub Pages Grenzen: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

WICHTIG ZU PREISEN
Die Produktpreise im Demo-Warenkorb sind ausschließlich Platzhalter. Sie sind keine aktuellen Kaufland-/Lidl-/ALDI-/EDEKA-/REWE-Preise. Vor einem öffentlichen Start müssen die Artikel, Preise, Verfügbarkeit, Pfand und eventuelle Ersatzartikel gepflegt und rechtlich geprüft werden.

GITHUB UPDATE
1. Repository Bringio öffnen.
2. Code > Upload files.
3. Die fünf Dateien aus diesem Paket auswählen und hochladen.
4. Commit changes direkt auf main.
5. Nach dem Deployment https://bringio.github.io/ öffnen bzw. die bisherige Website-Adresse neu laden. Wenn die alte Version bleibt, Browser-Refresh/Cache leeren.

VOR DEM ECHTEN START
Impressum, Datenschutzerklärung, AGB/Widerruf soweit anwendbar, Preis-/Lieferbedingungen, Gewerbe- und Steuerfragen sowie Zahlungs- und Erstattungsprozess klären. Nicht als live zahlungsfähig bewerben, bevor Stripe/Backend und diese Punkte eingerichtet sind.
