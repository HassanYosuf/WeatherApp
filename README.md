# Weather App (Spring Boot)

## 📌 Overview
This is a simple **Spring Boot** application that fetches weather forecasts using the **Tomorrow.io API**. The app provides a REST endpoint to get weather details based on location coordinates.

## 🚀 Features
- Fetches weather forecasts from Tomorrow.io
- REST API with Spring Boot
- Uses **RestTemplate** for API calls
- Configurable API key via `application.properties`

## 📂 Project Structure
```
weather-app/
├── src/
│   ├── main/
│   │   ├── java/com/weathermap/weather/
│   │   │   ├── WeatherAppMain.java  # Main Spring Boot application
│   │   │   ├── WeatherController.java  # REST API controller
│   │   ├── resources/
│   │   │   ├── application.properties  # Configuration file
│   ├── test/
├── pom.xml  # Maven dependencies
├── README.md  # Project documentation
```

## 🛠️ Setup & Installation
### 1️⃣ **Prerequisites**
- Java 17 or higher
- Maven installed (`mvn -version` to check)

### 2️⃣ **Clone the Repository**
```
git clone https://github.com/your-username/weather-app.git
cd weather-app
```

### 3️⃣ **Configure API Key**
Edit `src/main/resources/application.properties` and add your Tomorrow.io API key:
```
tomorrow.api.key=YOUR_API_KEY
```

### 4️⃣ **Build & Run the Application**
```sh
mvn clean install
mvn spring-boot:run
```

### 5️⃣ **Test the API**
Open a browser or use `curl` to test the endpoint:
```sh
curl "http://localhost:8080/weather?location=42.3478,-71.0466"
```

## 📜 API Endpoint
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/weather?location={lat,lon}` | Fetches weather data for a given location |

## 🛠 Technologies Used
- **Spring Boot** (Web, RestTemplate)
- **Java 17**
- **Maven**
- **Tomorrow.io API**
