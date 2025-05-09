# Weather App

A sleek, responsive web-based weather widget that displays real-time weather data for Cookeville, TN using the Open-Meteo API. The app includes current temperature, humidity, precipitation probability, and dynamic weather condition icons—all styled with Bootstrap 5 and Bootstrap Icons.

## Features

- Location: Displays current weather for Cookeville, TN (static for now, but can be expanded to support multiple cities)
- Current Temperature in Fahrenheit
- Precipitation Probability and Humidity Percentage
- Weather condition icons that change dynamically based on real-time data
- Displays today’s date
- Fully responsive layout using Bootstrap
- Progressive Web App (PWA) ready with support for mobile icons and manifest

## Technologies Used

- HTML5, CSS3, JavaScript (ES6)
- Bootstrap 5.3.3
- Bootstrap Icons
- Open-Meteo API

## How It Works

- On page load, the JavaScript fetches current weather data from the Open-Meteo API using hardcoded coordinates for Cookeville, TN.
- It parses temperature, humidity, and precipitation probability from the response and updates the UI.
- Based on the `weather_code` provided by the API, an appropriate Bootstrap Icon is selected to represent the weather condition visually.

## API Reference

**Open-Meteo API**
- Endpoint: `https://api.open-meteo.com/v1/forecast`
- Parameters used:
- `latitude`, `longitude`
- `current=temperature_2m,relative_humidity_2m,weather_code`
- `hourly=precipitation_probability`
- `temperature_unit=fahrenheit`
- `timezone=America/Chicago`

Full documentation: [https://open-meteo.com](https://open-meteo.com)

## Customization Tips

- To change the location, update the latitude and longitude in the `apiURL` inside the `<script>` tag.
- You can re-enable or customize the 7-day forecast section by uncommenting the related HTML and expanding the API call.

## License

This project is open source and available under the [MIT License](LICENSE).

## Credits

- Weather data provided by [Open-Meteo](https://open-meteo.com)
- UI components and styling via [Bootstrap](https://getbootstrap.com) and [Bootstrap Icons](https://icons.getbootstrap.com)
