# KI-Auffindbarkeit – Prüfbericht und Entwurf (24.11.2026)

## Freigabestatus
Nur Arbeitszweig `entwurf-ki-sichtbarkeit-2026-11-24`. Keine Änderung an `main`, keine Produktionsveröffentlichung.

## Bestätigte Grundlagen (GitHub, Stand 24.11.2026)
- `robots.txt`: `User-agent: * / Allow: /`, Sitemap angegeben. Keine Sperre von OAI-SearchBot, Googlebot, Bingbot oder PerplexityBot. Zugänglichkeit per WAF/Netzwerk ist damit **nicht** bewiesen.
- `sitemap.xml`: Startseite und vier separate Leistungsseiten.
- Hauptseite ist laut Google Search Console Screenshot vom 24.11.2026 im Google-Index; Sitemap wurde eingereicht, fünf URLs wurden entdeckt. Indexstatus der vier neuen Unterseiten **noch unbekannt**.
- Die Live-Seite konnte über die externe Abrufverbindung nicht zuverlässig geprüft werden. Kein nachgewiesener Live-Test gegen ChatGPT, Gemini, Copilot oder Perplexity.
- Keine garantierte Platzierung oder KI-Empfehlung.

## Im Entwurf vorgenommen
- Faktenbasiertes LocalBusiness-JSON-LD mit Hannover, Garbsen und Langenhagen, Kontakt und Leistungslinks; ohne erfundene Bewertungen, Preise oder Eröffnungszeiten.
- Sichtbare ausführliche Fragen und Antworten zu Reinigung, Hausmeisterservice, Trockenbau, Einsatzgebiet und unverbindlichen Anfragen.
- Canonical der Startseite, wenn vorher nicht vorhanden.

## Nicht verändert
- `robots.txt` muss nicht künstlich für jeden Bot ergänzt werden: vorhandene Allow-all-Regel reicht grundsätzlich.
- Keine `llms.txt` als angebliche KI-Registrierung angelegt: dafür gibt es keine generelle Ranking- oder Aufnahmegarantie.
- Keine KI-spezifischen Rankingversprechen, Fake-Rezensionen, versteckter SEO-Text, geänderten Festpreise oder ungeprüfte Referenzen.

## Nach Freigabe und Veröffentlichung separat erledigen
1. Google Search Console: URL-Inspektion für alle vier Leistungsseiten; bei Bedarf Indexierung beantragen und Verarbeitungszeit beachten.
2. Bing Webmaster Tools (https://www.bing.com/webmasters/): Property prüfen, Sitemap einreichen, Bing-Indexstatus und gegebenenfalls AI Performance ansehen.
3. Öffentlich angezeigte Firmendaten / Branchen in Google Business Profile, Bing Places, Gelbe Seiten und Das Örtliche angleichen (besondere Vorsicht bei der Kategorie Textilreinigung).
4. Fotos echter Arbeiten nur mit Kundenfreigabe ergänzen, echte Referenzen und Bewertungen sammeln.
5. Mit neutralen Suchfragen und wechselnden Standorten auf ChatGPT Search, Gemini/AI Mode, Copilot und Perplexity testen; Treffer samt Quellen/Datum dokumentieren. KI-Ausgaben können variieren.
6. Im Vercel-Projekt Sicherheitsregeln/WAF und Bot-Zugriff prüfen, falls Suchbots trotz robots.txt scheitern.
7. Rechtliche Angaben, für Hausmeister-/Trockenbauarbeiten zulässigen Gewerbeumfang und Kontaktfunktionen vor Produktionsfreigabe prüfen.

## Offizielle Dokumentation
- https://developers.openai.com/api/docs/bots
- https://developers.google.com/search/docs/appearance/ai-features
- https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a
- https://docs.perplexity.ai/docs/resources/perplexity-crawlers
