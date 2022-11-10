---
name: Homework 10 - Vasantha Chandrasekaran, Saahil Hiranandani
tools: [Python, HTML, vega-lite, Jekyll]
image: assets/pngs/cars.png
description: Homework 10 completed by Vasantha Chandrasekaran and Saahil Hiranandani
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 10 completed by Vasantha Chandrasekaran and Saahil Hiranandani

Data for this homework comes from [licenses_fall2022](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/licenses_fall2022.csv) and we have referred Professor Jill's [In class notebooks](https://starboard.gg/jnaiman/inClass_week10_online_fall2022-nrSZM7g) for reference.

## First plot visualizes the count of license types from each state. 

### Features: 

- Plot 1 is a visualization that shows the count of license types from each state from the Licenses Dataset. ‘License Type’ is a nominal variable with different categories of license types. ‘State’ is an ordinal variable. The count of license types in each state is visualized in Plot-1.

### Design Choices: 

- <b>Scale</b>: The x axis is chosen to be the License Type and the y-axis is chosen to be States in United States. 
- <b>Mark</b>: The mark is chosen as ‘rect’ as it would be  ideal for interpreting the information about the count of license types in each state.
- <b>Encoding Type</b>: The encoding type for the License Type is chosen as ‘nominal’ since there is no ordering in the categories. The encoding type for States is chosen as ‘ ordinal’ so that the states are listed in alphabetical order. 
- <b>Color</b>:  A colormap is used for the count of records in license type across each state. The encoding type is chosen as ‘ quantitative’, and the aggregate is chosen as ‘count’ since the objective of the visualization is visualize the count of records of license types in each state. The state having the higher number in the variety of license type is highlighted according to the color scale shown on the right.

### Transformations: 

- Interactivity is achieved by the ‘brush’ parameter. The plot is interactive in a way that it allows the selection of a particular interval.

### Overlap: 
- There is no overlap with the analysis done in Homework-9 as different datasets have been used for both approaches.

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.vl.json" style="width: 100%"></vegachart>

## Second plot is a histogram of frequency of license types.

### Features: 

- Plot 2 is a histogram of the frequency of license types. ‘License Type’ is a nominal variable with different categories of license types. The frequency of license types in each state across US is visualized in Plot-2.

### Design Choices:

- <b>Scale</b>: The x axis is chosen to be the License Type and the y-axis is chosen to be the frequency.
- <b>Mark</b>: The mark is chosen as ‘bar’ as it would be  ideal for interpreting the information about the frequency of license types in each state.
- <b>Encoding Type</b>: The encoding type for the License Type is chosen as ‘nominal’ since there is no ordering in the categories. 
- <b>Color</b>:  The color of the bars is not chosen as the objective is to only visualize the frequency of each license type, and by default is blue in color. The encoding type is chosen as ‘ quantitative’, and the aggregate is chosen as ‘count’ since the objective of the visualization is visualize the frequency of  license types. 

### Transformations:

- Plot-2 is not interactive, and it is a histogram of the frequency of license types.

###  Overlap:
- There is no overlap with the analysis done in Homework-9 as different datasets have been used for both approaches.


<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization2.vl.json" style="width: 100%"></vegachart>

## Third and final plot is an interactive dashboard of both plots

The plot showing the count of license types in each state(Plot-1) and the frequency of license types (Plot-2) have been used to create an interactive dashboard. The encoding type, color code and other characteristics are the same as shown in Plot-1 and Plot-2. 

<b>Interactivity</b>: The dashboard is interactive. If a particular interval is selected in the left visualization, the plot on the right is updated showing the frequency of license types according to the region selected in the License Type vs States visualization. 

The interactivity helps in visualizing the information better; The frequency of license types in a particular state or group of states can be visualized easily and the count can be interpreted in a better way.


<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard.vl.json" style="width: 100%"></vegachart>

## The data and analysis

Below is where we have put some links to both the data and the analysis code as buttons:

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="center">
{% include elements/button.html link="https://starboard.gg/vasanthachandrasekaran/Chandrasekaran-vasantha-homework-10-net49aB" text="Analysis on Starboard" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Saahil87/Saahil87.github.io/blob/main/python_notebooks/test_imports_License.ipynb" text="Analysis on Jupyter" %}
</div>