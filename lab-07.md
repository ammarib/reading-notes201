# Domain Modeling  

[Domain Modeling](https://github.com/codefellows/domain_modeling.git "Domain Modeling")

## Tables
*What's a Table?*    
A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.  

### Basic Table St ructure   
< table>   
The <table> element is used
to create a table. The contents
of the table are written out row
by row.   
< tr>   
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more
< td> elements (one for each cell
in that row).
At the end of the row you use a
closing < /tr> tag.     
< td>   
Each cell of a table is
represented using a < td>
element. (The td stands for
table data.)     
At the end of each cell you use a
closing < /td> tag.     

### Table Headings    
< th>   
The < th> element is used just
like the < td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)   
Even if a cell has no content,
you should still use a < td> or
< th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)   
Using < th> elements for
headings helps people who
use screen readers, improves
the ability for search engines
to index your pages, and also
enables you to control the
appearance of tables better
when you start to use CSS.    
You can use the scope attribute
on the < th> element to indicate
whether it is a heading for a
column or a row. It can take the
values: row to indicate a heading
for a row or col to indicate a
heading for a column.     

### Long Tables    
There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).     
< thead>   
The headings of the table should
sit inside the < thead> element.
< tbody>   
The body should sit inside the   
< tbody> element.   
< tfoot>   
The footer belongs inside the
< tfoot> element.   


# Summary   
TABLES  
* The < table> element is used to add tables to a web
page.   
* A table is drawn out row by row. Each row is created
with the < tr> element.  
* Inside each row there are a number of cells
represented by the < td> element (or < th> if it is a
header).  
* You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.   
* For long tables you can split the table into a < thead>,
< tbody>, and < tfoot>.  
==================================================

# objets

## CREATING OBJECTS USING CONSTRUCTOR SYNTAX   
> *example*  
> var hotel = new Object();   
hotel.name= 'Park';   
hotel.rooms = 120;   
hotel .booked = 77;   
hotel .checkAvailability = function()   
return this . rooms - this.booked;   
} ;  
var elName = document.getElementByid('hotelName');   
elName.textContent = hotel . name;   
var elRooms = document .getElementByid('rooms');   
elRooms .textContent = hotel .checkAvailability(};       



![](https://github.com/ammarib/reading-notes201/blob/main/images/jsobj.PNG?raw=true)  
## STORING DATA   
In JavaScript, data is represented using name/value pairs.
To organize your data, you can use an array or object to group a set of
related values. In arrays and objects the name is also known as a key.   

### WHAT ARE BUILT-IN
OBJECTS?
Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.      
The objects you create will usually be specifically
written to suit your needs. They model the data
used within, or contain functionality needed by,
your script. Whereas, the built-in objects contain
functionality commonly needed by many scripts.
As soon as a web page has loaded into the browser,
these objects are available to use in your scripts.      
These built-in objects help you get a wide range
of information such as the width of the browser
window, the content of the main heading in the page,
or the length of text a user entered into a form fie ld.     
You access their properties or methods using dot
notation, just like you would access the properties or
methods of an object you had written yourself.     



![](https://github.com/ammarib/reading-notes201/blob/main/images/brwsrobj.PNG?raw=true)

![](https://github.com/ammarib/reading-notes201/blob/main/images/brwsr.PNG?raw=true)
![](https://github.com/ammarib/reading-notes201/blob/main/images/objexm.PNG?raw=true)
![](https://github.com/ammarib/reading-notes201/blob/main/images/objexm.PNG?raw=true)  

 





