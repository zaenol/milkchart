The pie chart will draw a circle with the different rows as percentages of the circle.  This will only transform the first column of the tab;e supplied and ignore any others.

![http://www.brettdixon.com/static/pie.jpg](http://www.brettdixon.com/static/pie.jpg)

# Syntax #

```
var chart = new MilkChart.Pie(table[, options])
```

# Arguments #

  1. table - (mixed) a table Element (or its id) that should be transformed
  1. options - (object, optional) a key/value set of options

# Options #

  * stroke - (bool Defaults to true) Stroke the pie chart
  * strokeWeight - (int: Defaults to 2) Stroke weight in px
  * strokeColor - (string: Defaults to "#000000") Font color on pie slices
  * shadow - (bool: Defaults to false) Draw a shadow under the pie chart
  * showPercentages - (bool: Defaults to true) Draw slice percentage
  * chartLineWeight - (int: Defaults to 2) Outline line weight in px
  * pieBorder - (bool: Defaults to false) Draw a border around pie