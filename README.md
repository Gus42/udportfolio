## Website Performance Optimization portfolio project 4

@author Francesco Gusella

@date 30/09/2015

How to get started:

a - You can visit my GitHub page: http://gus42.github.io/udportfolio

b - Or you can open index.html in your browser. (right-click on index.html file->open with->Chrome/Firefox/Safari)

List of optimizations:

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
