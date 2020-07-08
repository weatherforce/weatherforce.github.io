Title: A way to build widgets on Jupyter Notebook with React
Date: 2020-07-08 15:30
Category: Python
Tags: jupyter, jupyter-notebook, ipyreactwidgets
Slug: ipyreactwidgets-release
Authors: Thomas Pouvreau, Alex Blaza, Alex Amarandon

# Hey! You are found of React, and would like to build widgets for your notebooks using it? then check this out !

![image](/images/ipyreact.png)

## IpyWhat? 

We are proud to present __ipyreact__, a beta version of a widget library for jupyter notebook using React on the front end. The aim is not to replace the great [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) project. Instead, ipyreact focuses on providing an alternative solution building widgets. 

## Why React? What for?  

React allows us to leverage both its efficiency and usability, through the state mechanism, and of course, JSX. Furthermore, using React allows developers to easily incorporate the [Material-UI](https://material-ui.com/) library into their project taking advantage of cool features such as theming and its components library designed with UX/UI best practices. That use of good looking component with theming options might not be useful for notebooks use as internal tools to share code and experiment with it. However, It becomes necessary when it comes to build dashboard with tools such as Voila. In that particular case, the use of React as front end library will be very useful since it is its very purpose to provide a simple development tool for building complexe user interfaces. 


## Where do I start ? 
 
The project is now quite young, yet it might become your next favorite widget library to build dashboards from notebooks!
To get started, you can have a look at [the code here](https://gitlab.com/weatherforce-platform/ipyreactwidgets).

To get details, do not hesitate to checkout [the documentation](https://weatherforce-platform.gitlab.io/ipyreact/)

And if you are eager to try it out, have a look at [the quickstart](https://weatherforce-platform.gitlab.io/ipyreact/quickstart.html) !

This project is still at an early stage so it would be great if you would like to get involved. You can start by have a look at our [developer guide](https://weatherforce-platform.gitlab.io/ipyreact/make-a-widget.html), start coding and send us a pull request!

<p align="center">
	<img src="https://media.giphy.com/media/vyEMmgHf9dQ4M/giphy.gif"/>
</p>

>Note:If you encounter any issues or want to add new features then please raise an issue [here](https://gitlab.com/weatherforce-platform/ipyreact/-/issues).
