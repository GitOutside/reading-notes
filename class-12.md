# Chart.js
Chart.js is a javaScript plugin that makes creating all kinds of charts.

You make a ```<canvas>``` tag in HTML.
Then write script that gets context and add to the ```<body>``` element.
Then you make an object that the necessary ahcrt information.

Before Chart.js, making charts was much more difficult.

# The ```<canvas>``` element
This is similar to the image element, but there are only two attributes: width and height, which are optional.

The reaminder of the reading is a tutorial for using canvas. I believe that reading the tutorial ans referencing it when I am using it makes re-writin it here unncessary.

This element needs a closing tag since it includes the option for a fallback image. 
Boroswers that support ```<canvas>``` will ignore the fallback, but those that don't will use the fallback. 

The canvas is initially blank, and uses js to fill it in. js uses the draw```()``` function to render the chart.