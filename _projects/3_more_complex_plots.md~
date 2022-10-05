---
name: Vega-lite Plots, 5 Ways
tools: [Python, HTML, vega-lite]
image: assets/pngs/vegalite5ways.png
description: This project shows how to get vega-lite plots into our project pages in multiple ways.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# 1. Vega-lite from the editor!

Use `vegachart` HTML plug in from the Jekyll walkthrough to host this JSON.

<vegachart schema-url="{{site.baseurl}}/assets/json/horbarchart2.json" style="width: 100%"></vegachart>


# 2. Use vega-specifications in Python with Altair

Adding in a simple histogram that we ported from Starboard:

<vegachart schema-url="{{site.baseurl}}/assets/json/hist.json" style="width: 100%"></vegachart>


# 3. Dashboard Building (combo fo vega-specs AND Altair-style plotting)

First try, a static, non-linked version of our chart:

<vegachart schema-url="{{site.baseurl}}/assets/json/static_mobility.json" style="width: 100%"></vegachart>

A small (though not-size responsive chart) is here:
<vegachart schema-url="{{site.baseurl}}/assets/json/static_mobility_small.json" style="width: 100%"></vegachart>

Now with interactivity:

<vegachart schema-url="{{site.baseurl}}/assets/json/dashboard_mobility.json" style="width: 100%"></vegachart>


# 4. Use Altair to make the dashboard (online data)

First we started with a quick scatter plot using "Altair-style" vega-lite:
<vegachart schema-url="{{site.baseurl}}/assets/json/population_scatter.json" style="width: 100%"></vegachart>

And then, using only Altair-flavored vega-lite Python commands we re-made this dashboard:
<vegachart schema-url="{{site.baseurl}}/assets/json/altair_mobility_dashboard.json" style="width: 100%"></vegachart>



# 5. Python Data analysis + Altair for Plotting

Oh look, we made the EXACT same plot but in a *new and fancy way in Python!*
<vegachart schema-url="{{site.baseurl}}/assets/json/altair_mobility_data_dashboard.json" style="width: 100%"></vegachart>







<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/mobility.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week11/inClass_week11.ipynb" text="The Analysis" %}
</div>

