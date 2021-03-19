
 # lay out:
 CSS treat each elements in the html as seperate box in can be seprated by boards and margin:
 * block -level like **li** has its on box
 * inline box flow through text like **img**
 * **the containing element** if block level element inside another block level element then its a containing or **parent** like **div**
 **you can Controlling the Position of Elements**:
 1. **Normal flow** Every block-level element appears on a new line and this is the default will cause to lower element to go down.
 2. **Relative Positioning** will not affect the other element you can shift top,right,left.
 3. **Absolute positioning** will not affect surrounding elements will be scrolled.
 
 **box offset** to control the box position hoe far from right,top,left,bottom.
 **Fixed Positioning** will not move when scrolled up or down.
 **Floating Elements** i can move it up down
 **z-index** to control which box appear on top.
 * **normal flow**  not nedd the CSS but this is the syntax for it:**position: static**
 * **relative position** position:relative
  * **the absolute position** use this syntax **position:absolute**
  * **fixed position:** use this syntax **position:fixed**
  * **float** to place element side by side.
  * we can clera float too
  * you should take in condration the screen size and resolution and paper size when printing. 
  ** the fixed layout wont change the size in different divice.
  
  | advantage    | disadvantage |
| ----------- | ----------- |
|  Pixel values are accurate at controlling size   | You can end up with big gaps around the edge        |
|  The designer has far greater control over the appearance   |  the page can look smaller    |
|  You can control the lengthsof lines  |      text might not fit into the allotted spaces   |
|  The size of an image will always remain the same   | The design works best on computer or laptop     |
|    |   The page will often take upmore vertical space       |

** Liquid layout designs stretch and contract as the user increases or decreases the size of their browser**

| advantage    | disadvantage |
| ----------- | ----------- |
| Pages expand to fill the entire browser window   |  the design can look very different than intended      |
|  fit it without the user having to scroll    | lines of text can become very long     |
|The design is tolerant of users setting      |  words may be squashed      |
|    | the image can overflow over the text.   |

* **Grids help create professional  designs** .
* **CSS Frameworks provide rules for common tasks.and You can include multiple CSS files in one page**