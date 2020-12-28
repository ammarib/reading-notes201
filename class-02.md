# intro to HTML
## Text
- Headings and paragraphs
- Bold, italic, emphasis
- Structural and semantic markup
> *When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.*
## Headings
 HTML has six "levels" of headings:
 * **H1**
 * **H2**
 * **H3**
 * **H4**
 * **H5**
 * **H6**
 ## Paragraphs
 To create a paragraph, surround the words that make up the paragraph with an opening **< p >** tag and closing **< /p >** tag.
 
 ## Quotations
 There are two elements commonly used for marking up quotations:
**< blockquote >**
* The < blockquote > element is used for longer quotes that take up an entire paragraph. Note how the <p> element is still used inside the < blockquote > element.
achieve this effect using CSS.
* **< q >**
The < q > element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the < q > element, however Internet Explorer does not — therefore many people avoid using the < q > element.
 
 ## Author Details
The **< address >** element has quite a specific use: to contain contact details for the author of
the page. It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address.
### Summary TEXT
* HTML elements are used t XX o describe the structure of the page (e.g. headings, subheadings, paragraphs).
* They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).
-------------------------------------------------------

# Introduction to CSS
## CSS Properties Affect How Elements Are Displayed
CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.
## Using External CSS
* The < link > element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the <head> element. It should use three attributes:
* href This specifies the path to the CSS file (which is often placed in a folder called css or styles).

## Using Internal CSS
You can also include CSS rules within an HTML page by placing them inside a < style > element, which usually sits inside the < head > element of the page. The < style > element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/ css.

### Summary introducting CSS
* CSS treats each HTML e XX lement as if it appears inside
its own box and uses rules to indicate how that
element should look.
* Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
* Different types of selectors allow you to target your
rules at different elements.
* Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document,
although they may appear within an HTML page.
-------------------------------------------------------------------

# Basic JavaScript instruction
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

## WHAT IS A VARIABLE
A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.
 ## Summary
 
 * A script is made up of a series of statements. Each
statement is like a step in a recipe.
* Scripts contain very precise instructions. For example,
you might specify that a value must be remembered
before creating a calculation using that value.
* Variables are used to temporarily store pieces of
information used in the script.
* Arrays are special types of variables that store more
than one piece of related information.
* JavaScript distinguishes between numbers (0-9),
strings (text), and Boolean values (true or false).
* Expressions evaluate into a single value.
* Expressions rely on operators to calculate a value.
## Decisions and Loops
### Decision making
##### USING COMPARISON OPERATORS
At the most basic level, you can
evaluate two variables using a
comparison operator to return a
true or false value.
## Logical Operator
logical operator allows you to compare the results of more than one compasition operator .
## if statement
the **if** statement evaluates or checks a condition. if the condition evaluates to true, any statements in the supsequent code block are excuted.
## if .. else statements
the if .. else statement check a condition 
- if it resolves to true the first code block is executed.
- if the condition resolves to false the second code block is run instead.


