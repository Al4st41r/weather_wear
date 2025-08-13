# weather_wear
Vibe coded app to tell me what to wear depending on the weather. 
Minimalist, mobile-first web app that checks the local weather and suggests what layers of clothing to wear — with both text and clean outline icons.

## 🌍 Live Demo
[View on GitHub Pages](https://al4st41r.github.io/weather_wear/)

## ✨ Features
- **Automatic location detection** (with permission) or manual city entry.
- **Default city:** London, UK.
- **Clothing advice** based on temperature, wind, humidity, and conditions (rain/snow).
- **Clean outline icons** alongside text suggestions.
- **Mobile-first responsive design**.

## 🧾 Clothing Rules
The app suggests layers based on the following temperature ranges:

### 20°C and above
- T-shirt (light, breathable fabrics)
- Shirt

### 15°C to 19°C
- T-shirt + Light Jacket
- Long-sleeved Shirt

### 10°C to 14°C
- T-shirt + Shirt
- Long-sleeved Shirt + Light Jacket

### 5°C to 9°C
- T-shirt + Shirt + Jacket
- Warm Coat

### 0°C to 4°C
- Warm Coat + Shirt + T-shirt
- Scarf

### Below 0°C
- Heavy Coat + Layers
- Scarf, Gloves, Hat

### Extra Factors
- Rain → Umbrella
- Snow → Gloves & Hat
- Wind > 30 km/h → Windbreaker
- Humidity > 80% and Temp > 20°C → Breathable fabrics

## ⚙️ How It Works
The app:
1. Fetches weather data via a **Cloudflare Worker**.
2. Displays current conditions and temperature.
3. Suggests clothing layers with icons and text.

## 🚀 Hosting
- **Frontend:** GitHub Pages
- **Weather API proxy:** Cloudflare Worker

## 🛠 Setup
1. Get an [OpenWeatherMap API key](https://openweathermap.org/api).
2. Add it to your Cloudflare Worker script.
3. Deploy the Worker.
4. Update `index.html` to point to your Worker URL.

## 📜 License
MIT License — feel free to fork, modify, and share.