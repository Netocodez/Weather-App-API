
# Weather App (API)

This is a simple Weather App built with React that allows users to search for a city and view real-time weather information using the OpenWeatherMap API.

The app demonstrates:

Handling user input with React state (useState)

Fetching data from an external API (fetch)

Error handling and conditional rendering in React


## Features

- Search for any city worldwide
- Displays temperature (in Celsius)
- Shows current weather condition (e.g.,  cloudy, sunny)
- Displays humidity level
- Shows country code of the city
- Handles errors (e.g., invalid city      name, network issues)


## Technologies Used

React (Frontend library)

JavaScript (ES6+)

CSS for basic styling

OpenWeatherMap API for weather data
## Project Structure

weather-app/
│── src/
│   ├── App.tsx          # Main React
│   ├── styles.css      # Styling
│   └── index.js        # App entry point│
│── package.json        # Dependencies & scripts
│── README.md           # Documentation
## Installation

1. Clone the repository
    git clone https://github.com/your-username/weather-app.git
    cd weather-app

2. Install dependencies
   npm install

3. Add your OpenWeatherMap API key
    - Sign up at OpenWeatherMap
    - Get your API key
    - Replace API_KEY in App.js:

4. Run the development server
    npm start

## Project Structure

weather-app/
│── src/
│   ├── App.tsx          # Main React
│   ├── styles.css      # Styling
│   └── index.js        # App entry point│
│── package.json        # Dependencies & scripts
│── README.md           # Documentation
## Usage

Enter a city name in the input box

Click Get Weather

View weather details such as:
    - City name
    - Country code
    - Temperature in Celsius
    - Weather description (e.g., "clear sky")
    - Humidity

Example
Search: London
Output:
    City: London
    Country Code: GB
    Temperature: 18°C
    Condition: scattered clouds
    Humidity: 72%

## Code Highlights

const [city, setCity] = useState("");   // Store input city name
const [weather, setWeather] = useState(null); // Store API response
const [error, setError] = useState(""); // Store error messages

value={city} binds the input to the state
onChange={(e) => setCity(e.target.value)} updates the state when typing
getWeather() fetches data from OpenWeatherMap
## Future Improvements

Add loading spinner while fetching data

Show 5-day forecast instead of just current weather

Display weather icons (e.g., ☀️ 🌧️ ❄️)

Improve UI with frameworks like TailwindCSS or Material UI
## License

This project is licensed under the MIT License.

