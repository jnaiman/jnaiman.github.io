---
name: Homework #10
tools: [Python, HTML, vega-lite]
image: assets/pngs/homework10.png
description: Example of post with vega-lite!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Plots of the Buildings Dataset using vega-lite

In the following plot, I am visualizing the Year Acquired vs. Year Constructed for different Congressional Districts.  I've transformed the data into date-time formats for easier plotting for the Year Constructed and Year Acquired columns.  For the Year columns, I used "T" for temporal encodings and for Congress Dist I used "N" for nominal (unordered categorical data).  I just used the default color scheme for Congress Dist since it's a nice categorical color scheme that is linked by default when I select "N"/nominal for the data type.  I used a different set of plots for Homework #9.


<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>

In the following plot, I am visualizing the Square Footage vs. Total floors for different Congressional Districts. For this plot, I didn't have to do any data transformations.  For Congress Dist I used "N" for nominal data and let the default encoding types (Q) be found for Total Floors and Squre Footage.  Like in the previous plot just used the default color scheme for Congress Dist since it's a nice categorical color scheme that is linked by default when I select "N"/nominal for the data type.  I used a different set of plots for Homework #9.

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>

In my final plot, I am visualizing the *Total* Square Footage vs. Total floors. For this plot, did a groupby-sum of the square footage on each floor.  I let the default encoding types (Q) be found for Total Floors and Total Square Footage for the barchart.  Here, there is no color scheme, so I went with the default blue.  I used a different set of plots for Homework #9.

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot3.json" style="width: 100%"></vegachart>

My interactive elements are the tooltips in the top two plots which show the Congress Dist when you hover over a point. Since there are a few times that the color scheme I used "loops" and repeats a color, this helps the user pick out the congressional district of specific points on the plots.

Note that in ALL plots -- I have transformed the data by setting zeros in Floors, Square Footage, and Year to NaN's and then removing these NaN's for the first plot of time (i.e. removing the rows that have NaN's in the Year Acquired and/or Year Constructed).




<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<!--
<div class="right">
{% include elements/button.html link="../python_notebooks/analysis_notebook.ipynb" text="The Analysis" %}
</div>
-->

<!-- note: this is a link example to another notebook that is public on github -->

<div class="right">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week15/prep_notebook_week15.ipynb" text="The Analysis" %}
</div>



