# IMAGES  
* How to add images to pages
* Choosing the right format
* Optimizing images for the web
------------------------
> There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.  

There are several things to consider when selecting and
preparing images for your site, but taking time to get them
right will make it look more attractive and professional.  
  for example  
* Include an image in your web pages using HTML  
* Pick which image format to use
* Show an image at the right size
* Optimize an image for use on the web to make pages
load faster  
## Choosing Images for Your Site  
*A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one .*  
"Images can be used to set the
tone for a site in less time than
it takes to read a description. If
you do not have photographs
to use on your website, there
are companies who sell stock
images; these are images you"  
## Adding Images
To add an image into the page
you need to use an < img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:  
* src  
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.  
* alt  
This provides a text description
of the image which describes the
image if you cannot see it.  
> for example : < img src="images/quokka.jpg" alt="A family of
quokka" title="The quokka is an Australian
marsupial that is similar in size to the
domestic cat." / >  

### Where to Place Images in Your Code  
Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:
1 **before a paragraph**  
The paragraph starts on a new
line after the image.  
2 **inside the start of a paragraph**  
The first row of text aligns with
the bottom of the image.  
3 **in the middle of a paragraph**  
The image is placed between the
words of the paragraph that it
appears in.  
### HTML 5: Figure and Figure Caption  
  < figure>  
Images often come with
captions. HTML5 has introduced
a new <figure> element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the <  figure>
element as long as they all share
the same caption.  
   < figcaption>
The < figcaption> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.  
Before these elements were
created there was no way to
associate an < img> element with
its caption.  
> *for example*  <figure>
< img src="images/otters.jpg" alt="Photograph of
two sea otters floating in water">
< br/>
< figcaption>Sea otters hold hands when they
sleep so they don't drift away from each
other.< /figcaption>
< /figure>   
 ### Summary IMAGES
* The < img> element is used to add images to a
web page.  
* You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.  
* You should save images at the size you will be using
them on the web page and in the appropriate format.  
* Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.  

# Color
> Color can really bring your pages to life.  

### Foreground Color  


The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:   
1 **rgb values**  
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90) 
2 **hex codes**  
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80  
3 **color names**  
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan  
### Background color  
CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.  
> If you do not specify a
background color, then the
background is transparent.  
### Opacity 
CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).   
### HSL & HSLA 

The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:  
1 hue  
This is expressed as an angle
(between 0 and 360 degrees).   
2 saturation  
This is expressed as a
percentage.  
3 lightness  
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black. 
The hsla color property allows
you to specify color properties
using hue, saturation, and
lightness as above, and adds a
fourth value which represents
transparency (just like the rgba
property). The a stands for:
4 alpha  
This is expressed as a
number between 0 and 1.0.
For example, 0.5 represents
50% transparency, and 0.75
represents 75% transparency.  
> *for example*  
body {
background-color: #C8C8C8;
background-color: hsl(0,0%,78%);}
p {
background-color: #ffffff;
background-color: hsla(0,100%,100%,0.5);}   

## Summary
**COLOR**  
* Color not only brings your s XX ite to life, but also helps
convey the mood and evokes reactions.  
* There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.  
* Color pickers can help you find the color you want.  
* It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).  
* CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.  
* CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.  

# TEXT  
### Choosing a Typeface for your Website  
When choosing a typeface, it is important to understand that a
browser will usually only display it if it's installed on that user's computer. 
* **Serif**  
Serif fonts have extra details on
the end of the main strokes of
the letters.  
* **Sans-Serif**  
Sans-serif fonts have straight
ends to letters and therefore
have a much cleaner design.   
* **Monospace**  
Every letter in a monospace
typeface is the same width.
(Non-monospace fonts have
different widths.)  
* **Cursive**  
Cursive fonts either have
joining strokes or other cursive
characteristics, such as
handwriting styles.  
* **Fantasy**  
Fantasy fonts are usually
decorative fonts and are often
used for titles. They're not
designed for long bodies of text.  
### Specifying Typefaces  
> font-family    

 The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.  
The value of this property is the
name of the typeface you want
to use.
> for example : body {  
font-family: Georgia, Times, serif;}   
h1, h2 {  
font-family: Arial, Verdana, sans-serif;}  
.credits {
font-family: "Courier New", Courier,  
monospace;}   

## Size of Type  
> font-size   

The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are: 
 * **pixels**  
 * **percentages**  
 * **ems**  > for example : h2 {  
font-size: 1.3em;}  

## font-face  
font-face allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.
Because this technique allows
a version of the font to be
downloaded to the user's
computer, it is important that the
license for the font permits it to
be used in this way.
You add the font to your style
sheet using the font-face
rule, as shown on the right.    
* font-family  
This specifies the name of the
font. This name can then be used
as a value of the font-family
property in the rest of the style
sheet (as shown in the rule for
the <h1> and <h2> elements).  
* src
This specifies the path to the
font. In order for this technique
to work in all browsers, you will
probably need to specify paths
to a few different versions of the
font, as shown on the next page.   
* format  
This specifies the format that the
font is supplied in. (It's discussed
in detail on the next page.)  
## font-weight  
The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:  
* **normal**  
This causes text to appear at a
normal weight.
* **bold**  
This causes text to appear bold.
In this example, you can see
that the element whose class
attribute has a value of credits
has been bolded.  
## font-style  
If you want to create italic text,
you can use the font-style
property. There are three values
this property can take:  
* **normal**  
This causes text to appear in a
normal style (as opposed to italic
or oblique).  
* **italic**  
This causes text to appear italic.  
* **oblique** 
This causes text to appear
oblique.  

## text-transform  
The text-transform property
is used to change the case of
text giving it one of the following
values:  
* *uppercase*  
This causes the text to appear
uppercase. 
* *lowercase* 
This causes the text to appear
lowercase.  
* *capitalize* 
This causes the first letter of
each word to appear capitalized.  
## text-decoration
The text-decoration property
allows you to specify the
following values:  
* *none*  
This removes any decoration
already applied to the text.
underline
This adds a line underneath the
text.  
* *overline*  
This adds a line over the top of
the text. 
* *line-through*  
This adds a line through words. 
* *blink*  
This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying).  
## text-align  
The text-align property allows
you to control the alignment of
text. The property can take one
of four values:  
* *left* 
This indicates that the text
should be left-aligned.  
* *right*  
This indicates that the text
should be right-aligned.  
* *center*  
This allows you to center text.  
* *justify*  
This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.  
 ## text-shadow
 The text-shadow property has
become commonly used despite
lacking support in all browsers.
It is used to create a drop
shadow, which is a dark version
of the word just behind it and
slightly offset. It can also be used
to create an embossed effect by
adding a shadow that is slightly
lighter than the text.  
> for example : text-shadow: 1px 1px 0px #000000;}   

The first length indicates how
far to the left or right the shadow
should fall.  
The second value indicates the
distance to the top or bottom
that the shadow should fall.  
The third value is optional and
specifies the amount of blur that
should be applied to the drop
shadow.   
The fourth value is the color of
the drop shadow.   

## Styling Links  
> :link, :visited  
* **:link** 
This allows you to set styles
for links that have not yet been
visited.  
* **:visited**  
This allows you to set styles for
links that have been clicked on.  
> *for example :* a:link {  
color: deeppink;  
text-decoration: none;}  
a:visited {  
color: black;}  
a:hover {  
color: deeppink;  
text-decoration: underline;}  
a:active {  
color: darkcyan;}     

## Responding to Users  
> :hover, :active, :focus  
* *:hover*  
This is applied when a user
hovers over an element with a
pointing device such as a mouse.
This has commonly been used
to change the appearance of
links and buttons when a user
places their cursor over them. It
is worth noting that such events
do not work on devices that use
touch screens (such as the iPad)
because the screen is not able to
tell when someone is hovering
their finger over an element.  
* *:active*  
This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make
a button or link feel more like it
is being pressed by changing the
style or position of the element
slightly.  
* *:focus*  
This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus  

### Summary   
**TEXT**  
* There are properties to control t XX he choice of font, size,
weight, style, and spacing.  
* There is a limited choice of fonts that you can assume
most people will have installed.  
* If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.  
* You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.  
* You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.  






  
