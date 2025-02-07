# Scripting-and-Programming-Project
WGU D493 Performance Assessment

# Weather Prediction Python Application

# Project Overview

This project retrieves weather data from the Historical Weather API for Charlottesville, VA,
focusing on January 26th for a span of 5 years. The retrieved data is stored in a SQLite database using SQLAlchemy,
allowing efficient data management and access. The program supports queries to analyze the weather data and outputs the
results in a structured format. Additionally, unit tests are included to verify the functionality and reliability of
the code.

# Required Python Packages

The necessary packages for running the program can be found under the requirements.txt file.

Libraries included:
- pytest - for running tests
- requests - for making API requests
- SQLAlchemy - for managing the SQLite database through ORM
- tabulate - for formatting and displaying data in table form

To install these packages, run:

pip install -r requirements.txt


# Program Structure

- Class.py:

* Contains the WeatherData class, responsible for automatically fetching the weather data from the API.
* Includes 4 methods to retrieve the mean temperature, maximum wind speed, and the precipitation sum.

- Main.py:

* Creates an instance of the WeatherData class.
* Contains a second class for managing the SQLite database and creating a table for storing the weather data.
* Queries the database and outputs a formatted table displaying the weather data.

# Sample Output

+--------+------+--------+----------------+----------------+----------------+--------------------+--------------------+--------------------+-----------------------+
| Month | Day | Year | Avg Temp (°F) | Min Temp (°F) | Max Temp (°F) | Avg Wind Speed (mph) | Min Wind Speed (mph) | Max Wind Speed (mph) | Precipitation (inches) |
+--------+------+--------+----------------+----------------+----------------+--------------------+--------------------+--------------------+-----------------------+
| 1 | 26 | 2020 | 39.7 | 39.7 | 39.7 | 9.7 | 9.7 | 9.7 | 0.0 |

# Tests

Unit tests are included to verify the correct functioning of the weather data fetching, database insertion,
and querying processes.

To run the tests, use the following command in the terminal:

python -m unittest test.py

If the tests are successful, the output will confirm that all tests have passed.
