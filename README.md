Weather App 🌤️

A sleek Flutter weather application that shows the current temperature and city based on your location. This app uses OpenWeatherMap API to fetch real-time weather data.

Features ✨

Automatically detect current location and fetch weather.

Displays city name and temperature in Celsius.

Handles location permissions gracefully.

Shows a loading indicator while fetching data.

Lightweight and easy to extend for additional features.

Getting Started 🚀
1. Clone the repository
git clone https://github.com/yourusername/weather_app.git
cd weather_app

2. Install dependencies
flutter pub get

3. Add your OpenWeatherMap API key

In lib/services/weather_service.dart:

final _weatherService = WeatherService('YOUR_API_KEY_HERE');


Get a free API key from OpenWeatherMap
.

4. Run the app
flutter run

Dependencies 📦

http
 – For making API requests.

geolocator
 – For retrieving device location.

geocoding
 – For reverse geocoding coordinates into city names.

Add to pubspec.yaml:

dependencies:
  flutter:
    sdk: flutter
  http: ^1.1.0
  geolocator: ^9.0.2
  geocoding: ^2.0.1

Project Structure 📁
lib/
├─ main.dart
├─ models/
│  └─ weather_model.dart      # Weather data model
├─ services/
│  └─ weather_service.dart    # API and location logic
└─ pages/
   └─ weather_page.dart       # UI screen

How It Works ⚡

Fetch Location: The app requests the device location and resolves it to a city name.

Fetch Weather: Calls the OpenWeatherMap API using the city name.

Display Data: Shows the city name and temperature in a clean UI.

Future Improvements 🔮

Manual city search.

Additional weather details like humidity, wind speed, and forecast.

Refresh button to update weather in real-time.

Enhanced UI with animations and icons.

License 📝

This project is open-source and available under the MIT License.
