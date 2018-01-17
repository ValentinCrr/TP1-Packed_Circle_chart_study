# TP1-Packed_Circles_chart_study

**Definition**: Circle Packing is a method to visualize large amounts of hierarchically structured data. Tangent circles represent brother nodes at the same level; to visualize the hierarchy, all children of a node are packed into that node (and thus determine its size).[1]

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/simple_packed_circle_diagram.gif)
__A simple packed circle chart__

## 1. Alternative names :
- Packed bubbles chart
- Packed circle diagram


## 2. Description :
A packed circles chart is thus a way to display 1D to 3D (or even 4D) information using the size of circles (or bubbles) as a property for data encoding. Its origin is unknown but it is is a variation of a scatter plot chart even if their philosophy is very different. 4D information can be displayed by changing the color of circles. Hereafter is an example of what a packed circles chart looks like [2]:

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/TECTPackedBubbles1.png)
__Example of a bubble chart__

Using a continuous data type as a fourth dimension can lead to graphs where the color vary continuously (as you can see in the next section, with the figure called "Bubble chart with higher dimension dataset")

## 3. Data Types

The first dimension must be of ordinal or quantitative data type, so that it can be "converted" into a circle diameter. Depending on how you display the data (bubble color, text label, distance to center, the type of the dataset can vary a lot.
The following figures show various use of bubble charts depending on the dimension of the displayed dataset.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/2D_bubble_chart.jpg)
__Packed Bubble chart with 2D dataset__

In the previous figure, the second dimension of the dataset contain nominal data, and is simply displayed via text labels. However, the bubbles color is also often used if the data is at least ordinal.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/3D_bubble_chart.png)
__Packed Bubble chart with 3D dataset__

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/4D_bubble_chart.png)
__Packed Bubble chart with higher dimension dataset__

## 4. Comments
- This type of charts is a way to display data with space optimization, using the packed-circles method. However, it can easily become unreadable if the data range is too high, or if the dataset size is too important, as shown on the following figure. Interactive charts are needed in that case.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/TooMuchData.PNG)
__Packed circle chart with too much data [X]__

- Several packing methods exist. If all the circles had the same size, uniform packing could be used. However, packed bubble chart used unequal circle, changing the process into a optimization problem : finding the maximum density of a space containing all the circles, i.e. the smallest space containing them.


- Those charts cannot be used to display negative values, unless the color (or shape) of the circle is used to describe the symbol (plus/minus/zero).
- Higher data dimension can be displayed by including circles into other circles, thus creating trees
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/BubblesIntoBubbles.png)
__A packed circle chart with several levels[Y]__

- The Circle Packing process is a variation of a Treemap that uses circles instead of rectangles. Each circle represents a level in the hierarchy (see the following figure): each branch of the tree is represented as a circle and its sub-branches are represented as circles inside of it. [7]
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/circle_packing_tree.svg)
__Packed circles seen as a treemap__

## 5. Variations 

- Bubble chart : The packed-circles charts are actually a variation of the bubble charts. In those bubble charts, the space is not an important matter, as shown below :
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/BubbleChart.png)
__Bubble chart[Z]__

- Bubble maps : This variation of bubble trees takes latitudes and longitudes coordinates as (x,y) coordinates, and the bubbles are displayed on a world map (or any region), as shown below. They are often used to identify region with lower or larger values of any indicators, or to gather together a list of data items across a region [4]. However, this is more a bubble chart than a packed circle chart.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Europe-GDP-per-country-1.jpg)
__Bubble map__

- Interactive bubble chart [5]: When the dataset dimension is too high, interactive charts are used as shown below. This also allows to isolate parts of the dataset.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Interactive_Bubble_chart.gif)
__Interactive bubble chart__

## 6. "Exotic" packed-circles charts
 The following charts were extracted from "TheDataViz" project, and show various examples of what can be accomplished with packed circle charts.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Exotic1.gif)
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/grape_packed_circle.jpg)

## Sources :
- [1] DataVizProject
- [2] Tableau essentials - Chart types(https://www.interworks.com/fr/blog/ccapitula/2015/01/06/tableau-essentials-chart-types-packed-bubbles)
- [4] eSpatial (https://www.espatial.com/articles/create-a-bubble-map)
- [5] StackOverflow (https://stackoverflow.com/questions/22460816/how-to-create-linked-href-labels-in-a-d3-circle-packing-chart)
- [6] FusionCharts (https://www.fusioncharts.com/chart-primers/bubble-chart/)
- [7] The Data Visualisation Catalogue
- [X] VisualCapitalist (https://www.visualcapitalist.com/population-every-country-bubble/)
- [Z]Visage - How to design bubble charts (https://visage.co/data-visualization-101-bubble-charts/)
- [Y] GitHub - d3-hierarchy