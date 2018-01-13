# TP1-Packed_Circles_chart_study
A study about packed circles charts : examples, possible variations, and alternative names


# Alternative names :
- Packed bubbles view
- Bubble chart



# Description :
A packed circles chart is a way to display 3D information using the size of circles (or bubbles) as a third property for data encoding. 4D information can be displayed by changing the color of circles. Hereafter is an example of what a packed circles chart looks like [2]:

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/TECTPackedBubbles1.png)

Using a continuous data type as a fourth dimension can lead to the following chart [2]:

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/TECTPackedBubbles3.png)

Even if the relative positions of the circles are sometimes randomly defined (or classified depending on the circle size), note that bubble charts also "allow the comparison of entities in terms of their relative positions with respect to each numeric axis and their size as well" [6] as shown in the following figure.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/BubbleChart2.PNG)



# Data Types
The two first dimensions must be location coordinates (x,y) whereas the third dimension can be of any ordinal or quantitative data type. Usually, the location of circles isn't that important, and this type of chart is used to display information without regards to axes. Finally, the fourth dimension must contain discrete data, but can be of any type (even nominal).




# Comments
- Packed Circles charts are often considered as a variation of scatter plots (with the circle size as an additional property), even if their philosophy is very different.
- This type of charts is a way to display data with space optimization, using the packed-circles method (a variation of "Treemap" graphs)
- Those charts cannot be used to display negative values, unless the color (or shape) of the circle is used to describe the symbol (plus/minus/zero).
- Higher data dimension can be displayed by including circles into other circles (an example is shown in the next section, with Interactive bubble maps) or text labels.



# Variations 

- Bubble maps : This variation of bubble trees takes latitudes and longitudes coordinates as (x,y) coordinates, and the bubbles are displayed on a world map (or any region), as shown below. They are often used to identify region with lower or larger values of any indicators, or to gather together a list of data items across a region [4].

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/Europe-GDP-per-country-1.jpg)

- Interactive bubble maps [5]:
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/Interactive_Bubble_chart.gif)



# Sources :
- [1] The Data visualization catalogue (https://datavizcatalogue.com/methods/circle_packing.html)
- [2] Tableau essentials - Chart types(https://www.interworks.com/fr/blog/ccapitula/2015/01/06/tableau-essentials-chart-types-packed-bubbles)
- [3] Wikipedia - bubble chart (https://en.wikipedia.org/wiki/Bubble_chart)
- [4] eSpatial (https://www.espatial.com/articles/create-a-bubble-map)
- [5] StackOverflow (https://stackoverflow.com/questions/22460816/how-to-create-linked-href-labels-in-a-d3-circle-packing-chart)
- [6] FusionCharts (https://www.fusioncharts.com/chart-primers/bubble-chart/)
