# Website Performance Optimization portfolio
date: 30/09/2015

Website Performance Optimization is the 4 project of Front-End Web Developer Nanodegree of [Udacity] (http://www.udacity.com).
In this project I used the Chrome Developer Tool to see why and where the website was performing so badly.


#How to get started:

a - You can visit my GitHub page: http://gus42.github.io/udportfolio

b - Or you can open index.html in your browser. (right-click on index.html file->open with->Chrome/Firefox/Safari)

#List of optimizations:

In optimized folder: you can find the minified css and js, and the index.html with css minified.
To Optimized image and minify css,js I used photosop and Gulp(csso,autoprefixer,uglify,imagemin).

index.html:
- style.css inline and minify
- print.css with media query "print"
- images optimazed
- script moved to the end
- font load using webfontloader 

pizza.html:
- css inline
- class "mover" now has "will-change: left" property

main.js:
- number of mover pizzas are now calculated according to the screen size 
- mover pizzas saved in "var arrayPizzas"
- count of mover pizzas saved in "var count".
- used getElementByClass or getElementById instead of querySelectorAll
- access to scrollTop before the for () insted inside it
- calculation of the 5 phases only one time for updatePositions()
- main "for" of updatePositions() now have "count" iteration, and it doesn't call the DOM, to know scroll and the mover
- deleted function determineDx
- resizePizza now use size in % and not in px
- calls to DOM are execute out from the "for"

Author: Francesco Gusella

Contacts: gus815@gmail.com
