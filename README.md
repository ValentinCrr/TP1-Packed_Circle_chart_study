# TP1-Packed_Circles_chart_study
A study about packed circles charts : examples, possible variations, and alternative names

# Alternative names :
- Packed bubbles view
- Bubble chart

Description :
A packed circles chart is a way to display 3D information using the size of circles (or bubbles) as a third property for data encoding. 4D information can be displayed by changing the color of circles. Hereafter is an example of what a packed circles chart looks like :

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/TECTPackedBubbles1.png)

Using a continuous data type as a fourth dimension can lead to the following chart :

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/TECTPackedBubbles3.png)


# Data Types
The two first dimensions must be location coordinates (x,y) whereas the third dimension can be of any ordinal or quantitative data type. Usually, the location of circles isn't that important, and this type of chart is used to display information without regards to axes. Finally, the fourth dimension must contain discrete data, but can be of any type (even nominal).

# Comments

Packed Circles charts are often considered as a variation of scatter plots (with the circle size as an additional property), even if their philosophy is very different.

This type of charts is a way to display data with space optimization, using the packed-circles method (a variation of "Treemap" graphs)


# Variations 

- bubble maps : This variation of bubble trees takes latitudes and longitudes coordinates as (x,y) coordinates, and the bubbles are dusplayed on a world map (or any region), as shown below :

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/Europe-GDP-per-country-1.jpg)

#Sources :
- [1] The Data visualization catalogue (https://datavizcatalogue.com/methods/circle_packing.html)
- [2] Tableau essentials - Chart types(https://www.interworks.com/fr/blog/ccapitula/2015/01/06/tableau-essentials-chart-types-packed-bubbles)
- [3] Wikipedia - bubble chart (https://en.wikipedia.org/wiki/Bubble_chart)
- [4] eSpatial (https://www.espatial.com/articles/create-a-bubble-map)