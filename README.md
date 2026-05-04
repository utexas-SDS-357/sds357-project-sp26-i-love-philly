# Passion or Public Disorder: Exploring Philadelpha Police Stop Data in Relation to Major Sporting Events in the City
*Medhavi Jambhekar, Vijetha Ramdas, Charlotte Suarez, Jasmine Xu, Alejandro Zamudio*

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MFzEnxem)


## File Structure

<pre> ```
├── EDA
│   ├── AdditionalEDA.ipynb: this Notebook contains exploration and visualizations of Arrests, Searches, 
                Frisks and additional information from the Policing Data bsed on game type (Home Games, 
                Away games, Any Event, No Games).
│   ├── PhillyEDA.Rmd: This file contains R code for basic initial
│   ├── PhillyEDA.pdf: Graphs for Philly dataset
│   ├── README.md
│   ├── eagles.ipynb: Data Wrangling of our Eagles dataset
│   ├── eagles_square_visualization.ipynb: More graphs
│   ├── eda_all_teams.ipynb: EDA on all the teams data
│   ├── gameday_outcome_analysis.ipynb: Analysis of traffic patterns for all sports across W/L outcomes.
│   └── gameday_vs_nongameday_analysis.ipynb: Analysis of traffic and arrest counts and distributions on gamedays and non-gamedays. Plots from this notebook are in our report.
├── README.md
├── archive
│   ├── README.md
│   ├── SOPPwithSports.ipynb
│   ├── eagles_circle_model.ipynb
│   ├── eagles_data_wrangling_circles.ipynb
│   ├── linReg_eagles.ipynb
│   ├── maps
│   │   ├── README.md
│   │   ├── all_stops.html
│   │   ├── eagles_gameday_ped_stop_density.html
│   │   ├── eagles_gameday_ped_stop_w5_density.html
│   │   ├── eagles_gameday_stop_density.html
│   │   ├── eagles_gameday_stops_w5_density.html
│   │   ├── eagles_nongameday_SAMPLED_stop_density.html
│   │   └── eagles_nongameday_stop_density.html
│   ├── prelim.ipynb
│   └── test_merging_data_eagles.ipynb
├── data_cleaning_and_wrangling
│   ├── CleaningScript.ipynb
│   ├── DATA_FILTER.ipynb
│   ├── README.md
│   ├── data_cleanse.ipynb
│   ├── eagles_data_wrangling.ipynb
│   ├── flyers_data_wrangling.ipynb
│   ├── location_mapping.ipynb
│   ├── phillies_data_wrangling.ipynb
│   └── philly76_data_wrangling.ipynb
├── datasets
│   ├── README.md
│   ├── input
│   │   ├── Eagles Schedule & Scores - Eagles.csv
│   │   ├── Flyers.csv
│   │   ├── Phillies_Schedule_Updated_2.csv
│   │   ├── Philly76.csv
│   │   └── Venue Locations.csv
│   └── output
│       ├── cleaned76ersData.csv
│       ├── cleanedEaglesData.csv
│       ├── cleanedFlyersData.csv
│       └── cleanedPhilliesData.csv
└── modeling
    ├── README.md
    ├── eagles_square_model.ipynb
    ├── flyers_modeling.ipynb
    ├── phillies_modeling.ipynb
    └── philly76_modeling.ipynb

``` </pre>

## Motivation
The city of Philadelpha has earned a notorious reputation in the sports world due to the actions of its fans. As a result, the media often uses words such as "passionate" and "destructive" when referring to the sports culture that has arisen in Philadelphia. An expectation has been set, and reinforced time and time again, that "win or lose, Philly burns."

Despite the prominence of this stereotype, it remains unclear whether such portrayals reflect measurable changes in real-world behaviour.  The extent to which major sporting events influence Philadelphia’s law enforcement activity (such as traffic stops or pedestrian stops) is an area of interest. Given the intensity with which sporting events are portrayed, understanding whether major sporting events shape policing patterns and the frequency of vehicle or pedestrian stops made on these particular days is both socially and analytically significant.

## Objectives
This project aims to investigate whether the “Philly will burn” stereotype is supported by empirical evidence, specifically found within police stop data. Our study is guided by three primary objectives:

1. **Comparison of Stop Patterns**
   
   Examine how traffic and pedestrian stop patterns differ between game days and non-game days across major league sports in Philadelphia. This will include analyzing stop frequency, arrest rates, and other stop outcomes, as well as observing variation across sports and proximity to stadium locations.

2. **Predictive Modeling of Game Day Outcomes** 
   
   Determine whether game-related characteristics can predict traffic stops or arrest rates by analyzing the extent to which score differential, the opponent played, or game significance affect the nature of stops performed on a game day. For example, is it reasonable to predict that sports fans will be more animated when their team is playing their biggest rival, such as when the Eagles play the Dallas Cowboys? This study aims to identify how these characteristics influence predictions of traffic stop outcomes. 


Ultimately, this project seeks to assess whether widely held perceptions of Philadelphia sports culture are grounded in real data or driven primarily by anecdotal evidence.


## Assumptions and Limitations

- Stadium-specific security data is not available
- External factors (weather, holidays, concurrent events) are not accounted for in the data
