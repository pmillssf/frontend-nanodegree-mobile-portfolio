### Part 1 Optimize PageSpeed Insights score
As I didn't use gulp, all that's necessary is to click the [link to the live page]https://pmillssf.github.io/frontend-nanodegree-mobile-portfolio/

Mobile: 94 Desktop 96
Changes that I made:
Following Google Recommendations // Udacity's Website Performance Optimization Class
1. Inline style.css
2. Add media="print" for css
3. Move javascript files to bottom of html page and add async
4. resize pizzeria.jpg to pizzeria-min.jpg via http://compressimage.toolur.com/
5. comment out google font

####Part 2: Optimize Frames per Second in pizza.html

Changes that I made:
1. Followed Cameron's example to fix pizza slide resizing. Removed Dx as well
2. Realized main.js was creating 200 moving pizzas every time, changed to create pizzas based on window height.
3. For the updatePositions function:
  1. I defined scrollTop outside of the loop so it wouldn't be repeatedly called
  2. Upon understanding that var phase was just generating the same five numbers over and over I changed it to an array holding the five values so it would be simple to iterate through instead of regenerating the numbers each time.
  
