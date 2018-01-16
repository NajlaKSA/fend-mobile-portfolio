[Original Project](https://github.com/udacity/frontend-nanodegree-mobile-portfolio)
========================
## Optimizing website:
after optimiziation the pagespeed insight's score is over 90.
[website after optimization in page speed insight](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fnajlaksa.github.io%2Ffend-mobile-portfolio&tab=mobile)

I did this by changing:
* inline style within html doc.
* resricted _print.css_ to the printing screen only using media attribute.
check the result out.


[demo](https://najlaksa.github.io/fend-mobile-portfolio/index.html)

## Pizza.html:
Time to resize pizzas is less than 5 ms thanks to:
* reducing the number of pizzas loaded to the  (from 200 to 25) .
* replaced _querySelector_ with _getElementById_ or _getElementByClassName_ [it's significantly faster](https://jsperf.com/getelementsbyclassname-vs-queryselectorall/18)
* moved unnecessary code lines out of the loop in _updatePosition()_.

[Demo](https://najlaksa.github.io/fend-mobile-portfolio/views/pizza.html)