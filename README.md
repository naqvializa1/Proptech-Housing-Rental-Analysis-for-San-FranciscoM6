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


This program analyzes and presents real estate data with one click. Just with one click, you can analyse rent and price per square foot trends in each neighborhood. The source of infomration has neighborhood historical data, in additon to a separae source of information for longitude and latitude. This information is then used to view geospatial data. The points of interest are then drawn on top of this geo view using hvplot libraries and functions.The graphs are interactive with zooming, panning, and selecting features.

Technologies

This project is written in python. The required libraries are as follows pathlib ver 2.3.6, pandas, hvplots.pandas

Usage

This project sources historical data and geospatial data to graph historical trends about average price per square foot and gross rent in different neighborhoods of San Francisco.The app uses hvplots to plot this interactive data.

Analysis Report

Based on the visualization above, there is uptrend in number of housing units from 2010 to 2018. Based on visualization, there is a drop in the average sale price per square foot in 2011 as compared to 2010. Clearly, the gross rent still went up from 2010 to 2011. There has been no year with drop of gross rent in the observed period from 2010 to 2016.

Overall, the rent and sales price per square foot has uptrend. With the exception of 2011, average sale price per square foot has risen and so have average rents. However, the story is not consistent when viewed each neighborhood on it's own. For e.g. Golden Gate heights saw a big drop in sales per square foot from 2013 to 2014. Glen Park price per square foot had dipped for multiple years since 2010, but it has been trending up for last few years. Alamo neighborhood price per square foot has dipped in 2016

However, the rent trend is up across all the neighborhoods.

Overall, the rents have been on the uptrend. However, there are certain neighborhoods, where the rent has not trended up in the same ratio as the price per square foot. This indicates, there is potential for higher rental income. Union Square and Corona Heights are examples for rental investments.

In few other neighborhoods, rent has gone up more in proportion than the price per square foot. Hence these areas may be good for buying opportunities.

If someone needs to move money by selling and buying in another neigborhood, then I would recommend selling in Marina, Alamo or Hayes Valley neighborhood, while buying in Glen Park as the trends have shown divergence.
Dropdown Menu                         |  Selecting a Neighborhood
:------------------------------------:|:------------------------:
![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/dropdown.PNG)                      |  ![Alt text](https://github.com/antonmaliksi/FinTechModule6Challenge/blob/main/Housing%20Analysis%20San%20Fransisco/Readme%20Resources/dropdown_select.PNG)
