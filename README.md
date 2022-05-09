# Proptech Real Estate Analysis for San Fransisco

To the board of Proptech, I offer an instant, one-click service for people to buy properties and rent them. <br> Using historical data from 2010-2016, I have created an all-in-one service to find properties in the <br> San Fransisco market that are viable investment opportunities.

This service includes:
1. Data Visualization
2. Data Aggregation
3. Interactive Visualizations
4. Geospatial Analysis

---

## Technologies

This service utilizes Python 3 and the following libraries:
1. Pandas
2. HVPlot
3. Pathlib

---

## User Guide

To begin using the notebook in Jupyter Labs:

### Part 1
1. Open "san_fransisco_housing.ipynb"
2. Look for the following:
    ```python
    sfo_data_df = pd.read_csv(Path("Resources/sfo_neighborhoods_census_data.csv"))
    ```
Please ensure that you have the correct .csv file imported from the Resources folder located within the parent folder.
3. Run each code cell to retrieve your data.

### Part 2
1. Look for the following:
    ```python
    prices_by_year_by_neighborhood.hvplot(
    x="year",
    xlabel="Year",
    ylabel="Rent / PSFT Amount",
    groupby="neighborhood"
    )
    ```
The line plot that this produces will showcase a dropdown menu to the right of the plot. <br> Use this dropdown menu to view data for each neighborhood.

### Part 3
1. Look for the following:
    ```python
    neighborhood_locations_df = pd.read_csv(
    Path("Resources/neighborhoods_coordinates.csv"),
    index_col="Neighborhood"
    )
    ```
Please ensure that you have the correct .csv file imported from the Resources folder located within the parent folder.

---

## Documentation
Please reference the following screenshots for guidance with any changes within the code:

San Fransisco                         |  Los Angeles
:------------------------------------:|:------------------------:
![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/san_fransisco.PNG)                      |  ![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/los_angeles.PNG)

Dropdown Menu                         |  Selecting a Neighborhood
:------------------------------------:|:------------------------:
![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/dropdown.PNG)                      |  ![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/dropdown_select.PNG)

---

## Contributors
Coding and data analysis was completed by Junior Analyst Anton Maliksi from Proptech.

---

## License
No licenses were used for this application.
