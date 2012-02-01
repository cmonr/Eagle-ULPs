~$ man svg2poly

__NAME__

svg2poly - import Simple SVG files as polygons in Eagle CAD
 

__SYNOPSIS__

svg2poly [options]

 
__DESCRIPTION__

There are currently a few Eagle ULPs that can import images into PCBs, but they can be fairly confusing to use. Furthermore, by having to convert to bitmaps, resolution is lost when the file is imported to the PCB.

svg2poly is a program that reads Simple SVG files and outputs polygons onto the PCB, in one simple step. Scaling the image, changing the layer, and even adding a line border are made easy by passing parameters to the script. 


__INSTRUCTIONS__

For the most up to date instructions, please go [here](thinkmaketest.com).
 
__OPTIONS__

Defaults are *-ratio 1.0 -layer tDocu -outline 0*

<<<<<<< HEAD
-ratio *number*
    >Change the X and Y ratio of the imported file. This number can be negative.

-ratiox *number*
    >Change the X ratio of the imported file. This number can be negative.

-ratioy *number*
    >Change the Y ratio of the imported file. This number can be negative.

-layer *name*
    >Change the layer that the polygin is made in. This should be the name of the layer.

-outline *width*
    >Change the width of the outline.
=======
>-ratio *number*
>>Change the X and Y ratio of the imported file. This number can be negative.
>-ratiox *number*
>>Change the X ratio of the imported file. This number can be negative.
>-ratioy *number*
>>Change the Y ratio of the imported file. This number can be negative.
>-layer *name*
>>Change the layer that the polygin is made in. This should be the name of the layer.
>-outline *width*
>>Change the width of the outline.
>>>>>>> c7392fdb43d9c0e1ee14b59e7bb117d5db13448e

    
__AUTHOR__

Written by Cruz Monrreal II