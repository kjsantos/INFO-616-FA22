# Homework Assignment #5

This repository contains the necessary material for the third homework assignment in INFO-616. For this week, We were challenged to create a visualization that uses interaction to improve the information presented. This visualization uses methods explained in class combined to encourage interacting with the svg elements.

## Understanding the Data

For this assignment, I chose to improve a previous visualization using interactivity. The data is taken from federal wildland fire agencies and dates back to 1983. For my purposes, I was curious about the past 20 years, so I scraped only the relevant data and saved it to a TSV for further cleaning. To see the full dataset, follow the link [here](https://www.nifc.gov/fire-information/statistics/wildfires).

## Coding the Visualization

### Cleaning Data

Because I had previously cleaned my data using OpenRefine, there was little cleaning to do before adding interactivity. The one thing I changed was sorting in ascending order. Initially, my visualization showed the most recent years at the beginning of my SVG; this conflicted with the slider that I intended on adding, so this change helped make my visualization more intuitive.

### D3 Code

My original visualization was quite busy with multiple labels, so my first thought was to remove one and add it to a tooltip to encourage users to seek more information. Additionally, I wanted to make my visualization feel less static, so I added code to both remove any paths that were generated from years past the current slider year. This proved to be quite challenging, but the final product was satisfying to explore.

### Final Visualization

![Final Bar Chart](/Week_8_HW/visgif.gif/ "Final Visualization")


