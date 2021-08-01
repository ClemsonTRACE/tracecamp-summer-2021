<h1 align="center">
   💥 Day 3: State and Events in React
</h1>

## 🎯 Learning Objectives
- Understand events and how you can interact with your page
- How to write a component with state
- How to render elements on your page conditionally

## 📚 Assigned Reading

Start your adventure today by reading the following article on events...

[Article: React Event Handlers: onClick, onChange](https://www.robinwieruch.de/react-event-handler)

Events are used everywhere in web development. This is what provides interactivity and reactivity to your site.

Now for the fun part: state. State is a critical concept in programming and has many layers of complexity. There are many philosophical discussions on state such as when to use it, the dangers of it, and best practices in different paradigms and contexts. You can simply describe state as the "state of the world." Whatever happens in the world, changes the world's state. In our context, the world is your site. We will eschew any further philosophical explanations of state for now and recommend that you just think of state as the state of your site as different events (which you read about earlier) occur on it. Read the following article:

[Article: React hooks introduction, useState - educative.io](https://www.educative.io/edpresso/react-hooks-introduction---usestate)

Now that you have a basic idea of how useState works in react, you can now walk through this tutorial on making a simple tic-tac-toe game:

[https://medium.com/@shifrb/how-to-build-tic-tac-toe-with-react-hooks-ca37f6040022](https://medium.com/@shifrb/how-to-build-tic-tac-toe-with-react-hooks-ca37f6040022)

## 📔 Project
Develop a memory game. Your game should contain a grid of boxes (recommended 3x3). The boxes will blink in a specific order. The user will be prompted to click the boxes in the order they just watched. They continue if they get it correct, otherwise the game ends. The box order remains the same but increases in length by one additional blink on each correct input by the player. The game should have a start screen and an end screen.

**Feature Requirements**

- Create a start screen
- Create a grid with clickable boxes
- Have a "next" button to go to the next "blink"
- Every "round" adds a new blink
- Game ends if wrong
- Create a game end screen

**Stretch Goals (implement 3+ of these features for extra points)**

- A score count above the grid
- Final score when you lose
- Random box pattern every game
- Increasingly shorter blinks as the game continues (increasing difficulty)
- Game modes
- Replay game on end screen
