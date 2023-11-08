---
name: HW 8 Visualization 1
tools: [Python, HTML, vega-lite]
image: assets/pngs/vis1.png
description: Homework 8 submission 1
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Homework 8 Visualization 1


<vegachart schema-url="{{ site.baseurl }}/assets/json/wow.json" style="width: 100%"></vegachart>


# Write up
In this visualization, an interactive bar chart is created to display the count of buildings acquired by year, with a color distinction for different agencies. The design uses ordinal encoding for the 'Year Acquired' on the x-axis and quantitative encoding for the count on the y-axis. The color encoding is based on the agency name, which is highlighted when selected with an interval brush, otherwise defaulting to a neutral light gray to reduce visual distractions. The interval brush allows for selection along the x-axis, enabling users to focus on specific years and see the corresponding count of buildings acquired. This interactivity not only adds depth to the data exploration but also allows for a comparative analysis across different time periods, making the visualization more informative and dynamic. The tooltip provides immediate feedback on the year and count of buildings, enhancing the data's readability and user engagement. Also, I used the same dataset from the HW7, but the visualization is comletely different in the way that this visualization is interactive and also the topic of the visualization. (For the previous visualization, I showed the average square feet of each room group by the floors.)

<div class="left">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/assets/json/wow.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/test.ipynb" text="The Analysis" %}
</div>
