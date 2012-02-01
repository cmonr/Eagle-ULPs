~$ man svg2poly

__NAME__

svg2poly - import Simple SVG files as polygons in Eagle CAD
 

__SYNOPSIS__

svg2poly [options]

 
__DESCRIPTION__

There are currently a few Eagle ULPs that can import images into PCBs, but they can be fairly confusing to use. Furthermore, by having to convert to bitmaps, resolution is lost when the file is imported to the PCB.

svg2poly is a program that reads Simple SVG files and outputs polygons onto the PCB, in one simple step. Scaling the image, changing the layer, and even adding a line border are made easy by passing parameters to the script. 

 
__OPTIONS__

Defaults are *-ratio 1.0 -layer tDocu -outline 0*

-ratio *number*<br/>
    Change the X and Y ratio of the imported file. This number can be negative.<br/>
-ratiox *number*<br/>
    Change the X ratio of the imported file. This number can be negative.<br/>
-ratioy *number*<br/>
    Change the Y ratio of the imported file. This number can be negative.<br/>
-layer *name*<br/>
    Change the layer that the polygin is made in. This should be the name of the layer.<br/>
-outline *width*<br/>
    Change the width of the outline.<br/>

    
__AUTHOR__

Written by Cruz Monrreal II