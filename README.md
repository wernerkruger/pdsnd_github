# Bikeshare Data Analysis

## Date Created
21 December 2025

### Date last updated : 25 December 2025

### Project author : L.W Kruger, Duizel, The Netherlands

## Project Title
Explore US Bikeshare Data

## Description
This project is an interactive Python program that analyzes bikeshare data from three major US cities: Chicago, New York City, and Washington. The program provides comprehensive statistics about bikeshare usage patterns, including:

- **Time Statistics**: Most common month, day of week, and start hour for trips
- **Station Statistics**: Most popular start and end stations, and most frequent trip combinations
- **Trip Duration Statistics**: Total and average trip durations
- **User Statistics**: User type counts, gender distribution, and birth year information

The program allows users to filter data by city, month, and day of week to explore specific patterns in bikeshare usage.

## Features
- Interactive command-line interface for data exploration
- Filter data by city (Chicago, New York City, Washington)
- Filter data by month (January through June, or all months)
- Filter data by day of week (Monday through Sunday, or all days)
- Comprehensive statistical analysis of bikeshare usage
- Performance timing for each statistical calculation
- Option to restart and explore different data filters

## Files Used
- `bikeshare_starter.py` - Main Python script containing all analysis functions
- `new_york_city.csv` - Bikeshare data for New York City
- `chicago.csv` - Bikeshare data for Chicago (referenced in code)
- `washington.csv` - Bikeshare data for Washington (referenced in code)

## Data Structure
The CSV files contain the following columns:
- **Start Time**: Date and time when the trip started
- **End Time**: Date and time when the trip ended
- **Trip Duration**: Duration of the trip in seconds
- **Start Station**: Name of the station where the trip started
- **End Station**: Name of the station where the trip ended
- **User Type**: Type of user (Subscriber or Customer)
- **Gender**: Gender of the user (available for Chicago and New York City)
- **Birth Year**: Birth year of the user (available for Chicago and New York City)

## Requirements
- Python 3.x
- pandas
- numpy

## Installation
1. Clone this repository to your local machine
2. Ensure you have Python 3.x installed
3. Install required dependencies:
   ```bash
   pip install pandas numpy
   ```

## Usage
Run the program from the command line:
```bash
python bikeshare_starter.py
```

The program will prompt you to:
1. Select a city (chicago, new york city, or washington)
2. Select a month to filter by (all, january, february, march, april, may, or june)
3. Select a day of week to filter by (all, monday, tuesday, wednesday, thursday, friday, saturday, or sunday)

After making your selections, the program will display:
- Time statistics (most common month, day, and hour)
- Station statistics (most popular stations and trips)
- Trip duration statistics (total and average duration)
- User statistics (user types, gender, birth years)

You can then choose to restart and explore different filters or exit the program.

## Functions

### `get_filters()`
Prompts the user to specify a city, month, and day to analyze. Includes input validation to ensure valid selections.

### `load_data(city, month, day)`
Loads the data file for the specified city and filters by month and day if applicable. Returns a pandas DataFrame with the filtered data.

### `time_stats(df)`
Displays statistics on the most frequent times of travel, including:
- Most common month
- Most common day of week
- Most common start hour

### `station_stats(df)`
Displays statistics on the most popular stations and trips, including:
- Most commonly used start station
- Most commonly used end station
- Most frequent combination of start and end stations

### `trip_duration_stats(df)`
Displays statistics on trip durations, including:
- Total travel time (in hours, minutes, and seconds)
- Mean travel time (in minutes and seconds)

### `user_stats(df)`
Displays statistics on bikeshare users, including:
- Counts of user types
- Counts of gender (if available)
- Earliest, most recent, and most common year of birth (if available)

## Credits
This project was created as part of the Udacity Programming for Data Science with Python Nanodegree program. The bikeshare data is provided by Motivate, a bikeshare system provider for many major cities in the United States.

## License
This project is for educational purposes as part of the Udacity Nanodegree program.
