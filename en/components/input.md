---
title: Input - Design System Component
_description: The Input Component Symbol allows the collection of user data such as strings, numbers and dates.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

## Input

Use the Input Component to collect user data such as strings and numbers fitting various contexts, dates, and other values. Multiple inputs can be combined to craft easy-to-use and aesthetic forms. The Input is visually identical to the [Ignite UI for Angular Input Group Component](https://www.infragistics.com/products/ignite-ui-angular/angular/components/input_group.html)

### Input Demo

<img src="../images/input_demo.png" srcset="../images/input_demo@2x.png 2x" />

### Types

The Input comes with or without a helper text and provides choice between three distinct types, e.g. line style for a more airy style or border style for a more structured perception on solid color backgrounds. The boxed style is most appropriate when the Input is placed on top of an vivid image to improve readability of its content.

<img src="../images/input_no-helper.png" srcset="../images/input_no-helper@2x.png 2x" />
<img src="../images/input_helper.png" srcset="../images/input_helper@2x.png 2x" />

<img src="../images/input_line.png" srcset="../images/input_line@2x.png 2x" />
`line`

<img src="../images/input_box.png" srcset="../images/input_box@2x.png 2x" />
`box`

<img src="../images/input_border.png" srcset="../images/input_border@2x.png 2x" />
`border`

<img src="../images/input_search.png" srcset="../images/input_search@2x.png 2x" />
`search`

### Variants

The Input can be used styled in **dark** and light variants to assure good readability and contrast for both lighter and darker backgrounds.

<img src="../images/input_dark.png" srcset="../images/input_dark@2x.png 2x" />
<img src="../images/input_light.png" srcset="../images/input_light@2x.png 2x" />

### State

When the user interacts with the Input, it goes through various states: **idle** with a placeholder in the place of the content, focused while the user is typing in it, filled once the user has finished adding content and moved on, and disabled when the input does not support any interaction. These flexibility enhancements afford a more dynamic interaction design that can seamlessly flow into high-fidelity prototyping.

<img src="../images/input_idle.png" srcset="../images/input_idle@2x.png 2x" />
`idle`

<img src="../images/input_focused.png" srcset="../images/input_focused@2x.png 2x" />
`focused`

<img src="../images/input_filled.png" srcset="../images/input_filled@2x.png 2x" />
`filled`

<img src="../images/input_disabled.png" srcset="../images/input_disabled@2x.png 2x" />
`disabled`

Every experienced designer uses constraints wisely to limit the user input and avoid invalid states, hence the availability of validation styles. Through the available validation styles, the Input is equipped for sophisticated designs that display success, warning, and error visuals.

<img src="../images/input_success.png" srcset="../images/input_success@2x.png 2x" />
<img src="../images/input_warning.png" srcset="../images/input_warning@2x.png 2x" />
<img src="../images/input_error.png" srcset="../images/input_error@2x.png 2x" />

### Layout

The Input has rich support for prefix and suffix through text string or icon that can, in certain cases, reduce the input effort for the user: e.g. an @email.com suffix means both less keystrokes and more clarity of expected content, while a clock or calendar prefix may indicate that the Input is suitable to provide time or date as content.

<img src="../images/input_prefix.png" srcset="../images/input_prefix@2x.png 2x" />
<img src="../images/input_suffix.png" srcset="../images/input_suffix@2x.png 2x" />

> [!Note]
> ↳ Layout
>
> - .../OnlyText/...
> - .../Prefix + Suffix/Icons/...
> - .../Prefix + Suffix/String/...
> - .../Suffix/Icons/...
> - .../Suffix/String/...

### Date Picker and Time Picker Inputs

These two are special types of Input customized for the purposes of date and time selection. They have a consistent structure with the other Inputs, but the layout, which is fixed in a certain way for each state. The icons that appear at the prefix location are set to the Material Icons `calendar-today` and `access-time` and can not be changed via the overrides panel.

<img src="../images/input_calendar.png" srcset="../images/input_calendar@2x.png 2x" />
<img src="../images/input_time-picker.png" srcset="../images/input_time-picker@2x.png 2x" />

### Styling

The Input comes with styling achievable through changing the primary, success, warning, and error colors of your theme in the Styling library.

<img src="../images/input_styling.png" srcset="../images/input_styling@2x.png 2x" />

## Usage

Use the box type of Input when placing forms on top of an image to improve readability. When using an Input in warning or error state in your designs, prefer the one with helper text and use the opportunity to provide guidance to the user.

| Do                                                                           | Don't                                                                            |
| ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| <img src="../images/input_do1.png" srcset="../images/input_do1@2x.png 2x" /> | <img src="../images/input_dont1.png" srcset="../images/input_dont1@2x.png 2x" /> |
| <img src="../images/input_do2.png" srcset="../images/input_do2@2x.png 2x" /> | <img src="../images/input_dont2.png" srcset="../images/input_dont2@2x.png 2x" /> |

## Code generation

This section describes some important overrides and how they affect code generation.

> [!WARNING]
> Triggering `Detach from Symbol` on an instance of the Input in your design is very likely to result in loss of code generation capability for the Input.

### Event Property

When supplied the `🕹️Event` property is used to create a method in the component TypeScript and add an Angular click signature in the HTML for the input’s icons. When supplied the event must be specified using the curly braces format: {onEventName}.

This property is currently only supported on the Searchbar component. The Searchbar can have two icons and each icon has an `🕹️Event` property that can be set.

### Data Property

When supplied, the `🕹️DataProperty` value is used to set up a two-way [data binding](../codegen/data-binding.md) using [Angular Reactive Forms](https://angular.io/guide/reactive-forms) to the input value property. The `🕹️DataProperty` is optional however when provided, it will be the name of the property on the data object specified by the model object name provided during code generation. As such, it is required that if the `🕹️DataProperty` is used that the developer must specify a model object name otherwise it will be ignored.

### Inputs Date and Time

Currently the theme and color values assigned in Sketch are not part of the generated code because Ignite UI for Angular does not provide theming support for these types of Inputs yet.

### Inputs (Except Searchbar, Date and Time)

#### Layout

Determines the layout of the Input Group. When set to display Prefix and/or Suffix, text or icons can be displayed at the corresponding ends of the Input.

#### Label

Determines the text to be displayed in the Label.

#### Input Text

Determines the text to display in the Input value. If the `🕹️DataProperty` is set this is ignored. In the Line, Box, or Border Inputs if this field contains only `*` characters the type of the input will be set to password.

#### Help Text

Determines the text to be displayed in the Hint of the Input Group. Date Picker and Time Picker do not support this.

### Searchbar

The Searchbar has Left and Right Icons that can be turned on/off individually and each have an Event that can be assigned. The Searchbar has a Search Hint that displays in the label of the Searchbar.

### Text Values

The above Label, Input, Help Text, and Search Hint properties may contain text, [binding text](../codegen/data-binding.md), or a combination of the two, examples:

- Settings
- {settingsLabel}
- Important {labelText}

## Additional Resources

Related topics:

- [Form Pattern](../patterns/form.md)
- [User Profile Pattern](../patterns/user-profile.md)
- [Data Binding](../codegen/data-binding.md)
  <div class="divider--half"></div>

Our community is active and always welcoming to new ideas.

- [Indigo Design **GitHub**](https://github.com/IgniteUI/design-system-docfx)
