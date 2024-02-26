## Introduction

In this project, I have created a step-by-step guide on how to prepare various types of graphical visuals using Python's Matplotlib library. I used Jupyter Notebook as the IDE and leveraged Pandas, Numpy, and Matplotlib libraries for data manipulation and visualization.

The project covers the following graphical visuals:

- Line Graph
- Bar Graph
- Histogram
- Pie Chart

## Project Details

### IDE: Jupyter Notebook
### Python Libraries: Pandas, Numpy, Matplotlib
### Documentation Link: [Matplotlib Documentation](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)

## Plotting Line Graph

- Defined legend parameters including title, labels, fonts, fontsize, scale/ticks, color, marker, markersize, markeredgecolor, etc.
- Plotted 2 line graphs.
- Resized the graph using figsize and dpi.
- Saved the graph using plt.savefig.

## Plotting Bar Graph

- Defined the legend parameters.
- Plotted the bar graph.
- Applied hatch pattern to the bar graph.
- Resized the bar graph.
- Saved the bar graph.

## Project 1: Gas Dataset

- Imported the gas dataset using the Pandas function.
- Used the head() function to check the dataset.
- Plotted the line graph (Years Vs Price in USD) with the title "Gas Prices of Countries over Years."

### Visual Insights: 
- South Korea has the highest gas rates, followed by Australia, Canada, and the USA.
- There is a sudden rise in gas prices after the year 2002.

## Project 2: Fifa Dataset

- Imported the Fifa dataset using the Pandas function.
- Used the head() function to check the dataset.

### Plotting the Histogram:
- Defined the legend parameters.
- Plotted the histogram (Skill Level vs Number of Players) with the title "Distribution of Player Skills in Fifa 2018."

### Visual Insights:
- The majority of players have skill levels ranging between 60-70.

### Plotting the Pie Chart:
- Checked the value counts of players who use their left or right foot during matches.
- Plotted the pie chart (left, right) with the title "Foot Preference in the FIFA Match."

### Visual Insights:
- 76.81% of players use their right foot, while 23.19% use their left foot during matches.
