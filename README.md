# Passion or Public Disorder: Exploring Philadelpha Police Stop Data in Relation to Major Sporting Events in the City
*Medhavi Jambhekar, Vijetha Ramdas, Charlotte Suarez, Jasmine Xu, Alejandro Zamudio*

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MFzEnxem)

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


## File Structure

<pre> ```
├── EDA
│   ├── AdditionalEDA.ipynb: this Notebook contains exploration and visualizations of Arrests, Searches, 
│   │      Frisks and additional information from the Policing Data bsed on game type (Home Games, 
│   │      Away games, Any Event, No Games).
│   ├── PhillyEDA.Rmd: This file contains R code for basic initial data exploration
│   ├── PhillyEDA.pdf: Output from PhillyEDA.Rmd
│   ├── README.md: Describes the contents of the EDA folder
│   ├── eagles.ipynb: Visualizes police stop characteristics and outcomes on Eagles gamedays
│   ├── eagles_square_visualization.ipynb: Creates a spatial heatmap to visualize stop frequency in Philly by 
│   │   square region
│   ├── eda_all_teams.ipynb: EDA on all the sports datasets
│   ├── gameday_outcome_analysis.ipynb: Analysis of traffic patterns for all sports across W/L outcomes.
│   └── gameday_vs_nongameday_analysis.ipynb: Analysis of traffic and arrest counts and distributions on 
                gamedays and non-gamedays. Plots from this notebook are in our report.
├── README.md: The current files detailing the repository structure and project overview
├── archive: This folder contains archived materials. These materials were created in the early stages of the project 
│               and were not used for any final data exploration, wrangling, or modeling. These files are being 
│                stored in case they need to be referenced during code development in the future.
│
│                The file descriptions within the archive folder are not included because they are not active files used 
│                    for our final project results.
├── data_cleaning_and_wrangling
│   ├── CleaningScript.ipynb: This file cleans the raw sport datasets and exports the cleaned data 
│   │   into datasets/output
│   ├── DATA_FILTER.ipynb: Adds an indicator column to the main dataset that indicates whether a game 
│   │       (for given sport) took place at the date of a stop.
│   ├── README.md: Describes the contents of the data_cleaning_and_wrangling folder
│   ├── eagles_data_wrangling.ipynb: Combines the Eagles data with SOPP data and transforms data to prepare for 
│   │       modeling
│   ├── flyers_data_wrangling.ipynb: Combines the Flyers data with SOPP data and transforms data to prepare for 
│   │       modeling
│   ├── location_mapping.ipynb: Determining the distance of each stop from venue locations (miles and km) and 
│   │       producing heatmaps of stops on gamedays and non gamedays
│   ├── phillies_data_wrangling.ipynb: Combines the Phillies data with SOPP data and transforms data to prepare for 
│   │       modeling
│   └── philly76_data_wrangling.ipynb: Combines the 76ers data with SOPP data and transforms data to prepare for 
│   │       modeling
├── datasets
│   ├── README.md: Describes the contents of the datasets folder
│   ├── input: Folder containing raw sport schedule and game outcome data.
│   │   ├── Eagles Schedule & Scores - Eagles.csv: raw Eagles schedule and game outcome data
│   │   ├── Flyers.csv: raw Flyers schedule and game outcome data
│   │   ├── Phillies_Schedule_Updated_2.csv: raw Phillies schedule and game outcome data
│   │   ├── Philly76.csv: raw 76ers schedule and game outcome data
│   │   └── Venue Locations.csv: latitude and longitude coordinates for the Philadelphia sporting venues
│   └── output: Folder containing interim cleaned datasets that were generated by cleaning scripts
│       ├── cleaned76ersData.csv: cleaned 76ers schedule and game outcome data
│       ├── cleanedEaglesData.csv: cleaned Eagles schedule and game outcome data
│       ├── cleanedFlyersData.csv: cleaned Flyers schedule and game outcome data
│       └── cleanedPhilliesData.csv: cleaned Phillies schedule and game outcome data
└── modeling: Folder containing our modeling code referred to in the final report.
    ├── README.md: Describes the contents of the modeling folder
    ├── eagles_modeling.ipynb: All model fitting, selection, and final evaluations for Eagles game day model
    ├── flyers_modeling.ipynb: All model fitting, selection, and final evaluations for Flyers game day model
    ├── phillies_modeling.ipynb: All model fitting, selection, and final evaluations for Phillies game day model
    └── philly76_modeling.ipynb: All model fitting, selection, and final evaluations for 76ers game day model

``` </pre>

## Dependencies

### Python Packages

- pandas
- numpy
- folium
- scikit-learn
- xgboost
- lightgbm
- matplotlib
- seaborn
- shap


### R Packages

- tidyverse

