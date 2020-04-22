Title: A legend for ipyleaflet
Date: 2020-04-17 12:03
Category: Python
Tags: jupyter, jupyter-notebook, ipyleaflet, ipywidget
Slug: ipyleaflet-legend-release
Authors: Thomas Pouvreau


# Introducing ipyleaflet-legend

ipyleaflet-legend is a leaflet legend to be used in jupyter-notebook. ipyleaflet-legend is based on the information found in the Custom Legend Control section of this [leaflet tutorial](https://leafletjs.com/examples/choropleth/). We won't go too far into details here, just have in mind that it is both a LeafletControl and an ipywidget. Therefore, ipyleaflet-legend must be instantiated with ipyleaflet. The good news is that since it is a LeafletControl, it can be positioned just like any other ipyleaflet control. 

A second Post or series will follow to explain how ipyleaflet-legend was made. This tutorial might help anyone wanting to import leaflet widget on ipyleaflet using ipywidget.

## Install

At the command prompt enter:

```bash
pip install ipyleaflet-legend
jupyter nbextension enable ipyleaflet_legend --py --sys-prefix
```
>Note: if you are not in a virtual environment, use --user instead of --sys-prefix to enable it.

## Basic Use

Since ipyleaflet-legend is a Leaflet Control implementation for ipyleaflet, we need to instantiate a map:

```python
from ipyleaflet import Map
mymap = Map(center=(-10,-45), zoom=4)
mymap
```
And then add a simple legend:

```python
from ipyleaflet_legend import Legend
my_legend = Legend({"low":"#FAA", "medium":"#A55", "High":"#500"}, name="Legend")
mymap.add_control(my_legend)
```

This is the output of the result in your notebook:
![image](/images/map_legend.png)


More details on [repository notebook example](https://github.com/weatherforce/ipyleaflet-legend/blob/master/example/test_legend.ipynb)

Enjoy!

T.Pouvreau @Weatherforce
