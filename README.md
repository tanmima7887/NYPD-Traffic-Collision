# NYC Accident Analysis and Visualization

## Overview

This project aims to analyze and visualize traffic accidents in New York City (NYC) using Python. The data includes information on the number of persons injured or killed, contributing factors to the accidents, and the locations of the accidents. The visualization includes plotting accidents by the hour of the day, the day of the week, and an interactive map showing the locations of accidents, and more features will be add on to it.

## Features

- **Data Cleaning**: Handling missing values and ensuring correct data types.
- **Data Analysis**: Extracting useful insights such as the hour of the day and the day of the week when accidents occur.
- **Data Visualization**: Creating plots to visualize accidents by hour and by day, and an interactive map to show accident locations.
- **Interactive Map**: Using Folium and MarkerCluster to create an interactive map that displays accident locations with markers indicating contributing factors.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/tanmima7887/NYPD-Traffic-Collision.git
    cd NYPD-Traffic-Collision
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. **Data Preparation**:
    - Place your dataset (CSV file) in the project directory.
    - Ensure the dataset has the following columns:
        - `CRASH DATE`
        - `CRASH TIME`
        - `BOROUGH`
        - `ZIP CODE`
        - `LATITUDE`
        - `LONGITUDE`
        - `LOCATION`
        - `ON STREET NAME`
        - `CROSS STREET NAME`
        - `OFF STREET NAME`
        - `NUMBER OF PERSONS INJURED`
        - `NUMBER OF PERSONS KILLED`
        - `NUMBER OF PEDESTRIANS INJURED`
        - `NUMBER OF PEDESTRIANS KILLED`
        - `NUMBER OF CYCLIST INJURED`
        - `NUMBER OF CYCLIST KILLED`
        - `NUMBER OF MOTORIST INJURED`
        - `NUMBER OF MOTORIST KILLED`
        - `CONTRIBUTING FACTOR VEHICLE 1`
        - `CONTRIBUTING FACTOR VEHICLE 2`
        - `CONTRIBUTING FACTOR VEHICLE 3`
        - `CONTRIBUTING FACTOR VEHICLE 4`
        - `CONTRIBUTING FACTOR VEHICLE 5`
        - `COLLISION_ID`
        - `VEHICLE TYPE CODE 1`
        - `VEHICLE TYPE CODE 2`
        - `VEHICLE TYPE CODE 3`
        - `VEHICLE TYPE CODE 4`
        - `VEHICLE TYPE CODE 5`

2. **Run the Analysis**:
    - Use the provided Jupyter Notebook or Python script to perform data cleaning, analysis, and visualization.
    - Example:
        ```python
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns
        import folium
        from folium.plugins import MarkerCluster
        from IPython.display import IFrame

        # Load dataset
        df = pd.read_csv('NYPD.csv')

        ```

3. **Generate the Interactive Map**:
    - Run the script to generate the interactive map and save it as an HTML file.
    - Display the map in a Jupyter notebook:
        ```python
        accident_map.save('interactive_accident_map.html')
        IFrame(src='interactive_accident_map.html', width=700, height=600)
        ```

## Examples

### All Accident
![Accidents by Hour of Day](images/accident_map_without_hour.html)

### Interactive Accident Map
![Accidents by Day of Week](images/interactive_accident_map.html)

### Top Accident Map
![Interactive Accident Map](images/top_accident_locations_map.html)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

## Acknowledgements

- NYC Open Data for providing the dataset [LINK](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95/data).
- [Folium](https://github.com/python-visualization/folium) for the interactive map visualization.
- [Seaborn](https://seaborn.pydata.org/) and [Matplotlib](https://matplotlib.org/) for data visualization.

## Contact

For any inquiries, please contact [Tanmim Ahmmed](mailto:tanmimahmmed@gmail.com).
