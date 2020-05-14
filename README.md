# docker-weather-dashboard

Use **node-red** to store the weather data of 4 cities in an InfluxDB database and show it in a dashboard.

Dockerization of [weather-bot project](https://github.com/opatiny/weather-bot).

## Access the dashboard


## How to run the project

### Clone
```bash
git clone https://github.com/opatiny/docker-weather-dashboard
```

### Add your environment variables

Copy the `docker-compose.yml.example` file to `docker-compose.yml` and replace the environment variable with your data:
```yml
    environment:
      OWM_ID: <your openweathermap appid here>
```

### Start the dashboard

Run the following command:

```bash
docker-compose up -d --build
```

Or use the script if you have node.js:

```bash
npm start
```

### Stop the dashboard

Run the following command:

```bash
docker-compose down
```

Or use this script if you have node.js:

```bash
npm run stop
```
