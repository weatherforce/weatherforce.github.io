Title: A legend for Ipyleaflet 
Date: 2020-04-17 12:03
Category: Python
Tags: jupyter, jupyter-notebook, ipyleaflet, ipywidget
Slug: Ipyleaflet-Legend is released
Authors: Thomas Pouvreau


# Introducing ipyleaflet-legend

It is an implementation on jupyter notebook of a leaflet legend found in this [leaflet tutorial](https://leafletjs.com/examples/choropleth/). More precisely, it refers to the Custom Legend Control section. We won't go too far in details here, just have in mind that it is both a LeafletControl and an ipywidget. So it cannot work outside of ipyleaflet and must be instantiated with it. The good news is that since it is a LeafletControl, it can be positioned like any other ipyleaflet control. 

A second Post will follow or a serie to explain how it was done. It might be an help to everyone seeking for importing leaflet widget on ipyleaflet using ipywidget. 

## Install 

Just hit:

```bash
pip install ipyleaflet-legend
jupyter nbextension enable ipyleaflet_legend --py --sys-prefix
```
>Note: if you are not in a virtual environment, use --user instead of --sys-prefix to enable it.

## Basic Use

Since it is a Leaflet Control implementation for ipyleaflet, we need to instantiate a map: 

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

And this is is what you will obtains as a final result into your notebook: 
![image](/images/map_legend.png)


More details on [repository notebook example](https://github.com/weatherforce/ipyleaflet-legend/blob/master/example/test_legend.ipynb)

Enjoy !

T.Pouvreau @Weatherforce 
