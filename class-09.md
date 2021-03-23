# forms:
* forms for print and enter information like google box,search,subscribe,answer,submit.
* how forms work:
1. A user fills in a form and then presses a button to submit the information to the server.
1. The name of each form control is sent to the server along with the value the user enters or selects.
1. The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
1. The server creates a new page to send back to the browser based on the information received.

 * A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element.
  
  * To differentiate between various pieces of inputted data, information is sent from the browser to the server using name/value pairs.

 * form structure:
  use form tag inside action att to put the page that will store the data.
 * method att:
 With the get method, the values from the form are added to the end of the URL specified in the action attribute. 
 
 * The get method is ideal for:
 1. short forms (such as search boxes)
1. when you are just retrieving data from the web server (not sending information that should be added to or deleted from a database).

* With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use  post method if your form:
1.  allows users to upload a file  is very long
1. contains sensitive data (e.g. passwords)
1.  adds information to, or deletes infor

**If the method attribute is not used, the form data will be sent using the get method.**

* Text Input:
* The input tag element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.
* type="text" When the type attribute has a value of text, it creates a singleline text input
* name When users enter information into a form.
* size The size attribute should not be used on new forms
* maxlength You can use the maxlength attribute to limit the number of characters
* type="password" When the type attribute has a value of password it creates a text box that acts just like a
single-line text input.
* textarea The **textarea** element is used to create a mutli-line text input
* type="radio" Radio buttons allow users to pick just one of a number of options.
* checked The checked attribute can be used to indicate which value (if any) should be selected when the page loads.
* Checkboxes allow users to select (and unselect) one or more options in answer to a question.
* type="image" If you want to use an image for the submit button, you can give the type attribute a value of
image.
* HTML5 introduces new form elements which make it easier for visitors to fill in forms.


* The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker). 
* In addition to the CSS properties covered in other chapters which work with the contents of all elements,
there are several others that are specifically used to control the appearance of lists, tables, and forms.
* List markers can be given different appearances using the list-style-type and list-style image
properties.
* Table cells can have different borders and spacing in different browsers, but there are properties you can
use to control them and make them more consistent. 
* Forms are easier to use if the form controls are vertically aligned using CSS.
* Forms benefit from styles that make them feel more interactive.

# Events 
* Scripts often respond to these events by updating the content of the web page.
* INTERACTIONS EVENT CREATE EVENTS:Events occur when user you
click or tap on a link.
* EVENTS TRIGGER CODE :
* CODE RESPON TO USERS .

![](https://1drv.ms/u/s!AiRND7yx23JIgjqagazL-gpwz-MJ?e=YZK2DX)
![](https://1drv.ms/u/s!AiRND7yx23JIgjkMcL5lRYSuYFgn?e=eed5EQ)

* EVENTS FIRE OR ARE RAISED When an event has occurred, it is often described as having fired or been raised. In the diagram on the right, if the user is tapping on a link, acl ick event would fire in the browser.

* HOW EVENTS TRIGGER JAVASCRIPT CODE :
1. Select t he element node(s) you want the script to respond to
1. Indicate which event on the selected node(s) will trigger the response. 
1. State the code you want to run when the event occurs.

* All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler. 

* When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see the approach below used; it relies on the this keyword. 
* When an event occurs on an element, it can trigger aJavaScript function. When this function then changes
the web page in some way, it feels interactive because it has responded to the user. 
* You can use event delegation to monitor for events that happen on all of the children of an element. 
* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events. 
