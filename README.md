# weather_forecast
## Project overview
This weather forecast app provides users with real-time weather data, depicting factors such as temperature, description, feel temperature, humidity, pressure and wind speed, as well as air quality information and NASA's Astronomical Picture of the Day (APOD). The application uses three APIs to obtain data. These are OpenWeather API, NASA API, AQICN API.
## Features
- Receive weather data based on the entered city and country data.
- Display air quality information including AQI, location and major pollutants.
- Access to NASA astronomical picture and information of the day with date selection.
- Interactive map showing the location using MapBox.
## Tech stack 
- Backend: Node.js
- Frontend: HTML, CSS, JavaScript
## Code Structure
- api.js: The main Node.js server file that handles the API routes.
- /weather_d/: 
- weatherrr.html: The page to view weather and air quality
- weatherrr2.html: The initial page with links to weather and NASA pages, and data about natural phenomena
- nasa.html: The  page that displays NASA pictures 
- stil.css: CSS file for styling the frontend forms
- script_weather.js: The file that contains javascript part
## Setup Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/weather_forecast.git
   cd weather_forecast
   npm install
2. **Install dependencies**:
   npm install
3. **Create a .env file**:
   openweather_api=your_openweather_api_key
   nasa_api=your_nasa_api_key
   aqicn_api=your_aqicn_api_token
   mapbox_api=pk.eyJ1IjoidHV0c24iLCJhIjoiY20xaGlndXQ4MGJ4dDJxczh0M3RyN3pudSJ9.BRSWNjZtZjMuVx3enGJk-A
4. **Start the server**:
   node api.js
5. **Go to server**:
   Open your browser and go to http://localhost:3000 or follow by the link from terminal
## API Usage
1. **Get Weather Data**
   - Endpoint: `/weather/:city`
   - Method: `GET`
   - Parameters:
      `city`: Name of the city.
   - Response: Weather data for the specified city.
2. **Get Air Quality Data**
   - Endpoint: `/airquality/:city/:country`
   - Method: `GET`
   - Parameters:
     - `city`: Name of the city.
     - `country`: Country name.
   - Response: Air quality data including AQI, location, and major pollutants.
3.  **Get Astronomy Picture of the Day (APOD)**
   - Endpoint: `/nasa/apod`
   - Method: `GET`
   - Parameters:
     - `date`: (optional) Specific date for the APOD.
   - Response: APOD data including image URL and explanation.
## Key design decisions
   **Responsive Design**: Ensured that the front-end is designed to be responsive and user-friendly, utilizing Bootstrap for styling.

   

