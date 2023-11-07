---
name: Vega Lite Example Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/wow.json" style="width: 100%"></vegachart>
In this visualization, an interactive bar chart is created to display the count of buildings acquired by year, with a color distinction for different agencies. The design uses ordinal encoding for the 'Year Acquired' on the x-axis and quantitative encoding for the count on the y-axis. The color encoding is based on the agency name, which is highlighted when selected with an interval brush, otherwise defaulting to a neutral light gray to reduce visual distractions. The interval brush allows for selection along the x-axis, enabling users to focus on specific years and see the corresponding count of buildings acquired. This interactivity not only adds depth to the data exploration but also allows for a comparative analysis across different time periods, making the visualization more informative and dynamic. The tooltip provides immediate feedback on the year and count of buildings, enhancing the data's readability and user engagement.

<vegachart schema-url="{{ site.baseurl }}/assets/json/test.json" style="width: 100%"></vegachart>
In this visualization, I'm crafting an interactive scatter plot that illustrates the relationship between the year buildings were acquired and their square footage, colored by agency name. The design leverages a quantitative encoding for the years and square footage, while nominal encoding is applied to the agency names with a color scheme that distinguishes agencies for clarity. A light gray fallback color is used for non-highlighted points to maintain focus on the selection. Data transformation was minimal, slicing the dataset for manageability. Interactivity is introduced through a 'mouseover' event, which highlights the nearest data point and displays a tooltip with detailed information. This feature not only makes the visualization more engaging but also allows for an immediate, detailed view of the data without cluttering the visual field, enhancing both clarity and user interest.


In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.


## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

