---
title: Step Line Chart - Design System Component
_description: The Step Line Chart Component Symbol shows data as a series of points connected by straight lines, resembling steps.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

# Step Line Chart

Step Line Chart belongs to a group of category charts and it is rendered using a collection of points connected by continuous vertical and horizontal lines forming a step-like progression. Values are represented on the Y-axis while the X-Axis (labels at the bottom) shows a time-series or comparison category. The Step Line series emphasize the amount of change over a period of time or compares multiple items. The Step Line Chart is identical to the Step Area Chart in all aspects except that the area below the step lines is not filled in. The Step Line Chart is useful when showing changes that occur at irregular intervals. You can include one or more data sets to compare, which would render as multiple lines in the chart.


## Step Line Chart Demo

<img class="responsive-img" src="../images/step_line_chart_demo.png" srcset="../images/step_line_chart_demo@2x.png 2x" />

The Step Line Chart has Title, Legend, and Chart Area, where you may choose between two states Idle and Hover. It also supports two chart types: Line and Area with a number of Series Amount configurations and allows to adjust the Legend accordingly.

## Title

The Step Line Chart has a title that when not needed can be removed by setting its override to ~No Symbol.

<img class="responsive-img" src="../images/step_line_chart_title.png" srcset="../images/step_line_chart_title@2x.png 2x" />

## Legend

The Step Line Chart comes with a Legend to show the number of series in it and what they represent. The Legend is built using a Smart Layout in Sketch and can be adjusted to contain the exact amount of series items by setting the overrides of those not needed to ~No Symbol. Legend items' shape is also configurable with built-in support for rectangle, line, and dot.

<img class="responsive-img" src="../images/step_line_chart_legend.png" srcset="../images/step_line_chart_legend@2x.png 2x" />

## Chart Type

The Chart Type allows switching between Line and Area. The latter one has the area between the X-axis and the Step Line filled with the series' color. Area charts are used to represent how big of a change there is and what the trend is over time.

<img class="responsive-img" src="../images/step_area_chart_three_series.png" srcset="../images/step_area_chart_three_series@2x.png 2x" />

## State

The Step Line Chart has two states - Idle and Hover. In the Hover state a tooltip, giving information about the series' values at this point, is shown upon hovering over a data point.

<img class="responsive-img" src="../images/step_area_chart_tooltip-off.png" srcset="../images/step_area_chart_tooltip-off@2x.png 2x" />
<img class="responsive-img" src="../images/step_area_chart_tooltip-on.png" srcset="../images/step_area_chart_tooltip-on@2x.png 2x" />

## Y-Axis

The Y-axis of the Step Line Chart comprises of a Title, Labels, and the Axis itself. The Title and the Labels are configurable and to hide a label simply set its override to ~No Symbol. You may hide the axis line by setting its color to `Transparent` and to hide all elements at once, change the Y-axis override to ~No Symbol.

<img class="responsive-img" src="../images/step_line_chart_yaxis.png" srcset="../images/step_line_chart_yaxis@2x.png 2x" />

## Gridlines

The Step Line Chart has vertical and horizontal built-in Gridlines to make it easier to visually trace a data point to the X and Y-axis. Both are configurable individually and to hide any or both of them just set their color to `Transparent`.

<img class="responsive-img" src="../images/step_line_chart_gridlines1.png" srcset="../images/step_line_chart_gridlines1@2x.png 2x" />
<img class="responsive-img" src="../images/step_line_chart_gridlines2.png" srcset="../images/step_line_chart_gridlines2@2x.png 2x" />

## Series Amount

The Step Line Chart comes with a selection of one, two, and **three** series that will be rendered in the Chart Area. This is also valid for the Area type.

<img class="responsive-img" src="../images/step_line_chart_one_series.png" srcset="../images/step_line_chart_one_series@2x.png 2x" />
<img class="responsive-img" src="../images/step_line_chart_two_series.png" srcset="../images/step_line_chart_two_series@2x.png 2x" />
<img class="responsive-img" src="../images/step_line_chart_three_series.png" srcset="../images/step_line_chart_three_series@2x.png 2x" />

## Styling

First and foremost, the Step Line Chart lets you change the color of the series. It is recommended to use only colors from the palette for data visualizations with nuances named series.1, series.2 and so on till series.10. You may also change the colors of the vertical and horizontal axis, the gridlines, as well as the chart area background and border colors. Titles, labels, annotation values etc. are also customizable via the available text styles in the **Indigo.Design System**.

<img class="responsive-img" src="../images/step_line_chart_styling.png" srcset="../images/step_line_chart_styling@2x.png 2x" />

## Usage

Use the Step Line Chart when you have a continuous data set and want to see the amount of change over a period of time. If you use time to represent the change in the category you should always set it on the horizontal axis. Always start the Y-Axis at 0 so data comparison is accurate and order time-series data from left to right. Use proper aspect ratio to minimize dramatic slope drops. When there is more than one series in the chart they should use different colors to be distinguishable. Using a legend to signify what they represent is considered to be best practice.


| Do                                                                                             | Don't                                                                                              |
| ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| <img class="responsive-img" src="../images/step_line_chart_do1.png" srcset="../images/step_line_chart_do1@2x.png 2x" /> | <img class="responsive-img" src="../images/step_line_chart_dont1.png" srcset="../images/step_line_chart_dont1@2x.png 2x" /> | 

## Additional Resources

Related topic:

- [Line Chart](../line-chart.md)
- [Spline Chart](../spline-chart.md)
- [Column Chart](../column-chart.md)
- [Skeleton Charts](../skeleton-charts.md)

Our community is active and always welcoming to new ideas.
