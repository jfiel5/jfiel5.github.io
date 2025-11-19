---
name: Bigfoot Sightings
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Bigfoot Sitings!

The following are visualizations using altair.



For this first graphic, I wanted to make a representation of where the bigfoot sightings were located. The best way to do that was my using a mark circle chart. I like this better instead of overlaying it directly over a map because you can make out the United States just based on where the dots are located. Also, the colors represent a different state, so If you wanted to see where the different sightings are by state, you are able to see that. Some of the encodings I used was color, by state, so that you were able to see what I was just describing. The opacity is lowered a little bit so that when there are more sightings in an area, the color will be more dense. There is a tool tip interactivity that shows you the date of when the siting itself was. This is information that would clutter the representation so i decided to keep it as the tooltip. I'm very proud of this visualization and I think it is a fun way to geographically see where bigfoot sightings are.

<vegachart schema-url="{{ site.baseurl }}/assets/json/sitings_map.json" style="width: 100%"></vegachart>


For my second visualization, I wanted to look at multiple different intersections of data. Specifically, I wondered if there was a relationship between heat, humidity, and the number of sightings. The x-axis of the first graph shows the mid temperatures of where the sightings were and the humidity in that area. The graph on the left shows that the hotter the area was, the more humid it was. the color scale for the graph on the left corresponds to the humidity, so the more humidity there is, the more red the point is. Then, on the right, you can see a simple histogram of the # of reports of bigfoot vs the humidity. There is a correlation between the two and most bigfoot sightings happen between .7 and .9 humidity levels. This is probably because of wooded areas and whatnot. I chose this off of altiars website because I thought he side-by-side looked cool. Also, the tooltip is utilized to allows users to select on specific points.

There are links to my dataset and teh notebook I have uploaded. Thank you!
<vegachart schema-url="{{ site.baseurl }}/assets/json/humidity_sitings.json" style="width: 100%"></vegachart>

<!-- 
In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet. -->


## Search The Data & Methods

Below are links to the dataset and the jupyter notebook used for analysis:

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
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jfiel5/jfiel5.github.io/blob/main/python_notebooks/homework5_script.ipynb" text="The Analysis" %}
</div>