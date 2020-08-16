# Read: 02 - jQuery, Events, and The DOM

## JavaScript and jQuery book by Jon Duckett pages 293-301, 306-331 and 354-357

- jQuery is a JavaScript file you include in your pages.
  - Lets you find elements using CSS-style selectors and then do something with the elements using jQuery methods.
    - ```$(‘li.hot’).addClass(‘complete’);```
- JQuery makes coding simpler
- Once included, it makes it faster and easier to write cross-browser JavaScript based on two steps:
  - Using CSS-style selectors to collect one or more nodes from the DOM tree.
  - Using jQuery’s built-in methods to work with the elements in that selection.
- jQuery’s CSS-style selector syntax makes it easier to select elements to work with.
  - Methods to easily traverse the DOM
- Four methods that update the content of all elements. p. 316
  - .html()
  - .text()
  - .replaceWith()
  - .remove()
- Inserting new elements involves two steps:
  - Creating a new elements in a jQuery object
  - Use a method to insert the content into the page. p. 318
    - .before()
    - .after()
    - .prepend()
    - .append()
- Create attributes, or access and update their contents. p. 320
  - .attr()
  - .removeAttr()
  - .addClass()
  - .removeClass()
- .css() method lets you retrieve and set the values of CSS properties
  - ```$(‘li’).css(background-color’, ‘red’);```
- .each() method - p.324
- jQuery makes it easier to handle events because the event methods work across all browsers.
  - .on() method is used to handle all events
    - More information on p. 326-328
- jQuery offers methods that make it quick and simple to achieve a range of tasks that JavaScrip[t programmers commonly need to perform.

## 6 Reasons for Pair Programming

- Pair programming commonly involves two roles: the Driver and the Navigator
  - Driver is the programmer who is typing and the only one whose hands are on the keyboard
  - Navigator uses their words to guide the Driver but does not provide any direct input to the computer
- Why paired programming?
  - Utilizes four fundamental skills that help anyone learn a new language:
    - Listening, speaking, reading and writing
  - Greater efficiency
    - Might take slightly longer, but better quality code
    - Finds solution to problem faster
  - Engaged collaboration
    - Keeps each other accountable
    - Rely on each other and get the help when needed
- Learning from fellow students
  - Exposes to new/different techniques
  - One team mate with higher skill in one field can teach the other. Vice versa.
- Social skills
  - Improve social and communication skills.
  - Companies would rather hire people who work well with each other than strong programmers
- Job Interview readiness
  - The ability to work with and learn from others and stellar communication skills are as important to a company than specific technical skills.
- Work environment readiness
  - Paired programming gets you ready for the real tech world.

## JavaScript and jQuery book by Jon Duckett pages 332-335

- jQuery effects list on p. 332
- .animate() method allows you to create some of your own effects and animations by changing CSS properties.

## JavaScript and jQuery book by Jon Duckett pages 302-305

- List of jQuery element selectors p. 302-303
- List of jQuery methods p. 304-305

[Back to README](README.md)
