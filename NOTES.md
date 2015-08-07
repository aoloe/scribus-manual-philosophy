# Notes

- or can we call this "scribus-manual-doing-the-right-thing"?
- linking to image frames, loading text frames
- creating and using colors
- bold and italics
- RGB, CMYK, input and PDF output
  - utnki says: most office printer drivers work with rgb input.  
    cmyk 0, 0, 0, 100 is not a rich black like rgb 000000. if you provide a file in cmyk, the driver converts this tone to some rgb equivalent (like 1d1b1b) as its input value and  reconverts this really dark gray in the profile of the printer.  
    so you should probably feed your printer with a file in rgb (or in grayscale, if there's no other color used in the whole document…)  
    rgb 000000 and cmyk 0, 0, 0, 100 colors with output in 'grayscale' should print black.  
    rgb 000000 colors with output for 'screen/web' should print black.  
    every other combination (with one exception) may end in a dark gray.  
    the exception is a professional workflow with the correct output profile for your printer.
- double pages, left and right masterpages, adding single/double pages
  - arrange pages can be of some help if you have to add a single page...
- master pages as a background (+scrapbook, ...)
- avoid using the "story editor" (ctrl-t) except for the cases where you really need it (double click a text field to enter the edit mode, press esc to leave the edit mode and display the "window > properties" palette for formatting your text)
- ESC key for leaving the current edit mode and go back, step by step, to the original unselected state.
