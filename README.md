~$ man svg2poly

__NAME__

svg2poly - import Simple SVG files as polygons in Eagle CAD
 

__SYNOPSIS__

svg2poly [options]

 
__DESCRIPTION__

There are currently a few Eagle ULPs that can import images into PCBs, but they can be fairly confusing to use. Furthermore, by having to convert to bitmaps, resolution is lost when the file is imported to the PCB.

svg2poly is a program that reads Simple SVG files and outputs polygons onto the PCB, in one simple step. Scaling the image, changing the layer, and even adding a line border are made easy by passing parameters to the script. 


__INSTRUCTIONS__

The script was made to handle Simple SVG files from Inkscape. When I was working on it, I found the SVG spec to be incredibly complicated, and non-coherent. Along with having to write my own stack for recursion (the scripting language isn't the powerful), I was only ever able to import Text in a very specific way.

If you're still interested in using the script, read on.

_Inkscape_
* Type out the text that you want. Format it and such.
* Lock the height/width ratio
* Change height to 100 (this helps with changing the ratio)
* *Ctrl-Shift-C* (Object to Path)
* Select all (w/ Node Cursor)
* Extensions > Modify Path > Add Nodes (Default settings are alright)
* Extensions > Modify Path > Flatten Beziers (Default settings are alright)
* For the closed loop letters O,o,D,d,etc...
*   Draw a rectangle dividing the letter ( O => ([)] )
*   Select the rectangle and the letter
*   *Ctrl-/* (Division)
*   Repeat with all closed letters
* Select all (w/ Node Cursor)
* *Ctrl-Shift-K* (Break Apart)
* Save As > Simple SVG

_Eagle_ 
* Open your .BRD file
* Type *mark*
* With your mouse, select where you want the center of the svg to appear
* Enter command and browse to svg file

 
__OPTIONS__

Defaults are *-ratio 1.0 -layer tDocu -outline 0*

-ratio *number*

&nbsp;&nbsp;&nbsp;&nbsp;Change the X and Y ratio of the imported file. This number can be negative.

-ratiox *number*

&nbsp;&nbsp;&nbsp;&nbsp;Change the X ratio of the imported file. This number can be negative.

-ratioy *number*

&nbsp;&nbsp;&nbsp;&nbsp;Change the Y ratio of the imported file. This number can be negative.

-layer *name*

&nbsp;&nbsp;&nbsp;&nbsp;Change the layer that the polygin is made in. This should be the name of the layer.

-outline *width*

&nbsp;&nbsp;&nbsp;&nbsp;Change the width of the outline.

    
__AUTHOR__

Written by Cruz Monrreal II