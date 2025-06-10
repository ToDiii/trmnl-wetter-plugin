# TRMNL Wetter Plugin

## Übersicht

Modernes Wetter-Display für TRMNL im Querformat (800x480 E-Ink Display).  
Zeigt aktuelles Wetter + 3-Tage-Vorschau mit Icons, Min/Max Temperatur, Regenwahrscheinlichkeit, Wind usw.  
Sprache: **Deutsch**  
Optimiert für **1-Bit E-Ink** → keine Graustufen!

## Installation

1. Ordnerstruktur:

```
TRMNL_Wetter_/
├── plugin.json
├── index.html
├── README.md
└── assets/
    └── icons/
```

2. Icons als 1-Bit PNG (64x64 px), Dateinamen:

- 01d.png, 02d.png, 03d.png, 04d.png, 09d.png, 10d.png, 11d.png, 13d.png, 50d.png
- wind.png, humidity.png, sunrise.png, sunset.png, clock.png, thermometer.png, rain.png

3. ZIP packen → Struktur muss exakt so sein!

4. Im TRMNL Dashboard:

- Private Plugins → Plugin hochladen → deine ZIP
- Neue Display View → Template: **TRMNL Wetter **
- Update-Intervall: **alle 3 Stunden empfohlen**

## API

- OpenWeatherMap Forecast API
- Dein API Key ist im Template integriert:

```plaintext
https://api.openweathermap.org/data/2.5/forecast?q=YOURTOWN,DE&units=metric&lang=de&appid=DEIN_API_KEY
```

## Icon Mapping

### Dynamische Wetter-Icons (OpenWeatherMap Icon Code → PNG Datei)

| OWM Icon Code | Bedeutung                  | PNG Datei (`/assets/icons/`) |
|---------------|----------------------------|-----------------------------|
| 01d           | Klarer Himmel (Tag)        | 01d.png                     |
| 01n           | Klarer Himmel (Nacht)      | 01d.png (oder eigenes 01n.png) |
| 02d           | Wenige Wolken (Tag)        | 02d.png                     |
| 02n           | Wenige Wolken (Nacht)      | 02d.png (oder eigenes 02n.png) |
| 03d           | Bewölkt                    | 03d.png                     |
| 03n           | Bewölkt                    | 03d.png                     |
| 04d           | Stark bewölkt              | 04d.png                     |
| 04n           | Stark bewölkt              | 04d.png                     |
| 09d           | Regenschauer               | 09d.png                     |
| 09n           | Regenschauer               | 09d.png                     |
| 10d           | Regen (leichter / normaler) | 10d.png                     |
| 10n           | Regen (leichter / normaler) | 10d.png                     |
| 11d           | Gewitter                   | 11d.png                     |
| 11n           | Gewitter                   | 11d.png                     |
| 13d           | Schnee                     | 13d.png                     |
| 13n           | Schnee                     | 13d.png                     |
| 50d           | Nebel / Dunst              | 50d.png                     |
| 50n           | Nebel / Dunst              | 50d.png                     |

### Statische Symbole (immer verwendet im Template)

| Funktion               | PNG Datei (`/assets/icons/`) |
|------------------------|-----------------------------|
| Windgeschwindigkeit    | wind.png                    |
| Luftfeuchtigkeit       | humidity.png                |
| Sonnenaufgang          | sunrise.png                 |
| Sonnenuntergang        | sunset.png                  |
| Letzte Aktualisierung  | clock.png                   |
| Temperatur             | thermometer.png             |
| Regenwahrscheinlichkeit| rain.png                    |

## Hinweise

- Template & Mapping sind fertig vorbereitet
- Fallback bei API Fehler: **"Daten derzeit nicht verfügbar"** wird angezeigt
- Darstellung ist **1-Bit optimiert für E-Ink → keine Graustufen**
- Night-Icons (`01n`, `02n` etc.) können identisch zu Day-Icons gemappt werden → oder eigene Icons bauen

## Lizenz

MIT License
