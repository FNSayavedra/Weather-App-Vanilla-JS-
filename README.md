# Weather App (Vanilla JS)

A simple, beginner-friendly weather app built with **HTML, CSS, and vanilla JavaScript**.  
It fetches current weather data from the **OpenWeather API** by city name and displays:

- City and country  
- Temperature in **°C** (converted from Kelvin)  
- Humidity  
- Weather description  
- Official OpenWeather icon

---

## How it works

1. The user enters a city and clicks **Search**.  
2. The app calls `https://api.openweathermap.org/data/2.5/weather` with the provided city and your API key.  
3. The JSON response is parsed and rendered into the page (no frameworks).  
4. Basic styling is provided via a custom CSS file and the **Poppins** font.

---

## Tech stack

- **HTML5** for structure  
- **CSS3** for styling (centered, responsive container)  
- **JavaScript (fetch API)** for network requests and DOM updates  
- **OpenWeather** for weather data

---

## Getting started

1. Get a free API key from **OpenWeather**.  
2. In `script.js`, set your key:

```js
const API_KEY = 'YOUR_API_KEY_HERE';
Open index.html in your browser and search for any city.

Note: The current version converts Kelvin to Celsius manually.
You can also request metric units directly by appending &units=metric to the API URL if you prefer.

Possible improvements
Handle errors (invalid city, network issues) with user-friendly messages.

Use &units=metric to avoid manual conversion.

Add loading states and keyboard submit (Enter key).
