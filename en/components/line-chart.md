---
title: Line Chart - Design System Component
_description: The Line Chart Component Symbol shows data as a series of points connected by straight lines.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

# Line Chart

 A Line Chart is a type of category line graph that shows the continuous data values represented by points connected by straight line segments of one or more quantities over a period of time. It’s often used to show trends and perform comparative analysis. The Y-Axis (labels on left side) show a numeric value, while the X-Axis (bottom labels) show a time-series or comparison category. You can include one or more data sets to compare, which would render as multiple lines in the chart. The Line Chart is identical to the Spline Chart in all aspects except that the line connecting data points does not have spline interpolation and smoothing for improved presentation of data.


## Line Chart Demo

<img class="responsive-img" src="../images/line_chart_three_series.png" srcset="../images/line_chart_three_series@2x.png 2x" />

The Line Chart has Title, Legend and a Chart Area, which can be changed between two states - Idle and Hover, and where you can also change the Chart Type and its Series Amount.

## Title and Legend

The Line Chart has a title that can be changed or hidden if not needed. The Legend can also be hidden and it stands for the number of the series in the chart and what they represent. Individual series of the legend can also be turned off by setting them to No Symbol. Their color and symbol - rectangle, line or dot, can also be changed individually.

<img class="responsive-img" src="../images/line_chart_legend.png" srcset="../images/line_chart_three_legend@2x.png 2x" />

## Chart Type

This is where the chart can be switched between Line and Line Area Chart. The Area Chart is the same as the Line, but the area between the X axis and the line itself is filled in the series's color. The area chart is used best to represent how big of a change there is and what the trend is over time.

<img class="responsive-img" src="../images/line_area_chart_three_series.png" srcset="../images/line_area_chart_three_series@2x.png 2x" />

## Tooltip

The Line Chart comes with an override for the tooltip visibility: **Tooltip Off** hides it and Tooltip On shows it on top of the series.

<img class="responsive-img" src="../images/line_chart_tooltip-off.png" srcset="../images/line_chart_tooltip-off@2x.png 2x" />
<img class="responsive-img" src="../images/line_area_chart_tooltip-off.png" srcset="../images/line_area_chart_tooltip-off@2x.png 2x" />
<img class="responsive-img" src="../images/line_chart_tooltip-on.png" srcset="../images/line_chart_tooltip-on@2x.png 2x" />
<img class="responsive-img" src="../images/line_area_chart_tooltip-on.png" srcset="../images/line_area_chart_tooltip-on@2x.png 2x" />

## Axis and Gridlines

Aside from being able to change the labels, you can also change the axis' color, ticks' color and also the gridlines. The Y axis title can be hidden by deleting its content.

<img class="responsive-img" src="../images/line_chart_axis.png" srcset="../images/line_chart_axis@2x.png 2x" />

## Line and Points

The line and points' color on the chart can be changed if it's needed so they match the color of the series.

<img class="responsive-img" src="../images/line_chart_colors.png" srcset="../images/line_chart_color@2x.png 2x" />

## Series Amount

This override provides flexibility to select between one, two and **three** series that will be rendered. They can also be changed for the Line Area Chart type.

<img class="responsive-img" src="../images/line_chart_one_series.png" srcset="../images/line_chart_one_series@2x.png 2x" />
<img class="responsive-img" src="../images/line_chart_two_series.png" srcset="../images/line_chart_two_series@2x.png 2x" />
<img class="responsive-img" src="../images/line_chart_three_series.png" srcset="../images/line_chart_three_series@2x.png 2x" />

<img class="responsive-img" src="../images/line_area_chart_one_series.png" srcset="../images/line_area_chart_one_series@2x.png 2x" />
<img class="responsive-img" src="../images/line_area_chart_two_series.png" srcset="../images/line_area_chart_two_series@2x.png 2x" />
<img class="responsive-img" src="../images/line_area_chart_three_series.png" srcset="../images/line_area_hart_three_series@2x.png 2x" />

## Styling

The Line and Area Line Chart's color of the series, dots and area can be easily changed and also border and background color.

<img class="responsive-img" src="../images/line_chart_styling.png" srcset="../images/line_chart_styling@2x.png 2x" />

## Usage

Use the Line Chart when you have a continuous data set and want to see the amount of change over a period of time. If you use time to represent the change in the category you should always set it on the horizontal axis. Always start the Y-Axis (left or right axis) at 0 so data comparison is accurate and order time-series data from left to right. Use proper aspect ratio to minimize dramatic slope drops.


/* | Do                                                                                             | Don't                                                                                              |
| ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| <img class="responsive-img" src="../images/line_chart_do1.png" srcset="../images/line_chart_do1@2x.png 2x" /> | <img class="responsive-img" src="../images/line_chart_dont1.png" srcset="../images/line_chart_dont1@2x.png 2x" /> | */

## Additional Resources

Related topic:

- [Data Binding](../codegen/data-binding.md)
  <div class="divider--half"></div>

Our community is active and always welcoming to new ideas.

