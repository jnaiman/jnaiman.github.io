---
name: More Complex Plots with Python + Altair
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/firstbuildingsplot.png
description: This project makes more complex plots using Altair + Python.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

## Buildings dataset

First just a pan/zoom "for free" interactivty:

<vegachart schema-url={{site.baseurl}}"/assets/json/buildings_sqft.json" style="width: 100%"></vegachart>

Add in a multi-line tool tip:
<vegachart schema-url={{site.baseurl}}"/assets/json/buildings_sqft_multitooltip.json" style="width: 100%"></vegachart>

And then with a dropdown to select my stats:
<vegachart schema-url={{site.baseurl}}"/assets/json/buildings_stats_dropdown.json" style="width: 100%"></vegachart>

## Corgis dataset

First interactive world map:
<vegachart schema-url={{site.baseurl}}"/assets/json/corgis_dotchart_world.json" style="width: 100%"></vegachart>

But the above has artifacts and so, let's try with smooth transitions with interpolation:
<vegachart schema-url={{site.baseurl}}"/assets/json/corgis_dotchart_world_smooth.json" style="width: 100%"></vegachart>





<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/corgs_per_country_over_time_columns_2020.csv" text="Main Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week13/inClass_week13.ipynb" text="The Analysis" %}
</div>

