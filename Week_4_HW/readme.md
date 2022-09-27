# Homework Assignment #3

This repository contains the necessary material for the third homework assignment in INFO-616. For this week, we were practicing drawing shapes using D3 using path and other various methods. Once I created a drawing, I then used it to visualize data using a CSV that I loaded into D3, using the appropriate attributes to style my finished product. The result can be seen below.

## Understanding the Data

The data used for this project was taken from the National Interagency Fire Center. NIFC's website offers a simple dataset containing the number of wildfires and the amount of acres they burned for each year. The reporting is taken from federal wildland fire agencies and dates back to 1983. For my purposes, I was curious about the past 20 years, so I scraped only the relevant data and saved it to a TSV for further cleaning. To see the full dataset, follow the link [here](https://www.nifc.gov/fire-information/statistics/wildfires).

## Coding the Visualization

### Cleaning Data

As a best practice, I typically use OpenRefine to clean any data before use in a visualization. Due the simplicity of my data for this exercise, I only had to make a few alterations, such as converting data types and removing commas from numbers. Once these steps were fulfilled, I exported the dataset to a CSV titled YearFireAcres.csv, which you can find in this repo.

### D3 Code

Before even thinking about my visualization, I first wanted to experiment with using paths to draw SVG shapes. Editing my path in real time, I was able to draw up an icon resembling a fireball using a variety of curves and control points. In order to give the appearance of natural fire, I tried to avoid consistency in the distance between points and their curve points. Once I was happy with my shape, I loaded in my data and created groups from each data point. For each individual row, I used all 3 categories to visualize the information--the volume of fires alters the shade of the icon, the year is displayed as a label, and the acres burned appears as a label as well. As a fun experiment, I wanted to alter the shade of the acres label to signify a higher amount of acres burned. To do this, I created a second color scheme, this time using my acres column for my max and min values. The result is a 3-step gradient that colors the text darker when the numbers are higher. 

### Final Visualization

Once I was happy with the general concept of my visualization, I began making minor adjustments as I cleaned up my finished product. After adjusting some coordinate placements for labels and titles, my work was finished. Overall, I was happy with the design and am excited to employ these methods when creating visualizations in the future.

![Final Bar Chart](/Week_4_HW/FireViz.png/ "Final Visualization")

## Final Thoughts

This exercise was both challenging and fulfilling at the same time. I very much enjoyed experimenting with shapes, as it helped me to better understand paths as a concept. I think this is a valuable concept to learn for future visualizations as well as certain web design projects. I would love to experiment further with this concept to attempt some more detailed drawings with multiple shapes layered together.


