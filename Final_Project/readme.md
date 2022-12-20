# Final Project

## Background

For my final project, I chose to highlight newly-released police misconduct data using a combination of D3 and reveal.js. In 2020, then-governor Andrew Cuomo repealed law 50-A, which sealed records of NYPD misconduct reports. The Legal Aid Society took action and requested, collected, and cleaned the data in order to present the information to the public. The data can be found at [Legalaidnyc.com](https://legalaidnyc.org/law-enforcement-look-up/). 

## Viewing the Piece

To view this piece, it is best to ensure all packages are installed. To do so, first clone this repository to your local machine. Next, navigate to the folder in a command line window and run the node server using the command 

```shell
npm start
```

Once the server has started, you can open a browser and navigate the the local host address provided in your shell. From there, simply open final.html and click through the pages to explore.


### Cleaning Data

Luckily, a majority of my data was clean prior to the analysis step. However, because of the size of data, I had to create more scalable datasets to work with. Starting with the CCRB dataset, I created a running total dataset from 1999-2022 using pivot tables in Microsoft Excel. I then used OpenRefine to further clean my data and remove any unnecessary values.

I also had to hard code some data into one of my visualizations—the data used in the fiscal budget slide was taken from an official state budget report from 2020.

### D3 Code

Organizing my project in a way that utilizes several visualizations proved to be a challenge, but I think my efforts were mostly successful. Because I wanted to build a narrative from my data, I needed to create several visualizations using D3. These graphs can be found in the figs file within the repository. Using reveal.js, I was able to embed my individual html files in each slide without having to compropmise on style or animation. The most difficult part of this process turned out to be arranging my graphs in a way that felt seamless, but using the methods learned in class, I was able to make it work.

### Final Thoughts

Overall, I enjoyed working on a project that I was invested in background research for. Because the data I worked with is so vast, however, I found it difficult to hone in on which visualizations would be worth my time including for this project. I chose to focus on the process of CCRB complaints because I figured the details were nuanced enough that they deserved to be highlighted. However, this narrowed the scope of the other visualizations I had planned to create for this project, as they simply did not fit properly with the narrative. However, I am proud of what I was able to accomplish given the scope of my data.

I plan to continue working on this project, as it feels as though some more visuals would help to propel the narrative I've begun to construct. One visualization I still plan on incorporating would be a bubble chart of NYPD officers' pay. When attempting to code this visualization specifically, I realized there were far too many records to include, so in the future, I will need to figure out a way to scale down the data while still making the information appear pertinent.

