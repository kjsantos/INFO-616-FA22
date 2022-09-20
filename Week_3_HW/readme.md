# Homework Assignment #2

This repository contains the necessary material for the second homework assignment in INFO-616. To complete my objective, I was to create a simple visualization (bar chart, scatterplot, etc.) using a dataset of my choice. The resulting visualization can be found within this repo as well as toward the end of this Readme.

## Understanding the Data

The data used for this assignment comes from a survey conducted by the Pew Research Center in 2014. The dataset includes results from a questionnaire where respondents were asked to disclose how frequently they attend church services regardless of religious denomination. To control for population density, the research also accounts for sample size, adhering as best to a real-world representation of each state's density. The data is broken up into percentages by state, so I decided to focus on those who stated they attended services at least once a week. A detailed breakdown of the full survey can be found [here](https://www.pewresearch.org/religion/wp-content/uploads/sites/7/2015/11/201.11.03_rls_ii_questionnaire.pdf).

## Coding the Visualization

### Cleaning Data

To extract the data and load it into D3 for visualization, I first had to clean up the data. The portal on Pew Research Center's website did not include a download link, so I took it upon myself to scrape the data. Because there are only 50 states, this task wasn't very difficult, but I used OpenRefine to ensure my data were all in the correct format and ready to be used in D3. The resulting dataset can be found in this repository as devout_religious_survey.csv

### D3 Code

Once cleaned, I used simple D3 functions to map my data by its columns and created an SVG using the templates from out in-class work. To add some style, I also included CSS and experimented with different colors for my bar chart fills. As a challenge, I also added X and Y labels to my data for clarity, as well as a title that appears when hovering over the visualization. While testing different dimensions as I worked through this assignment, I landed on the ones seen in the final product below.

### Final Visualization

Once rendered, I was able to fit my entire visualization on one page depicting the frequency of churchgoers in each state. While difficult, I found that making small adjustments as I went along resulted in a much cleaner final product. ![](/Week_3_HW/Final_viz.png "Final Visualization")

## Some Notes

Although I was happy with my bar chart, there are certainly a few things I would love to explore using this data in the future, given more practice and experience with D3:

- The data also includes other frequencies for service attendance, such as once a month/a few times a year or never. It would be interesting to attempt a stacked bar chart that shows the distribution in each state.
- If possible, it would be interesting to filter the data so that only the top 10 states with the highest frequencies are displayed. This may be useful when creating multiple visualizations to compare side-by-side
- I would also like to explore more style elements, such as implementing something like Bootstrap for consistency across the board.
- Once we start working with multi-dimensional data, it would be interesting to explore what manipulations I could make to this data, as well as comparing other data points such as census data to the data in this survey.


