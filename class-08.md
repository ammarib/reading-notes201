# LAYOUTS

## positioning elemnts  

1 bulding blocks  
There is two types of bulding block  
* block-level elemnts  
start on new line  
such as < h1> < p> < ul> < li> 
> *Example*  
![](https://github.com/ammarib/reading-notes201/blob/main/images/block.PNG?raw=true)   
* inline-block elements  
this will make element flow in between surrounding text  
such as < img> < b> < i>  
> *Example*  
![](https://github.com/ammarib/reading-notes201/blob/main/images/inline-block.PNG?raw=true)   

#### Position relative
     
Relative positioning moves an element in relation to where it would have been in normal flow.   
For example, you can move it 10pixels lower than it would have been in normal flow or 20% to
the right.  
#### Absolute Position   
When the position property is given a value of absolute,
the box is taken out of normal flow and no longer affects the
position of other elements on the page. (They act like it is not
there.)  
The box offset properties (top or bottom and left or right)
specify where the element should appear in relation to its
containing element.  
#### Fixed position   
 Fixed positioning is a type of absolute positioning that requires the position property
to have a value of fixed.   
It positions the element in relation to the browser window. Therefore, when a user scrolls
down the page.   

## Floating elements  
 The float property take an element place it as far to the left or right of the containing
element as possible.   
Anything else that sits inside the containing element will flow around the element that is
floated.   

## fixed layout width  

Fixed width layout
designs do not change size as the user increases or decreases the size of their
browser window. Measurements tend to be given in pixels.  

## liquid layout  
The liquid layout uses percentages to specify the width of each box so that the design
will stretch to fit the size of the screen.   

> body {
> width: 90%;
> margin: 0 auto;}
>.column1, .column2, .column3 {  
width: 31.3%;  
float: left;  
margin: 1%;}      



