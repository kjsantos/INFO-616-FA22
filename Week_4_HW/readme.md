# Homework Assignment #3

This repository contains the necessary material for the third homework assignment in INFO-616. For this week, we were practicing drawing shapes using D3 using path and other various methods. Once I created a drawing, I then used it to visualize data using a CSV that I loaded into D3, using the appropriate attributes to style my finished product. The result can be seen below.

## Understanding the Data

The data used for this project was taken from the National Interagency Fire Center. NIFC's website offers a simple dataset containing the number of wildfires and the amount of acres they burned for each year. The reporting is taken from federal wildland fire agencies and dates back to 1983. For my purposes, I was curious about the past 20 years, so I scraped only the relevant data and saved it to a TSV for further cleaning. To see the full dataset, follow the link ![here](https://www.nifc.gov/fire-information/statistics/wildfires).

## Coding the Visualization

### Cleaning Data

As a best practice, I typically use OpenRefine to clean any data before use in a visualization. Due the simplicity of my data for this exercise, I only had to make a few alterations, such as converting data types and removing commas from numbers. Once these steps were fulfilled, I exported the dataset to a CSV titled YearFireAcres.csv, which you can find in this repo.

### D3 Code



### Final Visualization

Once rendered, I was able to fit my entire visualization on one page depicting the frequency of churchgoers in each state. While difficult, I found that making small adjustments as I went along resulted in a much cleaner final product. 

![Final Bar Chart](/Week_3_HW/Final_viz.png "Final Visualization")

## Some Notes

Although I was happy with my bar chart, there are certainly a few things I would love to explore using this data in the future, given more practice and experience with D3:

- The data also includes other frequencies for service attendance, such as once a month/a few times a year or never. It would be interesting to attempt a stacked bar chart that shows the distribution in each state.
- If possible, it would be interesting to filter the data so that only the top 10 states with the highest frequencies are displayed. This may be useful when creating multiple visualizations to compare side-by-side
- I would also like to explore more style elements, such as implementing something like Bootstrap for consistency across the board.
- Once we start working with multi-dimensional data, it would be interesting to explore what manipulations I could make to this data, as well as comparing other data points such as census data to the data in this survey.


