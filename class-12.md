# Chart.js, Canvas
:
## Chart.Js:

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:  
`<script src='Chart.min.js'></script>`

## Drawing a line chart:



`<canvas id="buyers" width="600" height="400"></canvas>`




## Drawing a pie chart:

`<canvas id="countries" width="600" height="400"></canvas>`

And next:


`var countries= document.getElementById("countries").getContext("2d");`

`new Chart(countries).Pie(pieData, pieOptions);`

And next:

`var pieData = [{value: 20,color:"#878BB6"},`
`{value : 40,color : "#4ACAB4"},`
`{value : 10,color : "#FF8153"},`
`{value : 30,color : "#FFEA88"}];`

And you can also bo (Drawing a bar chart)

**To know more please 
[visit this page](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)**

-------

## Canvas:

`<canvas id="tutorial" width="150" height="150"></canvas>`

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed,
 the `<canvas>` element has only two attributes, `width` and `height`.

## Drawing shapes with canvas:

- Drawing rectangles
- Drawing paths
- Drawing a triangle
- Drawing Lines
- Drawing Arcs
- Drawing Bezier and quadratic curves
- Drawing Cubic Bezier curves

**To more info please 
[visit this pages](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes#rectangular_shape_example)**

------------

## Applying styles and colors:

**Colors:**

Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: `fillStyle` and `strokeStyle`.

`fillStyle = color`

    Sets the style used when filling shapes.

`strokeStyle = color`

    Sets the style for shapes' outlines.


**Line styles:**

`lineWidth = value`

`lineCap = type`

`lineJoin = type`

`miterLimit = value`

`getLineDash()` 

`setLineDash(segments)`

`lineDashOffset = value`


**Gradients:**

`createLinearGradient(x1, y1, x2, y2)`
    
`createRadialGradient(x1, y1, r1, x2, y2, r2)`
    
`createConicGradient(angle, x, y)`

**To more info please :[ Visit This Page](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors#transparency)**


--------------
## Drawing text:

**Drawing text:**

`fillText(text, x, y [, maxWidth])`

`strokeText(text, x, y [, maxWidth])`


**Styling text:**

`font = value`
    
`textAlign = value`
    
`textBaseline = value`
    
`direction = value`



**To more info please :[ Visit This Page](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)**








