# US Bikeshare Data Explorer

This project contains a starter command-line Python program for exploring US bikeshare data. The main script, `bikeshare_starter.py`, is designed to prompt the user for a city, month, and day filter, load the matching dataset with pandas, and then display summary statistics about travel times, stations, trip duration, and users.

At the moment, this repository reflects the starter version of the project. The structure of the program is in place, but several functions still contain TODO sections where the data filtering and statistics logic need to be implemented.

## Project files

- `bikeshare_starter.py`: starter script for the bikeshare analysis workflow
- `new_york_city.csv`: one of the bikeshare datasets referenced by the script

The script is written to work with these CSV files:

- `chicago.csv`
- `new_york_city.csv`
- `washington.csv`

Only `new_york_city.csv` is currently present in this repository, so you will need to add the other data files if you want to run the full city-selection flow without errors.

## Requirements

- Python 3
- pandas
- numpy

Install the dependencies with:

```bash
pip install pandas numpy
```

## How to run the project

From the project directory, run:

```bash
python bikeshare_starter.py
```

The intended program flow is:

1. Prompt the user to choose a city: `chicago`, `new york city`, or `washington`.
2. Prompt for a month filter: `all`, `january`, `february`, `march`, `april`, `may`, or `june`.
3. Prompt for a day-of-week filter: `all`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday`.
4. Load the matching CSV data into a pandas DataFrame.
5. Display summary statistics.
6. Ask whether the user wants to restart the analysis.

## Current implementation status

The following functions are scaffolded in the starter file and still need implementation:

- `get_filters()`
- `load_data(city, month, day)`
- `time_stats(df)`
- `station_stats(df)`
- `trip_duration_stats(df)`
- `user_stats(df)`

Because these sections are not yet completed, the script is not ready for full end-to-end use in its current form.

## Troubleshooting

- If you see `ModuleNotFoundError`, install the required packages with `pip install pandas numpy`.
- If you see `FileNotFoundError`, make sure the expected CSV files are available in the same directory as the script.
- If the program raises a `NameError` for variables such as `city`, `month`, `day`, or `df`, that is a sign the TODO sections in the starter code have not been implemented yet.

## Contribution guidelines

Contributions are best focused on completing the starter functions, validating input handling, and improving the README once the analysis logic is finished. Keep changes small and test the script from the command line after updating the implementation.

## Credits

This project is based on the Udacity starter repository for the Post Your Work project:

[Udacity post-your-work-project](https://github.com/udacity/post-your-work-project)

## Date created

22 April 2026