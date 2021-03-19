# Domain modeling:
 is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain.

# Define a constructor and initialize properties:
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

# The  object-oriented programming in JavaScript at its most fundamental level.
1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.

# Generate random numbers:
To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

# Generate random numbers
To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

 # Here's some tips to follow when building your own domain models.

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
3. Create instances using the new keyword followed by a call to a constructor function.
3. Store the newly created object in a variable so you can access its properties and methods from outside.
3. Use the this variable within methods so you can access the object's properties and methods from inside.






# table:
* A table represents information in a grid format                                   
* using table tag for maing atable and tr for roe td for the data th for heading data
* **colspan** and **rawspan** to indicate the number of raw and coulums.
* main 3parts of table:
1. thead for the table head
1. tbody for table main content
1. tfoot for end of the table.

* in the old code there was codes used in table opening tag like  width and border attribute.
 *Literal nation is the most popular way to store anobject 
 1. store object in **var** then 
1. open curly braces
1. enter the value wich called properaties seperated by colon,
1. then use amethod it could be function

* accsess the object:
 1. **dot nation :
 * object name followed by period then prpery or method name.
 * method and prperty are the object member.
 * the period is the operater member.

2. using square brackets:
using object name followed by brackets include property name

* used nation method when the property is 
1. anumber you should avoid this.
2. avariable.

* you can update prperty or adding by same method of acces followed by **='new update or new value of pro'
* you can delete use **delete** key word.

 * The keyword this is commonly used inside functions and objects.Where the function is declared alters what  his means. It always refers to one object, usually the object in which the function operates. 

* A FUNCTION IN GLOBAL SCOPE: 
When a function is created at the top level of a script (that is, not inside another object or function), then it is in the global scope or global context. 
 * GLOBAL VARIABLES
All global variables also become properties of the window object. so when a function is in the  context, you can access global variables using the window object, as well as its other properties. 

* If you want to access items via a property name or key, use an object (but note that each key in the object must be unique). If the order of the items is important, use an array.

* arrays are special type of object.

![](https://am3pap002files.storage.live.com/y4mUR1Az80NUkLjDKb_NStFNmVVDQ5l0laNQzZ9yiSFxqyiUBQ6sH1F2-1IbpGyb8RUMCuYegvecVFjEcz_C--ESdZ28ZhpGWuoNAP09X_jM2vk_rR5NWRKQCY5EX2TtXoTaw06frErU2hGawUtzpxRNyGUsyS_raaEVok1OoszfFhV9yIOFyZRlqrgzoDD52QuJ0sMrYsEq90c14MVi_ZlwQ/2021-03-19%20%282%29.png?psid=1&width=676&height=567)
![](https://1drv.ms/u/s!AiRND7yx23JIgh0CsVEBMDdnPRXH?e=UhXskN)

* Browsers come with a set of built-in objects that represent things like  browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

* The first thing you need to do is get to know what tools are available.You can imagine that your new toolkit has three compartments: 
1. BROWSER OBJECT MODEL The Browser Object Model contains objects that represent the current browser window or tab. It contains objects that model things  browser history and the device's screen. 
2. DOCUMENT OBJECT MODEL The Document Object Model uses objects to create a representation  the current page. It creates a new object for each element (and each individual section of text) within the page
3. GLOBAL JAVASCRIPT OBJECTS The global JavaScript objects represent things that the JavaScript language needs to create a model of. For example, there is an object that deals only with dates and times
 ![](https://1drv.ms/u/s!AiRND7yx23JIgh8D1EQi5XF9ycNQ?e=82goc7)

 * The window object represents the current browser window or tab. It is the topmost object in the Browser Object Model, and it contains other objects that tell you about the browser. 
  * Web browsers implement objects that represent both the browser window and the document loaded into the
browser window. 

