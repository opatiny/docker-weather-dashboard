# docker-weather-dashboard


Dockerization of [weather-bot project](https://github.com/opatiny/weather-bot).

This project uses sub-modules!

## How to use it
### Clone the project
```bash
git clone --recurse-submodules https://github.com/opatiny/docker-weather-dashboard
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

## For development only: Updating the submodules

```bash
git submodule update --recursive --remote
```

Or use the script:
```bash
npm run update
```
