# vis_exploration

**Exploring population data with plotly**

**Visualization Technique**

Today, I will go over how to create interactive line graphs, scatter plots, & maps using the Plotly Python package. I will investigate the population of countries around the world, in addition to their projected population for future years. In an ever growing society, I am curious if any country is experiencing a population decrease.

Maps are useful to visualize where a country is located, and by incorporating color it provides a scale to represent population. way to see the population of all countries in the dataset. Additionally, using a map provides the reader with a familiar tool to use to explore the data. One can use their previous knowledge in geography to identify the population of the country of their choice and can even learn where certain countries are in the world! However, creating an interactive map can limit your audience since they will not be effective in a static environment like a pdf file.

Scatter plots visualize two numeric data points to observe the relationship between the two variables. Relationships are defined as linear or non-linear and positive or negative. It is important to note that scatter plots can be difficult to understand if too much data is plotted and leaves you with a blob of data points. Also, scatter plots are generally avoid with non numeric values. For my analysis, I will use scatter plots with a slightly different approach. I will utilize the interactive tools in Plotly to show how the population of males and the population of females change over time in select countries. I found this visualization to be a unique way to identify if a country is experiencing a population decrease or increase.

Line graphs are useful to identify a trend over time. In this case I will visualize how the population of a country changes over the years. Line charts are versatile in the ability to plot multiple populations over the same period of time. This can allow me to visualize how the growth between males and females in a country changes over time. Although appropriate in the context of this notebook, line graphs are not always the best visualization to use. For example, if I wanted to compare the populations of males and females for multiple countries I may want to use a grouped bar chart instead. Additionally, line graphs should be avoided when analyzing statistical data such as distribution or interquartile range. Other visualization such as violin plots and box plots are more suited for this.

**Visualization Library**

Founded in Montreal, Quebec by Alex Johnson, Jack Parmer, Chris Parmer, and Matthew Sundquist, Plotly goes beyond Python and offers analytical tools that can be incorporated in R or even enterprise tools that are available for purchase. I will explore Plotly’s Python open source graphing libraries to broaden the knowledge of what is available to create visualizations with Python. I became interested in Plotly when discovering the ease of creating interactive visualizations. I have previously explored interactive graphs in packages like Altair, but I found Plotly to be more straightforward. Additionally, the code used to create visualizations is similar to Matplotlib, making the learning curve more manageable. I also like that Plotly’s interactive graphs can be displayed and used in a Jupyter Notebook. As my preferred environment to work in, I hope incorporating interactive graphs in my notebooks make exploring data more fun and easier to understand.

Under the hood, Plotly’s Python library is built on top of JavaScript. As a declarative tool, we specify what we want the underlying JavaScript to do. The benefit of this in Python is we do not need to worry about explicitly saying all the nuances of how to create the visualization. Rather, we simply command the underlying JavaScript what to do and have that do all the hard work for us. While all of this sounds great, Plotly does come with some disadvantages. Plotlty falls short in customizable features compared to Altair or Seaborn. Also, interactive visualizations are not always needed and matplotlib may be a better option for a quick visual analysis.

**Installation**

To get started with Plotly, I will first install Plotly and get support to use Plotly in a Jupyter Notebook.

Install Plotly (pip): pip install plotly==4.14.3

Install Jupyter support (pip) pip install "notebook>=5.3" "ipywidgets>=7.5"

Install Plotly (conda): conda install -c plotly plotly=4.14.3

Install Jupyter support (conda) conda install "notebook>=5.3" "ipywidgets>=7.5"

Now that I have Plotly installed and supported for Jupyter, I can import it into my notebook as I would with any Python library. By using import.

import Plotly

With Plotly I will use the .express module. This allows you to create common graphs like bar charts, line grapes, and scatter plots. County codes will be used to identify and map the data onto the correct location on a map

Install Pycountry (pip): pip install pycountry

**Documentation**
https://plotly.com/python/

