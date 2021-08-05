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
   - Don't worry if you don't understand _componentDidMount_, _componentDidUpdate_, and _componentWillUnmount_, they are old and unimportant because they have been replaced by useEffect.
- [Stringify and Parse](https://javascript.plainenglish.io/how-to-use-stringify-and-parse-in-javascript-6b637b571a32)
   - Breif introduction to the JSON.stringify and JSON.parse functions with a couple examples for each.
- [MDN Docs: Window.localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)
   - Very brief intro to localStorage
- [YouTube, Ben Awad: React Persist State to LocalStorage with useEffect](https://www.youtube.com/watch?v=fTP2gi7e3k8)
   - More in-depth guide to using localStorage in React

Optional resouces:
- [Stack Overflow: What is "Mounting" in React.js?](https://stackoverflow.com/questions/31556450/what-is-mounting-in-react-js): It is helpful to know what "mounting" means when talking about the lifecyle of a React component
- [dev.to: useEffect explained with lifecycle methods](https://dev.to/prototyp/react-useeffect-explained-with-lifecycle-methods-296n): If you're interested in understanding how React worked before February 2019, this explains how to use useEffect to accomplish the tasks of the old lifecycle methods it has replaced (_componentDidMount_, _componentDidUpdate_, and _componentWillUnmount_).
- [Reddit comment giving a simplified guide to using useEffect](https://www.reddit.com/r/reactjs/comments/lpkwrh/am_i_the_only_one_who_finds_react_lifecycle_hooks/goc3d2d/)



## 📔 Assignment

Create a persistent notes app, in which the user can type out text and save it for viewing later. There will need to be a large textarea input element for this functionality. Then the user will be able to save their work by clicking a button. When the page loads the next time, the text will be loaded without asking.

**Feature Requirements**

- A large text area for the user to type in
- Text in the text area is populated with any prior text (stored in local storage) if present.
- The user can save current text by clicking a button
- Make an indicator to show the user whether the current text is saved or not
- The user also has the option to enable auto-saving with a toggle or checkbox. This will save the input of the text field on every change of the text.

**Optional Features**

- Ability to make multiple notes. This can be either a set number of notes or a variable amount with addition or deletion.
- Add any flourish you like! if you can sell us on it we can award a point for it 🙂
