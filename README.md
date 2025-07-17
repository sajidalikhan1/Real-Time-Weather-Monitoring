# Real-Time Weather Monitoring System

This project is a real-time weather monitoring application that fetches data from the OpenWeatherMap API and provides summaries, alerts, and weather forecasts for specified locations. The system supports configurable thresholds for alerts, calculates daily summaries, and displays key weather parameters such as temperature, humidity, and wind speed.

## Features
- **Weather Data Retrieval**: Retrieves current weather and forecast data from OpenWeatherMap API.
- **Daily Summaries**: Calculates average, minimum, and maximum temperatures, average humidity, and wind speed.
- **Alerts**: Configurable user thresholds for temperature or specific weather conditions, with alerts triggered when thresholds are breached.
- **Responsive UI**: Displays real-time weather data, daily summaries, and a 5-day forecast in a user-friendly interface.



---

## Prerequisites

- **Node.js** and **Express.js** for backend and **React** for frontend development
- **MongoDB** for data storage (either locally or a cloud instance)
- **OpenWeatherMap API Key** for fetching weather data

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/sajidalikhan1/Real-Time-Weather-Monitoring-App.git

cd Real-Time-Weather-Monitoring-App
```

### 2. Setting Up the Backend

#### a. Navigate to the backend directory:
```bash
 cd backend
 ```

#### b. Install backend dependencies:
```bash
npm install
```

#### c. Configure Environment Variables:
Create a ``.env`` file in the ``backend/`` folder with the following content:
``` Plaintext
API_KEY=your_openweathermap_api_key

MONGODB_URI=mongodb://127.0.0.1:27017/weatherDB
           or
MONGODB_URI=MONGODB_URI=mongodb+srv://username:password@cluster0.mongodb.net/mydatabase?retryWrites=true&w=majority

```

1. ``API_KEY:`` Your OpenWeatherMap API key.
2. ``MONGODB_URI:`` URI for connecting to MongoDB (replace with your MongoDB instance).

#### d. Run the Backend:
```bash
node App.js
```
1. The backend server should be running at http://localhost:5000.

2. You should see a message in the console indicating a successful connection to MongoDB and fetching of weather data.


### 3. Setting Up the Frontend

#### 1. Navigate to the frontend directory:

```bash
cd frontend
```

#### b. Install frontend dependencies:

```bash
npm install
```

#### c. Start the frontend

```bash
npm start
```
* The frontend should be running at http://localhost:3000

* Access the application by opening a browser and navigating to http://localhost:3000


### Usage
*  **Access the Application:**  Go to http://localhost:3000

* **Search for a Location:** Enter a location in the search bar to view the weather summary and 5-day forecast.

* **Set Thresholds and Configure Alerts:**
Thresholds for temperature or specific conditions can be set in the backend. Alerts will trigger in the console if thresholds are breached.



## Project Structure in Detail
### Backend:
1. **app.js:** The entry point for the backend server. Initializes Express, connects to MongoDB, and sets up routes.

2. **env/:** Contains environment variables (API keys, database URIs).

3. **db/:** MongoDB models for weather data and daily summaries.

4. **routes/:** Express routes for handling weather data requests.

5. **services/:** Contains logic for interacting with the OpenWeatherMap API and processing weather data.

### Frontend :

1. **src/App.js:** Main React component displaying current weather, forecast, and alerts.

2. **public/:** Static files and assets.

3. **package.json:** Lists dependencies and scripts for frontend development.




## Technologies Used:

* **Node.js** and Express for the backend server
* **MongoDB** for data storage
* **React** with **Material-UI** for frontend interface
* **OpenWeatherMap API** for weather data
#
