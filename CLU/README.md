# Weather Utility

This is a simple command-line utility written in Python that provides weather information based on location.

## Modules and Technology Used

- Python 3.8 and above
- [Requests](https://docs.python-requests.org/en/master/)
- [argparse](https://docs.python.org/3/library/argparse.html)
- [WeatherAPI.com API](https://rapidapi.com/weatherapi/api/weatherapi-com): Used to get weather forecast by location name or coordinates.

## Installation and Setup Instructions

### Clone the Repository:

```bash
$ git clone https://github.com/Adtiya-Mohite-GitHub/CLU_WeatherUtility.git
```
### Install Dependencies:

```bash
pip install -r requirements.txt
```
### API setup 

- Visit (https://rapidapi.com/weatherapi/api/weatherapi-com) for API and subscribe to it's free version which allows API 500,000 requests per month.

- Use GET Realtime Weather API key and replace the text 'Your API key' with your API key in 'weatherandtimeutils.py'

## Usage

- Run the main.py script with appropriate command-line arguments:

    - [weather]: Main command keyword. This is a required positional argument.
    - [mode]: Specify mode:
    - [location]: Get weather by coordinates or location name.
    - [current]: Get weather for the current location.
    - [locationarg]: Argument if location is entered. Optional for location mode.

```bash 
python main.py [weather] [mode] [locationarg]
```

- Run for Information in detai

```bash 
python main.py weather -h 
```

## Examples : 

```bash
python main.py weather location London
python main.py weather current
```  

## Updates : 
- Removed the usecase of 'geocoder' , instead updated 'locationutils.py' with the usecase of 'requests' module for obtaining user's current co-ordinates. Updated on 08 April 2024.
