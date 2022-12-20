# Homework Assignment #7

## Background

This repository contains the necessary material for the fourth homework assignment in INFO-616. For this week, we were to experiment with layouts when designing visualizations. For my assignment, I paid special attention to creating linked network graphs to display campaign donation data collected by [OpenSecrets.org](https://docs.google.com/spreadsheets/d/1gJBJyd_Imn-kcNQbH08e5yjvPoLgxR-w4qKd_6hUGcM/edit?usp=sharing). This data includes individual donations made by law enforcement to presidential candidates and political action committees for the 2020 election cycle. 

## Coding the Visualization

### Cleaning Data

For this assignment, rather than using tools to create links, I ended up creating the dataset mostly from scratch. The dataset on OpenSecrets is in xlxs format, so I first converted it to a CSV and cleaned up column names and other anomalies in order to prepare the data for visualization. To create links between each node (recipient), I created a CSV that contains each node's index and links them to other recipients within the same political party. Once I was able to do so, I went ahead and started to code out my viz. 

### D3 Code

To create my visualization, I first set all of my CSS stylings, which included font sheets as well as settings for my tooltip. Once done, I loaded in my data from the CSVs I created using the class material as reference. I used the total amount of donations that a candidate received for their campaign as the radius for each node to highlight the difference in funding compared to others. This was a challenge, as the dollar amounts were incredibly high, so the radius calculation required a bit of scaling to get the sizes under control. Additionally, I was having issues with the clusters colliding and sending each other off of my page——to rectify this, I converted each candidate's party to a categorical number, which allowed me to center each party using a separate x-value. Once I was happy with the positioning of my graph, I added a few transitions and included relevant information in my tooltip.

Formatting my visualization in a way that appeared smooth, organized, and informative proved to be quite a challenge for this assignment. However, the end result was something I was proud to have accomplished.

### Final Visualization

The final visualization is rather simple, but effective in its goal. Each candidate is represented by a bubble that varies in size based on the amount of individual police contributions they received. Each candidate's party is also reflected by the color pallette I chose, which I've selected due to their party association. See the interactive viz below:

![Final Viz](/Week_10_HW/vizgif.gif/ "Final Visualization")


