<h1 align="center">
   Day 3
</h1>

<h3 align="center">

</h3>

### ****🎯 Learning Objectives****

- Learn about JavaScript objects
- Learn using JavaScript objects for state
- Learn to use array functions in your React code

### **📚 Assigned Reading**

- [W3 page on JavaScript Objects](https://www.w3schools.com/js/js_objects.asp)
    - If you are already familiar with JavaScript objects, you can skip this.  If you are not, I encourage you to read through at least the 'Accessing Object Properties' section.
- [Web Dev Simplified's Learn useState in 15 Minutes - React Hooks Explained](https://www.youtube.com/watch?v=O6P86uwfdR0)
    - A very nice, simple review of the useState hook for React that also touches on how to handle useState on JavaScript objects.
- [Anthony Sistilli's Learn React #5: Maps and Loops in JSX](https://www.youtube.com/watch?v=5llXA0RTYIU)
    - An introduction to using the map function to turn data, such as a JavaScript object into a React component.
- [Web Dev Simplified's 8 Must Know JavaScript Array Methods](https://www.youtube.com/watch?v=R8rmfD9Y5-c)
    - A quick but solid introduction to several JavaScript array methods.  Pay particular attention to filter and map as they will both be in the assignment
- [GeeksForGeeks article on array method chaining](https://www.geeksforgeeks.org/chaining-of-array-methods-in-javascript/)
    - In the assignment, you will be expected to filter and map the same array.  Normally, you might have to assign the result of the filter to a variable then map that variable.  This is a way to write code that does the same thing, but is far more readable.

Additional resources:

- (optional) [Javascript page](https://github.com/ClemsonTRACE/tracecamp-summer-2021/blob/main/tracecamp-docs/10-javascript.md#destructuring)  The destructuring and loops sections of the JavaScript resource page touch on today's topics
- (optional) [16.8: Array Functions: filter() - Topics of JavaScript/ES6](https://www.youtube.com/watch?v=qmnH5MT_luk) A more casual, down to earth introduction to the filter array function in particular.
- (optional) [MDN page on spread syntax (...)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax) The spread operator is an invaluable tool when it comes to working objects and arrays in JavaScript.  It gets briefly touched on in the videos, but not in as much depth as I would like, so here is the documentation.

### **📔 Project**

Create a To-do list in React\
If you're struggling to get started or want a decent starting point for the add new items form I wrote some starter code for this one:
[Starter Code](https://github.com/corey-andrews/Todo-Template)

Core requirements:

- Store the items in an array of objects with *at least* the following properties:  title, description, id, and stillTodo. (you may rename the properties if you like)
- Use map to dynamically turn your array of objects into components.  Have file for this component.
- Todo component should display title, description, have a way to delete this item, and have a way to mark the item as finished. (or unmark it if it is already marked)
- Give the user a way to filter out or show completed items
- Have a way for the user to add new items to the to do list (I recommend using a form to allow the user to enter a title and description)

Stretch Goals:

- Add your own styling
- Use a modal for adding an element (see tutorial from day 2)
- Allow users to sort todo list by title or id number
- Get creative! Webdev is about making stuff. Feel free to experiment.
