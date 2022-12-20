# Final Project

## Background

For my final project, I chose to highlight newly-released police misconduct data using a combination of D3 and reveal.js. In 2020, then-governor Andrew Cuomo repealed law 50-A, which sealed records of NYPD misconduct reports. The Legal Aid Society took action and requested, collected, and cleaned the data in order to present the information to the public. The data can be found at [Legalaidnyc.com](https://legalaidnyc.org/law-enforcement-look-up/). 

## Viewing the Piece

To view this piece, it is best to ensure all packages are installed. To do so, first clone this repository to your local machine. Next, navigate to the folder in a command line window and run the node server using the command 

```shell
npm start
```



### Cleaning Data

For this assignment, rather than using tools to create links, I ended up creating the dataset mostly from scratch. The dataset on OpenSecrets is in xlxs format, so I first converted it to a CSV and cleaned up column names and other anomalies in order to prepare the data for visualization. To create links between each node (recipient), I created a CSV that contains each node's index and links them to other recipients within the same political party. Once I was able to do so, I went ahead and started to code out my viz. 

### D3 Code

To create my visualization, I first set all of my CSS stylings, which included font sheets as well as settings for my tooltip. Once done, I loaded in my data from the CSVs I created using the class material as reference. I used the total amount of donations that a candidate received for their campaign as the radius for each node to highlight the difference in funding compared to others. This was a challenge, as the dollar amounts were incredibly high, so the radius calculation required a bit of scaling to get the sizes under control. Additionally, I was having issues with the clusters colliding and sending each other off of my page——to rectify this, I converted each candidate's party to a categorical number, which allowed me to center each party using a separate x-value. Once I was happy with the positioning of my graph, I added a few transitions and included relevant information in my tooltip.

Formatting my visualization in a way that appeared smooth, organized, and informative proved to be quite a challenge for this assignment. However, the end result was something I was proud to have accomplished.

### Final Visualization

The final visualization is rather simple, but effective in its goal. Each candidate is represented by a bubble that varies in size based on the amount of individual police contributions they received. Each candidate's party is also reflected by the color pallette I chose, which I've selected due to their party association. See the interactive viz below:

![Final Viz](/Week_10_HW/vizgif.gif/ "Final Visualization")


