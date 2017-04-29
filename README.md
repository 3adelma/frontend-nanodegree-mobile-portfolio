Website Performance Optimization portfolio project

Live version

A live version of the website can be found on 
https://3adelma.github.io/frontend-nanodegree-mobile-portfolio/index.html


Changes

####index.html, project-2048.html, project-mobile.html, project-webperf.html Inlined all style sheets Created local copies of images and thumbnails, resized images too large Made script calls async Closed off

container
####Pizza.html Resized pizzeria.jpg

####Main.js

Added size of pizzaImage in pizzaElementGenerator

Optimized changePizzaSizes Moved new width claculation outside of loop, needs to be calculated only once since all pizzas are the same size Replaced document.querySelectorAll(".randomPizzaContainer") with variable reference to all generated pizzas

Optimized randompizza appending loop Moved randomPizza reference outside of loop so it is not recalculated Added variable to store reference to all random pizzas so change pizza size does not have to recalculate

Optimized function updatePositions() Storing all moving pizzas in var items outside of function

Optimized document.addEventListener('DOMContentLoaded', function() {} Optimized algorithm to generate scrolling pizzas to produce only 32 elements instead of 200 Changed elem.src to prescaled image Floored the value of width