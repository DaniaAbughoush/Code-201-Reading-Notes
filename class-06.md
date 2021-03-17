
# domain:
one of the hardest thing in programming is knowing problem domain:
 * familiarity :the writer used protin tracking example over and over again to make things more easy to under stand.then take off the focus from the problem domain and put instade learning new technolgy .
  * we should take of problem domain because its like a buzzle we cant see what the picture look like .
* problem domain should be fully understood.
* delvepors should focus on markting themselves.
 # object :
 agroup of function and variable together creat amodel you know from real world variable and function will take different names .
* variable=propirty which tell us about the object like it's name
* function=method.
* in the example bellow the obcject value is always a function and it stored in a variable .
* function and variables aree called key and cannot have arepeated key:

![function](https://am3pap002files.storage.live.com/y4mbgTUWVFqoA_3KBf034msleqlahBXUqMGfErbVs0Adac46WS3oZswbZLgeXfrUNNnjR9brlH3dV9xeZTztux_x2pfRrKLvYt6SPM-2jTMBiWg-tOOFBkK1-aQxHFhFXufxiShgum8MSQCwnU7Q_vn51CMEorsxPDcTTP-QvUSd5SMqLMpx7ktRfrvhoKY2Yas5tkw4_-fvdLG1Bx54dH-Aw/2021-03-17%20%2824%29.png?psid=1&width=543&height=567)

* literal notatin is the way to creat an object:
* to acess an objectt you can use dot pr brackets.
 # The Document Object Model (DOM):
 * specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

 * DOM trees have four types of nodes: document nodes,element nodes, attribute nodes, and text nodes

![](https://am3pap002files.storage.live.com/y4mz720hRECrFblkp7SAHyYyc5lYE5Adwjjh4LijpBvzCv1-B_QOqMH9cgI3iyqoASOCQBr9SPYYKeQBIkokgTU44sRmsVhJcqJw6rhUljb7_FVJYHEdA-TlYGpjnIjuV-w-JoTcVdPENh_AitX3lMyyktXxjXzkM0E_8rs_xOykOIJEf4fthQvolR0epM3rnr0AO1RKMqMwdNdSh_R6FMaTQ/2021-03-17%20%2826%29.png?psid=1&width=552&height=288)

 * Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

* STEP 1: ACCESS THE ELEMENTS by:
1. SELECT AN INDIVIDUAL ELEMENT NODE .
2. SELECT MULTIPLE ELEMENTS (NODELISTS) 
3. TRAVERSING BETWEEN ELEMENT NODES 

* STEP 2: WORK W ITH THOSE ELEMENTS
1. ACCESS/ UPDATE TEXT NODES .
2. WORK W ITH HTML CONTENT.
3. ACCESS OR UPDATE ATTRIBUTE VALUES .

 * there is away to find elements in the DOM called querise.
* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 
* we can use selectors to select elements in DOM.
* TO CALL ELEMENT FROM NODE LIST USE ARRAY OR **()**
* YOU CAN USE LOOPS TO REPEATE.
* Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.

* TO ADD OR DELETE ELEMENT:
1. USE HTML inner.
2. DOM manuplation.
 
* DOM manipulation offers another technique to add new content to a page (rather than i nnerHTML). It involves three steps:
1. CREATE THE ELEMENT createEl ement ()  
2. GIVE IT CONTENT createTextNode() 
3. ADD IT TO THE DOM appendChild() 

* DOM manipulation can be used to remove elements from the DOM tree. 
1. STORE THE ELEMENT TO BE REMOVED IN A VARIABLE 
2. STORE THE PARENT OF THAT ELEMENT IN A VARIABLE
3. REMOVE THE ELEMENT FROM ITS CONTA INING ELEMENT 

 * If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site cripting Attacks or XSS; otherwise,an attacker could gain access to your users' accounts. 

* VALIDATE INPUT GOING TO THE SERVER:
1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation. Do not allow untrusted users to submit HTML markup or JavaScrip.
2.  Double-check validation on the server before displaying user content/storing it in a database. This is important because users could bypass validation in the browser by turning JavaScript off
3.  The database may safely contain markup and script from trusted sources (e.g., your content management ystem).This is because it does not try to process the code; it just stores it. 
