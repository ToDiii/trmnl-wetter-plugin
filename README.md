# TRMNL Wetter Taufkirchen Plugin

## Installation

1. Ordnerstruktur:
   - plugin.json
   - index.html
   - README.md
   - assets/icons/ → deine eigenen 1-Bit PNGs (siehe Liste)

2. Icons als 1-Bit PNG (64x64 px), Dateinamen:
   - 01d.png, 02d.png, 03d.png, 04d.png, 09d.png, 10d.png, 11d.png, 13d.png, 50d.png
   - wind.png, humidity.png, sunrise.png, sunset.png, clock.png, thermometer.png, rain.png

OWM Icon Code
Bedeutung
PNG Datei (/assets/icons/)
01d
Klarer Himmel (Tag)
01d.png
01n
Klarer Himmel (Nacht)
01d.png (oder eigenes 01n.png)
02d
Wenige Wolken (Tag)
02d.png
02n
Wenige Wolken (Nacht)
02d.png (oder eigenes 02n.png)
03d
Bewölkt
03d.png
03n
Bewölkt
03d.png
04d
Stark bewölkt
04d.png
04n
Stark bewölkt
04d.png
09d
Regenschauer
09d.png
09n
Regenschauer
09d.png
10d
Regen (leichter / normaler)
10d.png
10n
Regen (leichter / normaler)
10d.png
11d
Gewitter
11d.png
11n
Gewitter
11d.png
13d
Schnee
13d.png
13n
Schnee
13d.png
50d
Nebel / Dunst
50d.png
50n
Nebel / Dunst
50d.png

3. ZIP packen → Struktur muss genau so sein!

4. Im TRMNL Dashboard:
   - Private Plugins → Plugin hochladen → deine ZIP
   - Neue Display View → Template: "TRMNL Wetter Taufkirchen"
   - Update-Intervall: alle 3 Stunden empfohlen

5. API
   - OpenWeatherMap Forecast API
   - DEIN API Key → im Template (bereits vorbereitet)

## Hinweise

- Template & Mapping fertig
- Fallback bei API Fehler: "Daten derzeit nicht verfügbar"
- Voll 1-Bit optimiert → E-Ink geeignet

## Lizenz

MIT License
