% zdk-float-panel  
% zedesk.net
% May 2014

zdk-float-panel
===============

This component create a floating panel with a title bar. The component use the [polymer library](http://www.polymer-project.org) as backend.

To use it, install the compoent with the bower command : `bower install zdk-float-panel -S`

in the head of your html file :

```
<script src="bower_components/platform/platform.js"></script>
<link rel="import" href="zdk-float-panel.html">
```

Then in the body of your html page :

```
<zdk-float-panel heading="<heading>" x="20" y="20">
    <!-- insert your content here -->
</zdk-float-panel>
```

## Attributes

The zdk-float-panel component could have the following attributes :

  - __heading__ : the title of the panel
  - __x__ : the x coordinate of the panel
  - __y__ : the y coordiante of the panel
  
The panel is displayed with absolute coordinates (x,y) on the web page.

These attributes are accessible programmatically :

```javascript
var panel = document.querySelector("zdk-float-panel");
panel.activate();
panel.x = 300; panel.y = 400;
panel.heading = "New title";
```

## Methods

the __activate__ method allow to display the selected panel on top of all elements of your page.

## Compatibility

This component works on desktep browser, but also on mobile devices, like android tablets ( tested on my nexus7 with chrome ).

| Browser           | status    |
|:------------------|:---------:|
| Chrome            | OK        |
| Firefox           | OK        |
| Android (Chrome)  | OK        |
| IOS ( Simulator ) | OK        |
