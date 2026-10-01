# SELF//RECON — Digitaler Selbst-Check

Ein persönliches **Selbst-Audit-Werkzeug** im Hacker-Look. Es hilft dir herauszufinden,
was unter **deinem** Namen und mit **deinem** Gesicht über dich im Netz auffindbar ist —
damit du deinen eigenen digitalen Fußabdruck prüfen und aufräumen kannst.

> **Nur für den eigenen Gebrauch gedacht.** Das Werkzeug legt kein heimliches Profil über
> fremde Personen an und durchsucht das Netz nicht selbstständig. Es bündelt öffentliche
> Suchen, analysiert dein eigenes Foto und fasst deine eigenen Funde zusammen.

## Was es kann

1. **Ziel-Profil (DU)** — Name, Ort und eigene Merkmale eingeben (bleibt lokal im Browser).
2. **Biometrie-Scan** — Foto hochladen oder per Webcam aufnehmen; animiertes Gesichts-Mesh
   im Film-Look. Reine lokale Visualisierung, es wird **niemand identifiziert**.
3. **Recon-Launcher** — fertige Such-Links für Google, Bing, DuckDuckGo, Yandex, Brave,
   Bild-Rückwärtssuche (Lens, Yandex, TinEye, PimEyes-Selbstcheck), soziale Netzwerke und
   People-Search-Broker. Öffnet etablierte Suchmaschinen in neuen Tabs.
4. **Metadaten-Forensik (EXIF)** — liest GPS-Standort, Kameramodell und Aufnahmezeit aus
   deinem Foto aus (komplett lokal) und kann die Metadaten per Klick entfernen.
5. **KI-Analyse** — große Modellauswahl:
   - **Kostenlos:** Google Gemini (Free Tier), Groq, OpenRouter (viele `:free`-Modelle),
     Mistral, Cloudflare Workers AI, Together.
   - **Eigener Key:** OpenAI, Anthropic Claude, DeepSeek, xAI Grok.
   - **Lokal / eigene KI:** Ollama und LM Studio (laufen auf deinem Rechner) sowie ein
     frei konfigurierbarer OpenAI-kompatibler Endpunkt.

   Teil A analysiert dein eigenes Foto auf verräterische Details (Hintergrund, Schilder,
   Logos …). Teil B fasst die Fundstücke, die du selbst gesammelt hast, zu einem
   strukturierten Selbst-Steckbrief zusammen.
6. **Gegenmaßnahmen** — Opt-out- und Lösch-Links sowie eine DSGVO-Kurzanleitung.

## Datenschutz

- Läuft als **eine einzige HTML-Datei**, komplett im Browser. Kein Server, kein Tracking.
- Bild, Name und API-Keys verlassen dein Gerät nur, wenn du selbst eine Suche oder eine
  Cloud-KI-Analyse startest. API-Keys werden ausschließlich lokal (`localStorage`) gespeichert.
- Für maximale Privatsphäre: **Ollama/LM Studio** verwenden — dann bleibt auch die KI lokal.

## Nutzung

`index.html` im Browser öffnen. Fertig. Nichts zu installieren.

### Hinweise

- **CORS:** Manche Anbieter erlauben keine direkten Browser-Anfragen. Klappt einer nicht,
  funktionieren meist Gemini, Groq, OpenRouter oder Anthropic.
- **Ollama im Browser:** mit `OLLAMA_ORIGINS=*` starten, sonst blockt der Browser.
- **Bild-Rückwärtssuche:** Der Browser kann aus Sicherheitsgründen kein lokales Bild
  automatisch in eine fremde Suchmaschine laden — den Button anklicken und das Foto dort
  hineinziehen.

## Rechtliches

Nutzung nur für den eigenen Selbst-Check. Das Ausforschen anderer Personen ohne deren
Einwilligung kann Persönlichkeits- und Datenschutzrechte verletzen (u. a. DSGVO, KUG).
Die Verantwortung liegt bei der nutzenden Person.
