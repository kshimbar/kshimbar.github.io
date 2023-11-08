---
name: HW 8 Visualization 2
tools: [Python, HTML, vega-lite]
image: assets/pngs/vis2.png
description: Homework 8 submission 2
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Homework 8 Visualization 2


<vegachart schema-url="{{ site.baseurl }}/assets/json/test.json" style="width: 100%"></vegachart>

# Write-up

In this visualization, I'm crafting an interactive scatter plot that illustrates the relationship between the year buildings were acquired and their square footage, colored by agency name. The design leverages a quantitative encoding for the years and square footage, while nominal encoding is applied to the agency names with a color scheme that distinguishes agencies for clarity. A light gray fallback color is used for non-highlighted points to maintain focus on the selection. Data transformation was minimal, slicing the dataset for manageability. Interactivity is introduced through a 'mouseover' event, which highlights the nearest data point and displays a tooltip with detailed information. This feature not only makes the visualization more engaging but also allows for an immediate, detailed view of the data without cluttering the visual field, enhancing both clarity and user interest. Also, I used the same dataset from the HW7, but the visualization is comletely different in the way that this visualization is interactive and also the topic of the visualization. (For the previous visualization, I showed the average square feet of each room group by the floors.)

<div class="left">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/assets/json/test.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/test.ipynb" text="The Analysis" %}
</div>
