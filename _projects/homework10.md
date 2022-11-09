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

First plot visualizes the count of license types from each state. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.vl.json" style="width: 100%"></vegachart>

Second plot is a histogram of frequency of license types.

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization2.vl.json" style="width: 100%"></vegachart>

Third and final plot is an interactive dashboard of both plots 

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