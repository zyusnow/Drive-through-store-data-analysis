# Drive-through-store-data-analysis

This repository contains the code and data for a data analysis project of four drive-through stores. The purpose of this project is to identify patterns and trends using data visulization to identify customer behavior and store performance to optimize operational aspects such as staffing, menu offerings, and service stability.

## Data
The data for this project consists of four CSV files, one for each store. Each file contains data on the orders placed at the store, including the arrival time, order time, pickup time, and total time for each order.

## Code
The code for this project is written in Python and uses the following libraries:

- pandas
- datetime
- plotly.express

The code is contained in a Jupyter Notebook file named drive_through_analysis.ipynb. The notebook is divided into four sections, each analyzing a different aspect of the data:

- Histogram of # of orders over time
- Box graph on order time overtime
- Box graph on pickup time overtime
- Box graph on drive time overtime
- Box graph on total overtime

Each section includes a visualization and a brief summary of the insights gained from the analysis.

## General insights(Please find each data graph conclusion inside the file):

1. Store 1071 has the highest overall business volume, while store 1271 has the fewest orders. 
2. Stores 1081 and 1101 exhibit similar patterns.
3. The busiest period for all stores is between 5 am and 9 am. Additionally, red and green stores receive orders early (before 5 am) and late (after 10 pm).
4. Anomalies in order times are visible in the box graph, such as an order that took 489 seconds in the blue store after 5 am. These anomalies are also observed in green and red stores.
5. Variance in service times can be analyzed using the box graph. Longer boxes indicate a larger variance and less consistent service, as observed for the blue store after 5 pm and both green and red stores around 3 am, 3pm, 5pm, 10 pm.
6. The box graph allows for comparison of average order times across different time slots, revealing that the blue and red stores have considerably longer average order times (137 seconds) at specific points.
7. The purple store has fewest orders but unstable service throughout most of the day, indicating considerable room for improvement in service stability.
8. The blue store provides relatively stable service before 4 pm but has a larger variance in pickup times betwee 4pm and 6pm, possibly due to variations in dinner orders.

## Future design frontend work
1. Executive Dashboard: Create an executive dashboard that provides a high-level overview of the key performance indicators (KPIs) for each store, such as the number of orders, average order times, and customer satisfaction scores. This allows managers to quickly assess the performance of each store at a glance.
2. Comparative Analysis: Use visualizations that allow for easy comparison between stores. This can help managers identify best practices, areas for improvement, and opportunities for learning from one another. Bar charts, line charts, or heatmaps can be effective for comparative analysis.
3. Detailed Data Visualization: Use interactive charts and graphs to present the data, allowing users to explore the information in more depth. I'm familiar with ibraries like Plotly, D3.js for creating interactive visualizations above as shown. This can help managers identify best practices, areas for improvement, and opportunities for learning from one another
4. Anomalies and health level: Highlight anomalies and restaurant healthy level based on the data. This can help managers pinpoint issues that require attention and further investigation. Here, we need to talk with the users to build the baseline or the rules of every metrics.

## How to Use
To reproduce the analysis, follow these steps:

Clone the repository to your local machine.
Install the required libraries.
Open the Jupyter Notebook file drive_through_analysis.ipynb.
Run each cell in the notebook to generate the visualizations and analyze the data.

