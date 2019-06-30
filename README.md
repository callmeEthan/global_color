# Global controller
The SysColor plugin can read system color, however often return colors that are too dark or too light.
This skin would convert them back to a more colorful color, and apply to all skins in group ColorGroup (without refresh the skins).

## How this skin work
* A single skin with SysColor measure that check windows color, has no meter visually.
* Detect color change and convert them to HSV base color, increase the saturation and value for a brighten and preferable color.
* Convert output color back to RGB and set variable 'color' for skins in group "ColorGroup".
* Update skin measure/meter and redraw.

## How to use
* [SysColor](https://forum.rainmeter.net/viewtopic.php?t=14202) plugin is required (included in the .rmskin file)
* Firstly edit skin that need color update, under [Rainmeter] set Group=ColorGroup. (or add ColorGroup after "|" if skin already in a group)
* For meters that have color that need to update, set to use #Color# variable (not necessary predefined) and set DynamicVariables=1
* Refresh this skin or change system color (whether by changing background).

## Installation
* Get rainmeter
* Download .rmskin for easy install.

## Credit
HSV to RGB conversion code by [GigsD4X](https://gist.github.com/GigsD4X)
[Ethan](https://github.com/callmeEthan).  
