# Homework Assignment #4

This repository contains the necessary material for the fourth homework assignment in INFO-616. This week's assignment was to consider color and accessibility when designing a visualization.

## Understanding the Data

For this assignment, I explored greenhouse gas emission data from the World Resources Institute. The dataset I used was rather comprehensive, so I decided to focus on just the total amount of all types of emissions per year. To narrow down my scope more, I also took the most recent ten years in the dataset to compare trends. To see the full dataset, follow the link [here](https://datasets.wri.org/dataset/climate-watch-states-greenhouse-gas-emissions).

## Coding the Visualization

### Cleaning Data

To get my data in a format that I could easily work with, I first used Excel to create a pivot table and sum my values for each state per year and round my values to 2 decimal places. Once that was done, I made sure to run it through OpenRefine to make sure my data values were the correct type. once I had a nicely condensed dataset, I was then ready to plug my data into D3.

### D3 Code

To put my visualization together, I first designed a path drawing to create a smokestack-like image that goes along with the theme of my visualization. Then I used [Coolors.co](https://coolors.co/) to design a color palette that achieves the same effect as well as accounts for color deficiency. Additinally, I made sure to include Alt text and descriptions in order to give credit to the data source and allow for aria-labelledby to interpret my viz. Putting these steps together, along with material from previous weeks, I was able to build my final visualization.

### Final Visualization

The final product is a simple depiction of total greenhouse gas emissions with the deeper colors denoting higher levels of emissions. I feel this exercise was incredibly important to make sure information is accessible to as much of the population as possible.

![Final Bar Chart](/Week_5_HW/GHG_Viz.png/ "Final Visualization")


