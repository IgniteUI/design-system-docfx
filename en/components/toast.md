---
title: Toast - Design System Component
_description: The Toast Component Symbol is used to show a non-interactive information message or notification.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

## Toast

Use the Toast Component to show a short information message or notification, which is neither interactive nor possible to dismiss by the user. The Toast should be hidden automatically after a defined time interval. The Toast is visually identical to the [Ignite UI for Angular Toast Component](https://www.infragistics.com/products/ignite-ui-angular/angular/components/toast.html)

### Toast Demo

![](../images/toast_demo.png)

### Position

The Toast should be relatively positioned towards the bottom, center, or top of the content its information concerns.

![](../images/toast_bottom.png)
![](../images/toast_center.png)
![](../images/toast_top.png)

### Styling

The Toast comes with constrained styling possibility, allowing only control of the background and message text colors. However, it is highly advisable to choose between `white` and `grays.900` for the message text, whichever of the two gives better contrast with the background.

![](../images/toast_styling.png)

## Usage

The Toast should always be centrally aligned on the horizontal and other placements should be avoided. Approach the Toast styling with care, avoiding too distinct background colors and message text color that is neither white nor dark gray or black.

| Do                           | Don't                          |
| ---------------------------- | ------------------------------ |
| ![](../images/toast_do1.png) | ![](../images/toast_dont1.png) |
| ![](../images/toast_do2.png) | ![](../images/toast_dont2.png) |

## Code Generation

When colors are specified for the Toast, the Toast HTML element will be wrapped in a div. This is required by browsers to style a nested component (a component within another component).

> [!WARNING]
> Triggering `Detach from Symbol` on an instance of the Toast in your design is very likely to result in loss of code generation capability for the Toast.

### Data Bindings

Data bindings are specified by using curly brace syntax, example: {isAdmin}. Text fields (not `🕹️DataProperty` or `🕹️DataSource`) also support string interpolation syntax example: Admin: {isAdmin}. Data bindings can be non-nested or nested. If the target property is a nested property, include the nested property chain, but don’t include the model object name. Examples:

#### Not Nested

```typescript
Customer {
  imageName: String;
}
```

DataProperty would be: `{imageName}`

#### Nested

```typescript
Profile {
  imageName: String;
}

Customer {
  profile: Profile;
}
```

DataProperty would be: `{profile.imageName}`

### Data Property

When supplied, the `🕹️DataProperty` value is used to set up a data binding to the toast text property. The `🕹️DataProperty` is optional. The `🕹️DataProperty` is the name of the property on the data object specified by the model object name provided in the generation request. When supplied, this value overrides the Text property.

### Text

When supplied, the Text property may contain text, binding, or a combination of the two, examples:

- Settings
- {settingsLabel}
- Important {labelText}

## Additional Resources

Related topics:

Our community is active and always welcoming to new ideas.

- [Indigo Design **GitHub**](https://github.com/IgniteUI/design-system-docfx)
