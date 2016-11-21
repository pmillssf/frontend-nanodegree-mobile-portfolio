### Part 1 Optimize PageSpeed Insights score
As I didn't use gulp, all that's necessary is to click the [link to the live page](https://pmillssf.github.io/frontend-nanodegree-mobile-portfolio/)

#### Google page speed score: Mobile: 94 Desktop 96
Changes that I made:
Following Google Recommendations // Udacity's Website Performance Optimization Class
* Inline style.css
* Add media="print" for css
* Move javascript files to bottom of html page and add async
* Resize pizzeria.jpg to pizzeria-min.jpg via http://compressimage.toolur.com/
* comment out google font
* minify js and css files, including inline css
####Part 2: Optimize Frames per Second in pizza.html

Changes that I made:
* Followed Cameron's example to fix pizza slide resizing. Removed Dx as well
*  Realized main.js was creating 200 moving pizzas every time, changed to create pizzas based on window height.
* For the updatePositions function:
  1. I defined scrollTop outside of the loop so it wouldn't be repeatedly called
  2. Upon understanding that var phase was just generating the same five numbers over and over I changed it to an array holding the five values so it would be simple to iterate through instead of regenerating the numbers each time.
