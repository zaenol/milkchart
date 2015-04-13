The base class used for all Milk Charts.  It is meant to be an abstract class, but will default to Column if used by itself.  Please see below for all chart types available.

# Syntax #

```
<script type="text/javascript" src="mootoolsCore.js"></script>
<script type="text/javascript" src="MilkChart.js"></script>

<script type="text/javascript">
    window.addEvent('domready', function() {
        var chart = new MilkChart(table[, options]);
    })
</script>

<!-- Table structure -->
<table id="chart">
    <thead>
        <tr>
            <th>Column A</th><th>Column B</th><th>Column C</th><th>Column D</th>
        </tr>
    </thead>
    <tbody>
        <tr><td>8.3</td><td>70</td><td>10.3</td><td>100</td></tr>
        <tr><td>8.6</td><td>65</td><td>10.3</td><td>125</td></tr>
        <tr><td>8.8</td><td>63</td><td>10.2</td><td>106</td></tr>
        <tr><td>10.5</td><td>72</td><td>16.4</td><td>162</td></tr>
        <tr><td>11.1</td><td>80</td><td>22.6</td><td>89</td></tr>
    
    </tbody>
    <tfoot>
        <tr>
            <td>Row 1</td><td>Row 2</td><td>Row 3</td><td>Row 4</td><td>Row 5</td>
        </tr>
    </tfoot>
</table>
```

  * Note: This script will default to the [Column](Column.md) type graph
  * Note: The `tfoot` is not required but MilkChart uses this to gather row names.  If the `<table>` does not have a `<tfoot>` then no row names are shown

# Arguments #

  1. table - (mixed) a table Element (or its id) that should be transformed
  1. options - (object, optional) a key/value set of options

# Options #

  * width - (int: Defaults to 400) Width of chart in px
  * height - (int: Defaults to 280) Height of chart in px
  * padding - (int: Defaults to 12) Outer padding of chart in px
  * font - (string: Defaults to "Verdana") Font to be used for labels
  * fontColor - (string: Defaults to #000000) Color used for labels
  * fontSize - (int: Defaults to 10) Font size in pt
  * background - (string: Defaults to #ffffff) Background color of chart
  * chartLineColor - (string: Defaults to #333333) Color of value lines
  * chartLineWeight - (int: Defaults to 1) Line Wieght of value lines in px
  * border - (bool: Defaults to true) Draws a border around edge chart (ignores padding)
  * borderWeight - (int: Defaults to 1) Border width in px
  * borderColor - (string: Defaults to #333333) Border color
  * titleSize - (int: Defaults to 18) Size of title font in pt
  * titleFont - (string: Defaults to "Verdana") Font used for title
  * titleColor - (string: Defaults to #000000) Font color for title
  * showRowNames - (bool: Defaults to true) Show the row labels on one of the axes
  * showValues - (bool: Defaults to true) Show values on one of the axes
  * showKey - (bool: Defaults to true) Shows the column labels
  * useZero - (bool: Defaults to true) Always use 0 as the lowest value
  * useFooter - (bool: Defaults to true) Get row labels from table footer

# Classes #

  * [Column](Column.md)
  * [Bar](Bar.md)
  * [Line](Line.md)
  * [Scatter](Scatter.md)
  * [Pie](Pie.md)