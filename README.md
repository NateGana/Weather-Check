# 🌧️ RainCheck — Live Rain & Weather Monitoring System

RainCheck is a single-file, responsive web app that shows real-time rain forecasts, precipitation probability, humidity, and weather alerts for any city — or your current location. No build tools, no server, no API key. Just open `index.html` in a browser.

![tech](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JS-38bdf8)
![api](https://img.shields.io/badge/data-Open--Meteo%20API-22d3ee)
![license](https://img.shields.io/badge/license-MIT-94a3b8)

## ✨ Features

- **🔍 City search with autocomplete** — type any city name and pick from live suggestions
- **📍 Use current location** — one tap, powered by the browser Geolocation API
- **🌡️ Live weather dashboard** — current temperature, condition, and an animated rain overlay that reacts to real precipitation intensity
- **☔ Rain risk indicator** — color-coded badge: `No Rain`, `Light Drizzle`, or `Heavy Rain Warning`
- **📊 Rain status stats** — precipitation probability (%), precipitation amount (mm), humidity (%), wind speed (km/h)
- **🕐 24-hour rain forecast** — horizontally scrollable hourly cards
- **⭐ Saved favorite locations** — bookmark cities to a quick-access list stored in `localStorage`

## 🛠️ Tech Stack

- Pure **HTML5**, **CSS3**, **Vanilla JavaScript (ES6+)**
- No frameworks, no build step, no `npm install`
- Live data from the free [Open-Meteo API](https://open-meteo.com) (geocoding + forecast) — no API key required
- Everything lives in **one file**: `index.html`

## 🚀 Getting Started

1. Clone or download this repository:
   ```bash
   git clone https://github.com/<your-username>/raincheck.git
   ```
2. Open `index.html` directly in any modern browser (Chrome, Edge, Firefox).
   - No local server or XAMPP needed.
   - An internet connection is required to fetch live weather data.
3. Search a city, or tap **Use Current Location**, and the dashboard updates automatically.

## 📁 Project Structure

```
raincheck/
├── index.html   # Everything: markup, styles, and app logic in one file
└── README.md    # This file
```

## 🌐 API Reference

RainCheck calls two free, key-less Open-Meteo endpoints:

| Purpose            | Endpoint                                             |
|--------------------|-------------------------------------------------------|
| City search         | `https://geocoding-api.open-meteo.com/v1/search`      |
| Weather forecast     | `https://api.open-meteo.com/v1/forecast`             |

Current weather, hourly temperature, precipitation probability, precipitation amount, humidity, wind speed, and WMO weather codes are pulled live for every request.

## 🎨 Design

Dark glassmorphic weather UI — deep navy background (`#0f172a`), frosted-glass cards, electric sky-blue and cyan accents, with an ambient animated rain layer behind the hero temperature display whose density scales with real precipitation intensity.

## 🗺️ Roadmap Ideas

- [ ] 7-day forecast view
- [ ] Severe weather push notifications
- [ ] Unit toggle (°C / °F, km/h / mph)
- [ ] Offline caching of the last-viewed location

## 📄 License

MIT — free to use, modify, and share.

---

Built as part of a BSIT coursework/portfolio project. Weather data courtesy of [Open-Meteo](https://open-meteo.com).
