# Object Literals
**what is objects?**  
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object, variables and functions take on new names  
> **IN AN OBJECT**: VARIABLES BECOME KNOWN AS PROPERTIES  
If a variable is part of an object, it is called a
property. Properties te ll us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.  
> IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS  
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with# 
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.  

 Example:  

![](https://github.com/ammarib/reading-notes201/blob/main/images/Screenshot%20(31).png?raw=true)  

* literal notation is the easiest and most popular way to create objects .  

## Accessing an object and dot notation 
![](https://github.com/ammarib/reading-notes201/blob/main/images/objest.PNG?raw=true)  

![](https://github.com/ammarib/reading-notes201/blob/main/images/see.PNG?raw=true)

![](https://github.com/ammarib/reading-notes201/blob/main/images/swq.PNG?raw=true)
---------------------------------------------------------------------------   
-------------------------------------------------------------------------- 
   
   # Document Object Model  
   
   the document object level (DOM) specifies how browser should creat a model of an HTML page
   and how JavaScript can access and update the content of a web page while it is in the browser windows.   
   > The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. is implemented by all major browser makers, and covers two primary areas.    
   
   * MAKING A MODEL OF THE
HTML PAGE
When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.   
* ACCESSING AND CHANGING
THE HTML PAGE
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.   

## THE DOM TREE IS A
MODEL OF A WEB PAGE   

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.  

BODY OF HTML PAGE
< html>
 < body>
  < di v id="page">
   < hl id="header">List< /hl>
   < h2>Buy groceries< /h2>
   < ul>
    < li id="one" class="hot">< em>fresh< /em> figs< /li>
    < li id="two" class="hot">pine nuts< /l i>
    < li id="three" class="hot">honey< /l i>
    < li id="four">balsamic vinegar< /l i>
   < / ul>
   < script src="js/list.js ">< /scri pt>
  < / div>
 < / body>
< / html>   

![](https://github.com/ammarib/reading-notes201/blob/main/images/ewqd.PNG?raw=true)  

# WORKING WITH DOM TREE  
![](https://github.com/ammarib/reading-notes201/blob/main/images/domtree.PNG?raw=true)  
![](https://github.com/ammarib/reading-notes201/blob/main/images/cashingdom.PNG?raw=true)
![](https://github.com/ammarib/reading-notes201/blob/main/images/cashindom2.PNG?raw=true)  
 
 
 # NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT  
 
 > When a DOM method can return more than one element, it returns a
Nodelist (even if it only finds one matching element).  
A Nodelist is a collection of element nodes. Each
node is given an index number (a number that starts
at zero, just like an array).
The order in which the element nodes are stored in a
Node List is the same order that they appeared in the
HTML page.   

When a DOM query returns a Nodelist, you may
want to:  
* Select one element from the NodeList.  
* Loop through each item in the Nodelist and
perform the same statements on each of the
element nodes.   

![](https://github.com/ammarib/reading-notes201/blob/main/images/select.PNG?raw=true)  
 ## SELECTING ELEMENTS USING CLASS ATTRIBUTES    
 The getElementsByClass Name()
method allows you to select
elements whose c 1 ass attribute
contains a specific value.  
The method has one parameter:  
the class name which is given
in quotes within the parentheses
after the method name.  
Because several elements can
have the same value for their
cl ass attribute, this method
always returns a Nodelist.  
![](https://github.com/ammarib/reading-notes201/blob/main/images/exmpl.PNG?raw=true)  

## SELECTING ELEMENTS BY TAG NAME  
The get El ementsByTagName ()
method allows you to select
elements using their tag name.  
The element name is specified
as a parameter, so it is placed
inside the parentheses and is
contained by quote marks.  
Note that you do not include the
angled brackets that surround
the tag name in the HTML (just
the letters inside the brackets).   
 ## SELECTING ELEMENTS USING CSS SELECTORS  
 
querySe 1 ector() returns
the first element node that
matches the CSS-style selector.
querySe 1ectorA11 () returns a
Nodelist of all of the matches.  
Both methods take a CSS
selector as their only parameter.
The CSS selector syntax offers
more flexibility and accuracy
when selecting an element than
just specifying a class name
or a tag name, and should also
be familiar to front-end web
developers who are used to
targeting elements using CSS.  

## LOOPING THROUGH A NODELIST
If you want to apply the same
code to numerous elements,
looping through a Nodelist is a
powerful technique.  
It involves finding out how many
items are in the Nodelist, and
then setting a counter to loop
through them, one-by-one.
Each time the loop runs, the
script checks that the counter
is less than the total number of
items in the Nodelist   

var hotltems = document.querySelectorAll('li.hot');  
if (hotltems.length > O){  
for (var i=O; i<hotltems.length; i++) {  
hotltems[i ] .className = 'cool';  
}  
}    
##  ACCESSING & CHANGING A TEXT NODE  
To work with text in an element,
first the element node is
accessed and then its text node.  
The text node has a property
called node Value which returns
the text in that text node.
You can also use the nodeVa1ue
property to update the content
of a text node.  
> var itemTwo document.getElementByld('two');  
> var elText itemTwo.firstChild .nodeValue;  
> elText = elText.replace( ' pine nuts', ' kal e ' );   
> itemTwo . firstChi ld.nodeValue = elText;    

## ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INNERTEXT)  
The textContent property allows you to
collect or update just the text that is in the
containing element (and its children).  
To collect the text from the
< li> elements in our example
(and ignore any markup inside
the element) you can use the
textContent property on the
containing < li> element. In this
case it would return the value:
fresh figs.   

## ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML  
Using the innerHTML property, you can access and amend the contents of an element, including any child elements.   
innerHTML
When getting HTML from an
element, the i nnerHTML property
will get the content of an
element and return it as one long
string, including any markup that
the element contains.     
When used to set new content
for an element, it will take a
string that can contain markup
and process that string, adding
any elements within it to the
DOM tree.   
![](https://github.com/ammarib/reading-notes201/blob/main/images/croossite.PNG?raw=true)  
![](https://github.com/ammarib/reading-notes201/blob/main/images/ATT.PNG?raw=true)  


