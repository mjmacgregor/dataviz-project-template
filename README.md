# Data Visualization Project

## Data

The data I propose to visualize for my project comes from the [Consumer Behavior and Shopping Habits Dataset](https://www.kaggle.com/datasets/zeesolver/consumer-behavior-and-shopping-habits-dataset/data).

This data set describes a variety of demographic and logistic information related to consumer purchases throughout the United States. One instance of data includes information regarding who the consumer is, what they purchased, when they purchased it, where they purchased it, and how they purchased it. An example row of data can be seen below:

![Example Row](https://github.com/mjmacgregor/dataviz-project-template/blob/master/shopping-data.png)


## Questions & Tasks

The purpose of this project is to provide visualizations that would assist in driving data-based decision-making for the company. The following tasks and questions will drive the visualization and interaction decisions for this project:

 * Which states / regions have the best ratings and get the most purchases?
 * Which products are most popular by gender, season, and region?
 * Are different demographics more likely to be regular customers?
 * Which demographics and products provide the most sales in different states and overall?

## Sketches

The following is a first draft sketch of what the final dashboard could look like with several relevant visualizations:

![Sketch](https://github.com/mjmacgregor/dataviz-project-template/blob/master/shopping-dashboard-sketch.jpg)

These are the visualizations that were included in the sketch:

1. **Scatterplot** - A scatterplot where the data is organized by *state*. The horizontal position corresponds to the total number of purchases in the state while the vertical position corresponds to the average rating given by the customer in the state. Circles can also be colored by the season that has the most purchases in the state.
2. **Chloropleth** - A chloropleth map of US states where the states are colored by gender, by most popular season, by average rating, etc. with interactive property that the user can decide which metric to color the map by.
3. **Pie Chart** - Pie chart distributions of the products purchased in each season. There will be buttons representing each season so that the user can easily toggle which season the pie chart displays. The color of each section in the pie chart will correspond to the most popular color of the product.
4. **Bar Chart** - A stacked bar chart distribution of total sales. There are options for which metrics can be used, but one example is a bar chart of total sales by season by gender.
5. **Histogram** - A histogram distribution of total sales or just purchases by demographic. One interesting metric to display would be total sales by age.

These are first draft ideas, but all help answer questions of sales or purchases by demographic information. These are the questions that the company would look to answer to drive decisions.

## Prototypes

First draft prototype of a chloropleth map of the customer ratings for the US states:
![Sketch](https://github.com/mjmacgregor/dataviz-project-template/blob/master/chloropleth_us_state_ratings.png)

The size of the circles correspond to the number of purchases in a state, and the color corresponds to the average customer rating. A darker shade of blue indicates a higher average rating.

## Open Questions

There are several challenges that I know I will face throughout this process:

1. Learning and understanding aggregations
   - I anticipate that all of my visualizations will be based on aggregated values rather than individual data points (ex: total purchases of product x in season y). Because this is my first project in Java Script and D3, I am not very familiar with how these are coded in the language and into visualizations. There will be a learning curve with implementing these into my visualizations.
2. Implementing interactivity
   - Similar to above, I don't have experience with introducing interactivity into visualizations, so I am expecting a learning curve here as well. There are two main interactive elements I am expecting: clicking on different metrics to generate the respective visualizations, and hovering data points to display more complete information.
3. Developing new visualization types
   - I expect that some of the visualization types will be a lot more complex than others to implement. For example, I am most concerned about the chloropleth map. I believe the scatterplot and bar chart will be the least complicated to implement, but as of right now I do not know how to implement a chloropleth map. I'm expecting another learning curve with learning how to implement all of the different visualization types.

## Milestones

These are the milestones I am expecting for my project:

1. Researching and understanding aggregations in JS / D3 and implementing them into visualizations
2. Develop first draft prototypes for the least complex visualizations (i.e. scatter plot, bar chart)
3. Learn more about the more complicated visualization types (i.e. chloropleth, pie chart)
4. Develop first draft prototypes for the remaining visualizations
5. Introduce interactivity into the visualizations that allow for hovering data points to show more complete information
6. Introduce interactivity into the dashboard to allow the user to display the visualizations based on metrics of choice
7. Finalize dashboard design
8. Culminate findings and process into a final report

## Progress

### Week 1

The majority of the work I did this week was preparing the data for visualizations. I performed aggregations and joins on the data in Python to prepare several tables to go into visualizations. For example, for my chloropleth chart, I grouped the data by state and calculated the average and total number of customer ratings for each state.

I then started creating prototypes for visualization. The first big prototype I created was the map of US states and customer ratings.
My next steps are to create prototypes of the scatterplot and bar chart visualizations.

I also want to learn more and incorporate hovering and interaction into my chloropleth as well as adjust some of the design choices, but the prototype works well! The prototype can be found in the prototype section.
