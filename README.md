Select each script in the EAGLE Command Panel for more information.

__INSTRUCTIONS for svg2poly__

svg2poly was made to handle Simple SVG files from Inkscape. It can currently only handle text.

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

    
__AUTHOR__

Written by Cruz Monrreal II