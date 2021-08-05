<h1 align="center">
   🌐 Day 6 - Promises, APIs, Axios
</h1>

## 🎯 Learning Objectives

- Understand how to use **promises** to handle asynchronous calls effectively
- Be able to communicate with an **API** using **Axios**

## 📚 Resources

- [MDN Using Promises Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)
   - One of the harder concepts in JS to wrap your head around; this guide goes over solely using promises. If you want to learn about the inner workings of promises and what is actually going on when they are employed, it is recommended that you read this [MDN Promises Page](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise). It goes over some of the finer details.

- [Quick Async/Await Introduction](https://javascript.info/async-await)
   - Does not go into the details of promises, but shows the syntax behind the asynchronous features in javascript. You may not need this syntax for this assignment, but is a key feature that is common in code involving requests.

- [Axios with React Youtube Tutorial](https://youtu.be/bYFYF2GnMy8)
   - Walks through using Axios to make a request and storing the result in state within a component.

Additional Resources:

- [Node.js overview of async-await feature](https://nodejs.dev/learn/modern-asynchronous-javascript-with-async-and-await) - Similar to the first resource, but this one also explains some of the reasoning behind the syntax.

## 📔 Assignment

For this project you will make a trivia game using the free Open Trivia Database api. The app will contact the api to get a question and the user will then answer the question to get points. The amount of questions they answer in a row should be displayed. I recommend using the single question true/false endpoint, like this `https://opentdb.com/api.php?amount=1&type=boolean`; as handling true or false is easier than storing all of the possible answer choices for multiple choice.

Heres a template repository if you don't want to re-setup create-react-app, tailwind, or axios every time: [https://github.com/Mjtlittle/tracecamp-cra-template](https://github.com/Mjtlittle/tracecamp-cra-template).

And here is an example implementation of this project, feel free to diverge from this as much as you want: [https://tracecamp-2021-day6-example.surge.sh/](https://tracecamp-2021-day6-example.surge.sh/). This is just an example of how it could be done. 

**Feature Requirements**

- The website must contact the api to retrieve a trivia question to display to the user
- Players can then answer the question via some form of input
- The game must keep track of the current streak of answering questions

**Optional Features (Extra point for each feature added)**

- Keep track of the user's highest streak
- Notify the user that their answer was right or wrong with
- Add multiple screens like a main menu or for game over
- Make the questions timed, and end the player's streak when they don't answer in time
