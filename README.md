## Website Performance Optimization Portfolio Project
The challenge in this project was to optimize the online portfolio for speed. In particular, to optimize the critical rendering path and make this page render as quickly as possible.

### To run the file , go to https://sameersattur.github.io/frontend-nanodegree-mobile-portfolio/

### Optimizations 
#### Part 1: Optimize PageSpeed Insights score for index.html
##### Changes made:
- Compressed pizzeria.jpg and profilepic.jpg
- Used asynchronous google font
- Inline style.css and print.css
- Used async JavaScript instead of loading it externally

#### Part 2: Make pizza.html to load at 60fps 
#### Changes made in views/js/main.js file:
- Made changes in changePizzaSizes function
- Made changes in updatePositions function
- Changed  querySelectorAll to getElementsByClassName in changePizzaSizes function
- Changed the querySelector call for selecting movingPizzas1 element to getElementById
- Changed the number of pizzas generated on page load to be based on the browser window resolution.


#### Optimizations made in views/css/styles.css
- Included transform: translateZ(0) and backface-visibility:hidden in .mover class
