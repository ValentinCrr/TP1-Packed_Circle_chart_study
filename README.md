# TP1-Packed_Circles_chart_study

**Definition**: Circle Packing is a method to visualize large amounts of hierarchically structured data. Tangent circles represent brother nodes at the same level; to visualize the hierarchy, all children of a node are packed into that node (and thus determine its size).[1]

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/simple_packed_circle_diagram.png)

__A simple packed circle chart__

## 1. Alternative names :
- Packed bubble(s) chart
- Packed circle(s) diagram


## 2. Description :
A packed circles chart is thus a way to display 1D to 3D (or even 4D) information using the size of circles (or bubbles) as a property for data encoding. Its origin is unknown but it is a variation of a scatter plot chart even if their philosophy is very different. 3D information is usually displayed by changing the color of circles. Hereafter is an example of what a packed circles chart looks like [2]:

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/TECTPackedBubbles1.png)

__Example of a bubble chart__

## 3. Data Types

The first dimension must be of ordinal or quantitative data type, so that it can be "converted" into a circle diameter. Depending on how you display the data (bubble color, text label, distance to center, the type of the dataset can vary a lot.
The following figures show various use of bubble charts depending on the dimension of the displayed dataset.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/2D_bubble_chart.jpg)

__Packed Bubble chart with 2D dataset[2]__

In the previous figure, the second dimension of the dataset contain nominal data, and is simply displayed via text labels. However, the bubbles color is also often used if the data is at least ordinal.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/3D_bubble_chart.png)

__Packed Bubble chart with 3D dataset[4]__

Using a continuous data type for the coloring dimension can lead to graphs where the bubbles color varies continuously as shown in the next figure, where data labels are used in order to display a fourth data dimension.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/4D_bubble_chart.png)

__Packed Bubble chart with higher dimension dataset__


## 4. Comments
- This type of charts is a way to display data with space optimization, using the packed-circles method. However, it can easily become unreadable if the data range is too high, or if the dataset size is too important, as shown on the following figure. Interactive charts are needed in that case.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/TooMuchData.PNG)

__Packed circle chart with too much data [4]__

- Several packing methods exist. If all the circles had the same size, uniform packing could be used. However, packed bubble chart used unequal circle, changing the process into a optimization problem : finding the maximum density of a space containing all the circles, i.e. the smallest space containing them.


- Those charts cannot be used to display negative values, unless the color (or shape) of the circle is used to describe the symbol (plus/minus/zero).
- Higher data dimension can be displayed by including circles into other circles, thus creating trees
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/BubblesIntoBubbles.png)

__A packed circle chart with several levels[5]__

- The Circle Packing process is a variation of a Treemap that uses circles instead of rectangles. Each circle represents a level in the hierarchy (see the following figure): each branch of the tree is represented as a circle and its sub-branches are represented as circles inside of it. [6]

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/circle_packing_tree.svg)

__Packed circles seen as a treemap__


## 5. Variations

- **Bubble chart** : The packed-circles charts are actually a variation of the bubble charts. In those bubble charts, the space is not an important matter, as shown below :
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/BubbleChart.png)

__Bubble chart[7]__


- **Bubble maps** : This variation of bubble trees takes latitudes and longitudes coordinates as (x,y) coordinates, and the bubbles are displayed on a world map (or any region), as shown below. They are often used to identify region with lower or larger values of any indicators, or to gather together a list of data items across a region [8]. However, this is more a bubble chart than a packed circle chart.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Europe-GDP-per-country-1.jpg)

__Bubble map[8]__


- **Interactive bubble charts** [9]: When the dataset dimension is too high, interactive charts are used as shown below. This also allows to isolate parts of the dataset.
![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Interactive_Bubble_chart.gif)

__Interactive bubble chart__


## 6. "Exotic" packed-circles charts
 The following charts were extracted from "TheDataViz" project, and show various examples of what can be accomplished with packed circle charts.

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/Exotic1.gif)

![alt text](https://github.com/ValentinCrr/TP1-Packed_Circle_chart_study/blob/master/img/grape_packed_circle.jpg)


## 7. Tools

Most of the packed bubble charts are created using Tableau (see Tableau Essentials website for details). Only bubble charts can be created with most of the commonly used softwares (including Microsoft Excel).


## 8. Sources :
- [1] DataVizProject
- [2] Tableau essentials - Chart types(https://www.interworks.com/fr/blog/ccapitula/2015/01/06/tableau-essentials-chart-types-packed-bubbles)
- [3] StackOverflow - Flex Packed Bubble Chart
- [4] VisualCapitalist (https://www.visualcapitalist.com/population-every-country-bubble/)
- [5] GitHub - d3-hierarchy
- [6] The Data Visualisation Catalogue
- [7]Visage - How to design bubble charts (https://visage.co/data-visualization-101-bubble-charts/)
- [8] eSpatial (https://www.espatial.com/articles/create-a-bubble-map)
- [9] StackOverflow (https://stackoverflow.com/questions/22460816/how-to-create-linked-href-labels-in-a-d3-circle-packing-chart)
