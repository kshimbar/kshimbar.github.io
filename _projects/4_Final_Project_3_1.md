---
name: Final Project 3.1
tools: [Python, HTML, vega-lite]
image: assets/pngs/fp3-1.png
description: Final Project 3.1
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Final Project 3.1 
<br>
Written by Group 17 (Kohta Shimbara, Nicholas Yeung, Sophia Matias)
<br>
<br>

# The Dataset
<br>
The dataset covers various aspects of video games including their features (like if they are handheld, support max players, are multiplatform, or have online capabilities), metadata (genres, whether they are licensed, publishers, if they are a sequel), sales metrics (review scores, sales, used price), release information (console, rating, year, if it’s a re-release), and length in different play styles (average, leisure, median, polled, rushed) for various game modes (all playstyles, completionists, main story, main story + extras). These fields provide a comprehensive overview of video game characteristics, sales performance, and player engagement metrics
<br>
<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/fp3-1.json" style="width: 100%"></vegachart>
<br>
<br>
<br>

# Main Visualization
<br>
The visualization above depicts the relationship between the genre and sales of video games from the videogames.csv dataset. With the bars each depicting a genre of video games and the Y axis representing the number of video games under each genre. Through this visualization, you can see games under the action genre are most represented. With sports and racing/driving being the second and third genre most games fall under. 
<br>
<br>


<vegachart schema-url="{{ site.baseurl }}/assets/json/fp3-1-con1.json" style="width: 100%"></vegachart>
<br>
<br>
<br>

# Contextual Visualization: Global Sales of Video Games Between 2004 and 2010 By Genre
<br>
This visualization was made from the Video Games Sales dataset retrieved from [this link](https://data.world/sumitrock/video-games-sales). This visualization shows the global sales of video games (measured in millions) between 2004 and 2010 and is color coded by the genre of the video game. Since this dataset consists of more than 10,000 rows, we filtered the dataset to only include games between 2004 and 2010 in order to match the years of our main dataset. The dataset was also filtered to only display video games that had global sales of $0.01 million or more. Between 2004 and 2010, we can see that Wii Sports had the highest global sales in 2006 of 82.74 million which falls into the sports genre. Feel free to use the dropdown to see the global sales of different genres and you can hover over the data points to see more information. 

<br>
<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/fp3-1-con2.json" style="width: 100%"></vegachart>

<br>
<br>
<br>

# Contextual Visualization: Top 10 Video Game Publishers By Global Sales 
<br>
This visualization was also made from the Video Games Sales dataset. This visualization shows the top 10 video game publishers that sold the most video games globally. The visualization is in descending order so we can see that Nintendo had the most global sales.  

<br>
<br>

<div class="left">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/assets/csv/video_games.csv" text="The Main Dataset" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kshimbar/kshimbar.github.io/blob/master/test.ipynb" text="The Python Notebook" %}
</div>