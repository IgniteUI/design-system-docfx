---
title: Category Chart - Design System Component
_description: The Category Chart Component Symbol provides simple visual representations for dense complex data.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

## Category Chart

Use the Category Chart Component to wrap the density and complexity of data in a simple visual. Category Charts are often combined to create beautiful dashboards for related sets of data. The Category Chart is visually identical to the [Ignite UI for Angular Category Chart Component](https://www.infragistics.com/products/ignite-ui-angular/angular/components/categorychart.html)

### Category Chart Demo

<img class="responsive-img" src="../images/chart_category_demo.png" srcset="../images/chart_category_demo@2x.png 2x" />

### Tooltip

The Category Chart comes with an override for the tooltip visibility: **Tooltip Off** hides it and Tooltip On shows it on top of the series.

<img class="responsive-img" src="../images/chart_category_tooltip-off.png" srcset="../images/chart_category_tooltip-off@2x.png 2x" />
<img class="responsive-img" src="../images/chart_category_tooltip-on.png" srcset="../images/chart_category_tooltip-on@2x.png 2x" />

### Types

The Category Chart comes with flexibility for selecting the Chart type through various overrides such as:

|             |                                                                                                                |
| ----------- | -------------------------------------------------------------------------------------------------------------- |
| Area        | <img class="responsive-img" src="../images/chart_category_area.png" srcset="../images/chart_category_area@2x.png 2x" />               |
| Column      | <img class="responsive-img" src="../images/chart_category_column.png" srcset="../images/chart_category_column@2x.png 2x" />           |
| Line        | <img class="responsive-img" src="../images/chart_category_line.png" srcset="../images/chart_category_line@2x.png 2x" />               |
| Point       | <img class="responsive-img" src="../images/chart_category_point.png" srcset="../images/chart_category_point@2x.png 2x" />             |
| Spline      | <img class="responsive-img" src="../images/chart_category_spline.png" srcset="../images/chart_category_spline@2x.png 2x" />           |
| Spline Area | <img class="responsive-img" src="../images/chart_category_spline-area.png" srcset="../images/chart_category_spline-area@2x.png 2x" /> |
| Step Area   | <img class="responsive-img" src="../images/chart_category_step-area.png" srcset="../images/chart_category_step-area@2x.png 2x" />     |
| Step Line   | <img class="responsive-img" src="../images/chart_category_step-line.png" srcset="../images/chart_category_step-line@2x.png 2x" />     |
| Waterfall   | <img class="responsive-img" src="../images/chart_category_waterfall.png" srcset="../images/chart_category_waterfall@2x.png 2x" />     |

### Series Amount

This override provides flexibility to select between one and **three** series that will be rendered.

<img class="responsive-img" src="../images/chart_category_one_series.png" srcset="../images/chart_category_one_series@2x.png 2x" />
<img class="responsive-img" src="../images/chart_category_two_series.png" srcset="../images/chart_category_two_series@2x.png 2x" />
<img class="responsive-img" src="../images/chart_category_three_series.png" srcset="../images/chart_category_three_series@2x.png 2x" />

## Usage

Even though you might need to combine different types of series in the same chart, you should avoid stacking multiple Category Charts on top of one another. Use the Category Chart Component as if it were a simplified stencil for data visualization.

| Do                                                                                             | Don't                                                                                              |
| ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| <img class="responsive-img" src="../images/chart_category_do1.png" srcset="../images/chart_category_do1@2x.png 2x" /> | <img class="responsive-img" src="../images/chart_category_dont1.png" srcset="../images/chart_category_dont1@2x.png 2x" /> |

## Code Generation

This section describes some important overrides and how they affect code generation.

> [!WARNING]
> Triggering `Detach from Symbol` on an instance of the Category Chart in your design is very likely to result in loss of code generation capability for the Category Chart.

### Data Source Property

When supplied, the `🕹️DataSource` value is used to set up a [binding](../codegen/data-binding.md) to the chart dataSource property. Without a `🕹️DataSource` and valid data in the data source, the Category Chart cannot render at runtime.

### Chart Dimensions

The Category Chart will generate with fixed dimensions obtained within the Sketch. The developer can then modify these dimensions as they see fit within the HTML. Valid values for the width and height are pixel values and percent values. Examples:

width=”300px” or width=”100%”

### Chart Type

Configures the chart to use the provided series type. When Type is None, the chart will not render.

### Chart Title

The Title property may contain text, [binding text](../codegen/data-binding.md), or a combination of the two, examples:

- Settings
- {settingsLabel}
- Important {labelText}

The Title is optional.

## Additional Resources

Related topic:

- [Data Binding](../codegen/data-binding.md)
  <div class="divider--half"></div>

Our community is active and always welcoming to new ideas.


