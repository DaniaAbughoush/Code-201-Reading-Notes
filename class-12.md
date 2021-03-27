# Charts;
 great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas elemen.

 * Setting up:
 1.  download Chart.js.
2. Copy the Chart.min.js
3.  create a new html page and copy:
![](/images/script.png)

* Drawing a line chart:
add this line `<canvas id="buyers" width="600" height="400"></canvas>`
*  retrieve the context of the canvas, add this to the foot of your body element:
`<script>`
    `var buyers = document.getElementById('buyers').getContext('2d');`
   ` new Chart(buyers).Line(buyerData);`
`</script>`

* reate our data:
`var buyerData = {`
`	labels : ["January","February","March","April","May","June"],`
`	datasets : [`
	`{`
			`fillColor : "rgba(172,194,132,0.4)",`
			`strokeColor : "#ACC26D",`
			`pointColor : "#fff",`
			`pointStrokeColor : "#9DB86D",`
			`data : [203,156,99,251,305,247]`
		`}`
	``]`
`}`

# Drawing a pie chart:
`<canvas id="countries" width="600" height="400"></canvas>`
*  get the context;
`var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);`
* Next we need to create the data.
`var pieData = [
	{
		value: 20,
		color:"#878BB6"
	},
	{
		value : 40,
		color : "#4ACAB4"
	},
	{
		value : 10,
		color : "#FF8153"
	},
	{
		value : 30,
		color : "#FFEA88"
	}
];`
* add our options:
`var pieOptions = {
	segmentShowStroke : false,
	animateScale : true
}`
* 

# Drawing a bar chart
`<canvas id="income" width="600" height="400"></canvas>`
* retrieve the element and create the graph:
`var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);`
* bar chart’s data:
`var barData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "#48A497",
			strokeColor : "#48A4D1",
			data : [456,479,324,569,702,600]
		},
		{
			fillColor : "rgba(73,188,170,0.4)",
			strokeColor : "rgba(72,174,209,0.4)",
			data : [364,504,605,400,345,320]
		}

	]
}`

# Creating a Chart
It's easy to get started with Chart.js. All that's required is the script included in your page along with a single `<canvas>` node to render the chart.

# `<canvas> `element;
 * the `<canvas> `element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. 

*  is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explore
* rowsers that don't support `<canvas>` will ignore the container and render the fallback content inside it. 

# Required canvas tag
* the `<canvas>` element requires the closing tag (`</canvas>`).
* If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed
* If fallback content is not needed, a simple `<canvas id="foo" ...></canvas> `is fully compatible with all browsers that support canvas at all.

# The rendering context:
* ement creates a fixed-size drawing surface that exposes one or more rendering contexts.
* The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it.

# Checking for support:
Scripts can also check for support programmatically by testing for the presence of the getContext() method.

# A skeleton template;
it is not good practice to embed a script inside HTML. We do it here to keep the example concise
* The script includes a function called draw(), which is executed once the page finishes loading; this is done by listening for the load event on the document.
* this function, or one like it, could also be called using window.setTimeout(), window.setInterval(),

# Drawing shapes with canvas;
1. The grid:
 Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0)
2. Drawing rectangles;
* fillRect(x, y, width, height)
Draws a filled rectangle.

* strokeRect(x, y, width, height)
Draws a rectangular outline.

* clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.

# Drawing paths:
1. First, you create the path
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

* commands:
1. beginPath()
Creates a new path. 

2. Path methods
Methods to set different paths for objects.

3. closePath()
Adds a straight line to the path, going to the start of the current sub-path. 

4. stroke()
Draws the shape by stroking its outline.

5. fill()
Draws a solid shape by filling the path's content area.

# Drawing a triangle:
`function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }
}`

# Lines:
lineTo(x, y)
Draws a line from the current drawing position to the position specified by x and y..

# Applying styles and colors:
1. Colors:
* two important properties we can use: fillStyle and strokeStyle.
* fillStyle = color
Sets the style used when filling shapes.
* strokeStyle = color
Sets the style for shapes' outlines

2. Transparency:
* globalAlpha = transparencyValue
Applies the specified transparency value to all future shapes drawn on the canvas.

3. Line styles:
* There are several properties which allow us to style lines.;
1. lineWidth = value
 width of lines drawn in the future.

2. lineCap = type
appearance of the ends of lines.

3. lineJoin = type
 the appearance of the "corners" where lines meet. 

4. miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes. 

4. getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.

5. setLineDash(segments)
Sets the current line dash pattern.

 6. lineDashOffset = value
Specifies where to start a dash array on a line.

3. Gradients:
1. createLinearGradient(x1, y1, x2, y2)
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
2. createRadialGradient(x1, y1, r1, x2, y2, r2)
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
 
 3. createConicGradient(angle, x, y)
Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

4. Patterns:
1. repeat
Tiles the image in both vertical and horizontal directions.

2.  repeat-x
Tiles the image horizontally but not vertically.
 
 3. repeat-y
Tiles the image vertically but not horizontally.

4. no-repeat
Doesn't tile the image. It's used only once.

5. Shadows:
1. shadowOffsetX = float
Indicates the horizontal distance the shadow should extend from the object.
2. shadowOffsetY = float
Indicates the vertical distance the shadow should extend from the object.
3. shadowBlur = float
Indicates the size of the blurring effect
4. shadowColor = color
A standard CSS color value indicating the color of the shadow effect

# Canvas fill rules:
Two values are possible:

1. "nonzero": The non-zero winding rule, which is the default rule.
2. "evenodd": The even-odd winding rule.

# Drawing text
* fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

* strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

# Styling text:
* font = value
The current text style being used when drawing text.

* textAlign = value
Text alignment setting. Possible values: start, end, left, right or center
 # Advanced text measurements:
 measureText()
Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.

