# The *Lists* in HTML

> There are lots of occasions when we
need to use lists. HTML provides us with
three different types:
- ***Ordered lists*** are lists where each item in the list is
numbered. For example, the list might be a set of steps for
a recipe that must be performed in order, or a legal contract
where each point needs to be identified by a section
number.
- ***Unordered lists*** are lists that begin with a bullet point
(rather than characters that indicate order).
- ***Definition lists*** are made up of a set of terms along with the
definitions for each of those terms.
---------------------------
## Ordered Lists
The ordered list is created with
the < ol > element.  
Each item in the list is placed between an opening < li > tag  and a closing < / li > tag. ( The li stands for list item. )
> < ol>  
< li>Chop potatoes into quarters< /li>  
< li>Simmer in salted water for 15-20 minutes until tender< /li>    
< li>Heat milk, butter and nutmeg< /li>  
< li>Drain potatoes and mash< /li>  
< li>Mix in the milk mixture< /li>  
< /ol>  

> 1 Chop potatoes into quarters
 2 Simmer in salted water for 15-20 minutes until tender  
3 Heat milk, butter and nutmeg  
4 Drain potatoes and mash  
5 Mix in the milk mixture

## Unordered Lists
The unordered list is created with the < ul> element.

> <ul>  
< li>1kg King Edward potatoes</li>    
< li>100ml milk</li>   
< li>50g salted butter</li>  
<  li>Freshly grated nutmeg</li>  
< li>Salt and pepper to taste</li>  
< /ul> 
> - 1kg King Edward potatoes
> - 100ml milk
> - 50g salted butter
> - Freshly grated nutmeg
> - Salt and pepper to taste

## Definition Lists
#### < dl>The definition list is created with
the < dl> element and usually
consists of a series of terms and
their definitions.  
Inside the < dl> element you will
usually see pairs of < dt> and
< dd> elements.
#### < dt>
This is used to contain the term
being defined (the definition
term).
#### < dd>
This is used to contain the
definition.
## Nested Lists
You can put a second list inside
an < li> element to create a sublist
or nested list.
>Browsers display nested lists
indented further than the parent
list. In nested unordered lists,
the browser will usually change
the style of the bullet point too.  
> < ul>   
< li>Mousses< /li>  
< li>Pastries  
< ul>  
< li>Croissant< /li>  
< li>Mille-feuille< /li>  
< li>Palmier< /li>  
< li>Profiterole< /li>  
< /ul>  
< /li>  
< li>Tarts< /li>  
< /ul>  
  
> - Mousses  
> - Pastries  
>   - corissant  
>   - mille-fuille  
>   - profiterole 
> - Tarts

# *Boxes* in HTML 

You can set several properties that affect the appearance of
these boxes. In this chapter you will see how to:
- Control the dimensions of your boxes
- Create borders around boxes
- Set margins and padding for boxes
- Show and hide boxes  
Once you have learned how to control the appearance of each
box, you will see how to position these boxes on your pages in
Chapter 15 when we look at page layout.

### Box Dimensions
**width,height**  
By default a box is sized just big
enough to hold its contents.To
set your own dimensions for a
box you can use the height and
width properties.   
The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.
### Limiting Width 
**min-width,max-width**  
Some page designs expand and
shrink to fit the size of the user's
screen. In such designs, the
min-width property specifies  
the smallest size a box can be
displayed at when the browser
window is narrow, and the
max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.
### Limiting Height
**min-height,max-height** 
In the same way that you might
want to limit the width of a box
on a page, you may also want
to limit the height of it. This is
achieved using the min-height
and max-height properties.

### Overflowing Content
The **overflow** property tells the
browser what to do if the content
contained within a box is larger
than the box itself. It can have
one of two values:  
- hidden   
This property simply hides any
extra content that does not fit in
the box.  
- scroll  
This property adds a scrollbar to
the box so that users can scroll
to see the missing content. 

##  Border, Margin & Padding  
Every box has three available properties that
can be adjusted to control its appearance:  
1 **Border** :  
Every box has a border (even if
it is not visible or is specified to
be 0 pixels wide). The border
separates the edge of one box
from another.
2 **Margin**  
Margins sit outside the edge
of the border. You can set the
width of a margin to create a
gap between the borders of two
adjacent boxes.
3 **Padding**   
Padding is the space between
the border of a box and any
content contained within it.
Adding padding can increase the
readability of its contents.


## Border Width
The *border-width* property
is used to control the width
of a border. The value of this
property can either be given
in pixels or using one of the
following values:  
- thin
- medium
- thick
> (You cannot use percentages with this property.)
## Border Style  
**border-style**

You can control the style of a
border using the border-style
property. This property can take
the following values:  
- **solid** a single solid line  
- **dotted** a series of square dots
(if your border is 2px wide, then
the dots are 2px squared with a
2px gap between each dot)    
- **dashed**  a series of short lines  
- **double**  two solid lines (the
value of the border-width
property creates the sum of the
two lines)  
- **groove** appears to be carved
into the page  
- **ridge** appears to stick out from
the page  
- **inset** appears embedded into
the page  
- **outset** looks like it is coming
out of the screen  
- **hidden / none**  no border is
shown 

## Border Color
*border-color*  
You can specify the color of a
border using either RGB values,
hex codes or CSS color names .

## Padding
*padding*  

The padding property allows
you to specify how much space
should appear between the
content of an element and its
border.  
The value of this property is
most often specified in pixels
(although it is also possible to
use percentages or ems). If a
percentage is used, the padding
is a percentage of the browser
window (or of the containing box
if it is inside another box).  
> Please note: If a width is specified for a box, padding is added onto the width of the box.  
## Margin 

The margin property controls
the gap between boxes. Its value
is commonly given in pixels,
although you may also use
percentages or ems.  
If one box sits on top of another,
margins are collapsed , which
means the larger of the two
margins will be used and the
smaller will be disregarded.

> If the width of a box
is specified then the margin is
added to the width of the box

## Change Inline/Block 

The display property allows
you to turn an inline element
into a block-level element or vice
versa, and can also be used to
hide an element from the page.
The values this property can
take are:
- **inline**  
This causes a block-level
element to act like an inline
element.
- **block**  
This causes an inline element to
act like a block-level element.
- **inline-block**  
This causes a block-level
element to flow like an inline
element, while retaining other
features of a block-level element.
- **none**  
This hides an element from the
page. In this case, the element
acts as though it is not on the
page at all (although a user could
still see the content of the box if
they used the view source option
in their browser).


## Box Shadows 
*box-shadow* 
The box-shadow property
allows you to add a drop shadow
around a box. It works just like
the text-shadow property that
you met on page 288. It must
use at least the first of these two
values as well as a color:  
- **Horizontal offset**  
Negative values position the
shadow to the left of the box.  
- **Vertical offset**  
Negative values position the
shadow to the top of the box.  
- **Blur distance**  
If omitted, the shadow is a solid
line like a border.  
- **Spread of shadow** 
If used, a positive value will
cause the shadow to expand in
all directions, and a negative
value will make it contract.  
## Rounded Corners
*border-radius*  
CSS3 introduces the ability to
create rounded corners on any
box, using a property called
border-radius. The value
indicates the size of the radius
in pixels.

----------------------------------------------------------------------  
----------------------------------------------------------------------  

# ARRAYS in JAVASCRIPT

An array is a special type of variable. It doesn't
just store one value; it stores a list of values.
> For example, an array can be
suited to storing the individual
items on a shopping list because
it is a list of related items.
Additionally, each time you write
a new shopping list, the number
of items on it may differ.

### CREATING AN ARRAY
You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).  
The values are assigned to the
array inside a pair of square
brackets, and each value is
separated by a comma. The
values in the array do not need
to be the same data type, so you
can store a string, a number and
a Boolean all in the same array.

> var colors;  
colors['white', 'black', ' custom '];  
var eldocument.getElementByld('colors');  
el.textContent = colors[0];  
### VALUES IN ARRAYS
Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 

## ACCESSING & CHANGING VALUES IN AN ARRAY

To access a value from an array,
after the array name you specify
the index number for that value
inside square brackets.  
You can change the value of an
item an array by selecting it and
assigning it a new value just as
you would any other variable
(using the equals sign and the
new value for that item). 

## F.....ELSE STATEMENTS
the  if...else statement checks a  condition .  
- if it resolves to true the first code block is excuted.  
- if the condition resolves to false the secound code block is run instead.  

## Switch statements 

A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value.  

## TYPE COERCION & WEAK TYPING
If you use a data type JavaScript did not expect,
it tries to make sense of the operation rather
than report an error.  
JavaScript can convert data
types behind the scenes to
complete an operation. This is
known as type coercion. For
example, a string 'l ' could be
converted to a number 1 in the
following expression:(' 1' > 0).
As a result, the above expression
would evaluate to true.  
JavaScript is said to use weak
typing because the data type
for a value can change. Some
other languages require that you
specify what data type
each variable will be. They are
said to use strong typing.  
## TRUTHY & FALSY VALUES 
Due to type coercion, every value in JavaScript
can be treated as if it were true or false; and
this has some interesting side effects. 
## LOOPS
Loops check a condition. if it returns true, a code block will run.  
then the condition will be ckecked again and if it still return true, the code block will run again.  
it repeats until the condition return false.  
** there are three common types of loops : **
- **For**  
if you need to run code a spicific number of times, use for loop.  

- **While**  
if you don't know how many time the code should run, you can use a while loop.  
- **do while**  
the do..while loop is very similar to the while loop, but has one key diffirence: it will
always run statements inside the curley braces at least once *even* if the condition evaluates to **false**  


### LOOP COUNTER
This instructs the code to run a spicified number of times.

#SUMMARY "DECISIONS & LOOPS"

- Conditional statements allow your code to make
decisions about what to do next.
- Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.
- Logical operators allow you to combine more than one
set of comparison operators.
- if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.
- switch statements allow you to compare a value
against possible outcomes (and also provides a default
option if none match).
- Data types can be coerced from one type to another.
- All values evaluate to either truthy or falsy.
- There are three types of loop: for, while, and
do ... while. Each repeats a set of statements





