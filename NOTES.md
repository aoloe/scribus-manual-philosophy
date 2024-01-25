# Notes

Similar to the first steps but more focused on linking to the relevant information rather than on getting the simplest things done (in the right way)

Table of contents:

- Frame based content
- Loading text
  - For very simple documents: double click on the text frame and type ahead.
  - For longer documents, type and proofread your text in LibreOffice or text files and load it into text frames.
- Formatting text
  - The content palette
  - Paragraph and character styles
- Images
  - Supported and suggested image types
  - Scaling and moving inside of the frame
- Page layout
  - Guides (snap, columns / rows)
- Repetive content
  - Styles
  - Scrapbook and symbols
    1. Design a page with the desired layout.
    2. Select everything on the page and "Send to scrapbook"
    3. When you want to create a page with that design, go to that page and double click the scrapbook entry. The contents is the inserted onto the page in the same position as it was when you sent it to the scrapbook.
  - Master page
  - Templates
- Output: producing PDFs
- Color management
- Weak points
  - Table of contents (python script)
  - Footnotes
  - Running titles (python script)
  - Tables (import from LibreOffice)

Some notes:

- or can we call this "scribus-manual-doing-the-right-thing"? "doing it the scribus way"? "Scribus: basic concepts"
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


I created a master page template. When I go into edit mode and add pages with the chosen template, the text or image blocks are not accessible to enter elements? This is nonsense. Where is the time saved by making a master page template and having to retrace the frames to enter text or images?

that's because common items tend to have far more exceptions, than what you expect when carefully set up the "templates" before starting the layout.

in scribus, master pages are some sort of background for the pages.

use them for:

- guides
- page numbers
- whatever is *exactly* the same on *every* page based on that master page

if you want to get some help, for creating "similar" items on your pages you can use:

- styles
- the scrapbook and symbols
- text variables

mix them at your liking and you will be able to create your document in a "positive" way (and never ask yourself: how can i remove the image borders but only on this specific page?)
