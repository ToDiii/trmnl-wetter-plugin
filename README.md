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
