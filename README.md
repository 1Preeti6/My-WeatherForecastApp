# Weather Forecast Web App

A simple weather app that shows the current weather for any city, with a frosted-glass interface over a blurred background.

## Features

- Search any city by name (click the search icon or press Enter)
- Current temperature, weather description, wind speed and humidity
- Weather icon that changes with the conditions (clear, clouds, rain, drizzle, snow, mist, haze)
- Friendly 404 screen when a city isn't found
- Frosted-glass card (`backdrop-filter`) over a blurred background image

## Tech Used

- HTML5
- CSS3
- JavaScript
- [OpenWeatherMap API](https://openweathermap.org/api) (Current Weather Data)

## Project Structure

```
Weather Forecast Web App/
├── index.html
├── style.css
├── app.js
├── README.md
└── images/
    ├── bg.jpg
    ├── clear.png
    ├── clouds.png
    ├── drizzle.png
    ├── haze.png
    ├── humidity.png
    ├── mist.png
    ├── rain.png
    ├── search.png
    ├── snow.png
    └── wind.png
```

## Getting Started

1. **Clone or download** this repository.
```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
```
2. **Get a free API key** from [OpenWeatherMap](https://openweathermap.org/api). New keys can take a little while to activate.
3. **Add your key** in `app.js`:
```javascript
   const apiKey = "YOUR_API_KEY_HERE";
```
4. **Open `index.html`** in your browser (or use the VS Code Live Server extension).
5. Click **Get Start**, type a city and search.

> **Note:** Never commit a real API key to a public repository. Use a private repo, or replace the key with a placeholder before pushing.

## How It Works

1. The app sends the city name to the OpenWeatherMap endpoint `/data/2.5/weather`.
2. The JSON response is used to fill in the temperature, description, wind and humidity.
3. The `weather[0].main` value (for example `Clouds` or `Rain`) selects which icon to display.
4. If the API returns a 404, the app shows the "Page Not Found" screen.

## Ideas for Improvement

- Change the background image with the weather and time of day
- 5-day forecast
- °C / °F toggle
- "Use my location" button
- Hide the API key behind a small backend

## Credits

Weather data provided by [OpenWeatherMap](https://openweathermap.org).
