## Website Performance Optimization portfolio project

In this project, we are tasked to make changes on index.html so it achieves a PageSpeed score of 90 or above. Next we are to make optimizations on views/js/main.js make views/pizza.html render with a consistent frame-rate at 60fps when scrolling. I used Chrome Developer Tools Console and Timeline to measure performance.

Click [here](https://envincebal.github.io/web-optimization/) to view page.

### Optimizations I made

####Part 1: Optimize PageSpeed Insights score for index.html

- Removed Google Font.
- Moved CSS from css.style to inline styling on index.html.
- Added "print" attribute in print.css.
- Added "async" property to "http://www.google-analytics.com/analytics.js" and "js/perfmatters.js."
- Compressed all images.

####Part 2: Optimize Frames per Second in pizza.html

- Removed determineDx function on line 420.
- Stored (document.body.scrollTop / 1250) into a variable outside of loop so it only runs once on line 486.
- Reduced the columns of pizzas from 8 to 6 on line 508.
- Moved "movingPizzas1" into a variable outside of for loop and changed from querySelector to getElementById so it's called only once on line 513.
- Reduced from 200 to 25 pizzas to remove unnecessary pizzas not seen on screen on line 516.
