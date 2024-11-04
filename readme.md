
---

# Weather CLI

A simple Python command-line application that retrieves and displays weather information for a specified city, using the [OpenWeather API](https://openweathermap.org/).

## Features

- Get current weather and temperature for any city.
- Display weather conditions with corresponding emojis and colors.
- Supports both metric (Celsius) and imperial (Fahrenheit) units.

## Prerequisites

- Python 3.x
- An OpenWeather API key. Sign up for free at [OpenWeather](https://home.openweathermap.org/users/sign_up).

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/weather-cli.git
   cd weather-cli
   ```

2. **Configure the API key:**
   - Create a file named `secrets.ini` in the root directory.
   - Add your OpenWeather API key as follows:
     ```ini
     [openweather]
     api_key=<YOUR-OPENWEATHER-API-KEY>
     ```

## Usage

Run the program from the command line:

```bash
python weather.py <city_name> [-i]
```

- **city_name**: Name of the city to fetch weather data for.
- **-i, --imperial**: Display temperature in Fahrenheit (optional; defaults to Celsius).

### Examples

1. **Get weather in Celsius**:
   ```bash
   python weather.py London
   ```

2. **Get weather in Fahrenheit**:
   ```bash
   python weather.py London -i
   ```

## Code Structure

- **weather.py**: Main script for handling API requests and displaying weather information.
- **style.py**: Contains styling for colored text output in the terminal.

## Dependencies

- `argparse`
- `json`
- `configparser`
- `urllib`
- [OpenWeather API](https://openweathermap.org/api)

## License

This project is licensed under the MIT License.

---