---
title: Indigo Design App Builder - Change Log 
_description: Indigo Design App Builder enables design and development teams to use various interactions when creating connections between screens and components in order to cover real application scenarios.
_keywords: App Builder, Web App Builder, Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch UI kits, Interactions
---
# Indigo Design App Builder - Change Log 

> [!NOTE]
><b>Latest update was made on July 12th, 2021.

## July 12, 2021 Release

### Features
* **GitHub Integration**: Publish your generated app to a GitHub repository instead of downloading as a ZIP
* Added “SLIDER” to the component toolbox
* Added “BANNER” to the component toolbox
* Added two new sample apps as reference in “Create new app” dialog
* Added Korean language translation

### Improvements
* When previewing an app, switch between "master" and "child views" using a dropdown in the toolbar
* Ability to reorder components in the document outline or design surface using drag & drop
* Ability to reorder “master” and “child views” in the views tab of the toolbox using drag & drop
* Updated “Radio” component to “Radio-group”
* Updated “Tab Layout” to allow custom content inside “Tab header”
* Improved icons for "align-content" dropdown when wrapping is enabled in Flex layouts
* Apps are generated using Ignite UI Angular v12.0.1 instead of v11.1.15

### Maintenance updates & bug fixes
* Improved load times and performance tweaks when using the App Builder UI
* General bug fixes

## Official Release

### General
* Cloud integration and team collaboration - accessing the App Builder can be done through the <b>App tab in Indigo.Design cloud</b>, where users will find their active application projects. From there, users are enabled to start a new app or to preview, rename, archive or duplicate an existing one
* Using <b>a Sketch file</b> as a starting point for a new application in the App Builder - now, users are enabled to start a new application from an existing <b>Sketch file</b> by uploading it in the App Builder. 

### UI components
* Dialog
* Combo
* Tabs layout
* Expansion panel
* Date time editor (as an input type)
* Button group
* Text area
* Hyperlink

### Interactions
* Open/Close - "Open/Close" interaction enables users create interactions using overlay components, such as <b>a dialog component</b>.
* Show/Hide - "Show/Hide" is an interaction that can be applied to a component to show and hide another component visibility in the same view.

### Using Data in the App Builder
* Data sources -  enables users to upload their own JSON file or provide a Rest API URL with the data source. The added data source can be used also in the repeaters to connect components to actual data source fields.

### Code Generation
* General improvements and bug fixes

## Public Release

### General
* Option to set <b>min and max width and height</b> for layouts
* More components and layouts size units - the newly added units are <b>auto min, auto max, px, rem, vh, vw, %</b>.
* New layout position options - the newly added positioning options are <b>relative, absolute, fixed, sticky and overflow</b>, which can be applied to components and layouts.
* Quick add shortcut for components through <b>Ctrl/Cmd + E</b>​
* Error handling service​ improvements
* Quick app preview on various devices​ - when previewing an app project, users can quickly preview it on various viewports through the device icons in the top bar.
* Appearance and border options for components​
* Initial concurrency version is implemented​
* Sample apps library extended - the components in this release were used to enrich the existing sample apps.

### UI components
* Dropdown
* Select
* Chip
* Navigation drawer
* Navigation bar​

### Using Data in the App Builder
* Repeaters feature - enables users to connect a component to a data source field.
* Binding to a mock data -  enables users to try the data binding and repeaters with data features using a mockup Northwind data.

### Code Generation
* General improvements and bug fixes


## Private Release

### General
* Interactive flows - the interactive flows feature has been extended with master and child views routing.
* Preset layouts - 4 predefined layouts for quick start of a new design have been added.
* Library of sample apps - 3 predefined sample apps have been added which users can use as a starting point to speed up the design process or quickly learn how Indigo.Design App Builder works
* General improvements and bug fixes
* Visual improvements and user experience enhancement

### Themeing Service
* Theme presets - 6 predefined themes have been added for dark and light versions of <b>Material, Bootstrap and Fluent</b>.
* Adding new custom themes feature - users are enabled to create custom themes aligned with the brand assets and design system of their company.


### UI components
* Absolute Layout 
* Row Layout 
* Column Layout 
* Card
* Views Container
* Avatar
* Calendar
* Icon
* Image
* Text
* Title
* Button
* Checkbox
* Date picker
* Floating Action Button 
* Icon Button
* Input Group
* Radio
* Switch
* Grid
* Badge

### Code Generation
* General improvements and bug fixes

## Additional Resources

<div class="divider--half"></div>


* [Getting Started](getting-started.md)
* [Indigo Design App Builder Components](indigo-design-app-builder-components.md)
* [Interactions](interactions.md)
* [Using data in the Indigo Design App Builder](using-data-in-your-app.md)