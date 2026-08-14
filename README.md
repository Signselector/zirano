# ZIRANO Charging Solutions — Website

Ladeinfrastruktur. Entwickelt für Wachstum.

Statische, animierte B2B-Landingpage für skalierbare DC-Schnellladeinfrastruktur. Keine Build-Tools, keine Abhängigkeiten — `index.html` öffnen genügt.

## Struktur

```
index.html                  komplette Seite (HTML + CSS + JS inline)
assets/
  video/                    8 Loops als MP4 + WebM, je mit Poster-Frame
  img/                      3D-Renders (WebP) + animiertes Systemdiagramm (SVG)
  icons/                    11 animierte Icons (SVG)
```

## Sektionen

| # | Sektion | Inhalt |
|---|---|---|
| — | Hero | Videoloop, animierte Kennzahlen, zwei CTAs |
| 01 | Ausgangslage | Netzanschluss als Nadelöhr |
| 02 | Technologie | Batteriespeicher, animiertes Systemdiagramm |
| 03 | Mehrwert | Business Case für den Standort |
| 04 | Full-Service | 11 Leistungsbereiche |
| 05 | Projektablauf | 5 Schritte bis zum Roll-out |
| 06 | Standortnetz | Skalierung über das Portfolio |
| 07 | Hardware | Ladesäulen und Standards |
| — | Kontakt | CTA mit animiertem Canvas-Hintergrund |

Die Reihenfolge folgt den Fragen eines Standortverantwortlichen: Warum ist das bisher nicht passiert → wie löst ihr es → was bringt es mir → was übernehmt ihr → was muss ich tun → skaliert das → taugt die Technik.

## Technik

- **Typografie:** Space Grotesk (Display) + Inter (Fließtext) via Google Fonts
- **Farben:** Graphit `#101418`, Hell `#F7F9FA`, Akzent Elektrisch-Grün `#00D97A`
- **Motion:** Scroll-Reveals, perspektivische 3D-Frames, Tilt-Karten, Hero-Parallax, hochzählende Kennzahlen, animierte SVGs, Canvas-Hintergrund
- **Videos:** WebM (VP9) mit MP4-Fallback, `autoplay muted loop playsinline`, Poster-Frames für Lazy Loading
- **Barrierefreiheit:** `prefers-reduced-motion` wird durchgängig respektiert — Animationen aus, Endzustände sichtbar
- **Gewicht:** ~6 MB Medien gesamt, größte Einzeldatei 1,4 MB

## Hosting

Reine statische Dateien — funktioniert auf Vercel, Netlify, GitHub Pages, S3 oder jedem Webserver ohne Konfiguration.

## Offene Punkte vor Livegang

- Kontaktdaten im Footer und in den CTAs sind Platzhalter (`kontakt@zirano.example`, Telefonnummer)
- Impressum und Datenschutz sind noch nicht verlinkt
- Kennzahlen (99,8 % Verfügbarkeit, Kostenangaben in Sektion 01) fachlich gegenprüfen
