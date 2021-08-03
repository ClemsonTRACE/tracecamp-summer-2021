<h1 align="center">
   🗃 Day 5: useEffect, localStorage, and JSON
</h1>


## 🎯 Learning Objectives

- The React component lifecycle (mount, unmount/cleanup) and how to use **useEffect** to hook into it
- How to save and retrieve data from the browser's **localStorage**
- How the **JSON.stringify** and **JSON.parse** functions can be used to convert js objects into string form

## 📚 Resources

- [In-depth Explanation of The useEffect Hook](https://dev.to/mpodlasin/react-useeffect-hook-explained-in-depth-on-a-simple-example-19ec)
   - Dives into the using the useEffect hook using specific examples to show the properties of the React component lifecycle.
- [Official Introduction to The useEffect hook](https://reactjs.org/docs/hooks-effect.html)
   - Similar to the first resource, but references the older version of react to explain the same concepts.
- [Stringify and Parse](https://javascript.plainenglish.io/how-to-use-stringify-and-parse-in-javascript-6b637b571a32)
   - Breif introduction to the JSON.stringify and JSON.parse functions with a couple examples for each.


## 📔 Assignment

Create a persistent notes app, in which the user can type out text and save it for viewing later. There will need to be a large textarea input element for this functionality. Then the user will be able to save their work by clicking a button. When the page loads the next time, the text will be loaded without asking.

**Feature Requirements**

- A large text area for the user to type in
- Text in the text area is populated with any prior text (stored in local storage) if present.
- The user can save current text by clicking a button
- Make an indicator to show the user whether the current text is saved or not

**Optional Features**

- The user also has the option to enable auto-saving with a toggle or checkbox. This will save the input of the text field on every change of the text.
- Ability to make multiple notes. This can be either a set number of notes or a variable amount with addition or deletion.
- Add any flourish you like! if you can sell us on it we can award a point for it 🙂
