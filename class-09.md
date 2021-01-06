# FORMS  
The HTML < form> element represents a document section containing interactive controls for submitting information.   
The < form> element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons   
The HTML <form> element can contain one or more of the following form elements:   
* < input>  
element can be displayed in several ways, depending on the type attribute.   
* < label>   
defines a label for several form elements.    
* < select>   
defines a drop-down list   
* < textarea>   
defines a multi-line input field (a text area):    
* < button>   
defines a clickable button:    
> Example : < button type="button" onclick="alert('Hello World!')">Click Me!< /button>   
* < fieldset>    
used to group related data in a form.  
* < legend>   
defines a caption for the <fieldset> element.   
* < datalist>   
 specifies a list of pre-defined options for an <input> element.     
* < output>    
represents the result of a calculation (like one performed by a script).    
* < option>   
defines an option that can be selected.   
* <optgroup>    
	Defines a group of related options in a drop-down list   
================================================
# LISTS , TABLES AND FORMS   
* In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.     
* List markers can be given different appearances
using the list-style-type and list-style image
properties.    
* Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.   
* Forms are easier to use if the form controls are
vertically aligned using CSS.   
* Forms benefit from styles that make them feel more
interactive.  
===============================================================
# JS EVENTS 
events are actions or occurrences that happen in the system 
you are programming — the system produces (or "fires") a signal
of some kind when an event occurs, and provides a mechanism by
which an action can be automatically taken (that is, some code running) when the event occurs   
There are many different types of events that can occur. For example:   
* The user selects a certain element or hovers the cursor over a certain element.   
* The user chooses a key on the keyboard.   
* The user resizes or closes the browser window.   
* A web page finishes loading.    
* A form is submitted.   
* A video is played, paused, or finishes.   
* An error occurs.    
> for example :
< button>Change color< /button>   
> const btn = document.querySelector('button');   
> function random(number) {   
>   return Math.floor(Math.random() * (number+1));   
> }   
> btn.onclick = function() {   
 >  const rndCol = 'rgb(' + random(255) + ',' + random(255) + ',' + random(255) + ')';   
 >  document.body.style.backgroundColor = rndCol;   
> }        

In this code, we store a reference to the button inside a constant called btn, using the
Document.querySelector() function. We also define a function that returns a random number.
The third part of the code is the event handler. The btn constant points to a < button> element,
and this type of object has a number of events that can fire on it, and therefore, event handlers
available. We are listening for the click event firing, by setting the onclick event handler property to
equal an anonymous function containing code that generates a random RGB color and sets the < body> background-color equal to it.    





