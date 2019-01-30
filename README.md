# Global controller
Idea was to create a method to match the color of multiple skin, without using too many code.

## How this skin work
* Have a single skin with SysColor measure that update windows color, has no meter visually.
* Detect color change and convert them to HSV base color, increase the saturation and value for a brighten and preferable color.
* Convert output color back to RGB and set variable 'color' on group skins.
* Update skin measure/meter and redraw.

## Requirement
* Set Group=ColorGroup in [Rainmeter] for group bangs to work
* Meter must use a #color# variable and has DynamicVariables=1

HSV to RGB conversion code by [GigsD4X](https://gist.github.com/GigsD4X)
## Authors
[Ethan (Finch)](https://github.com/callmeEthan).  
