<h1 align="center">
   Day 2
</h1>

<h3 align="center">
   Intro to React
</h3>

## 🎯 Learning Objectives
- Learn how to set up a React project
- Learn how to write and use React components
- Learn how to use props to produce dynamic components

## 📚 Assigned Reading
- [React Crash Course for Beginners 2021 - YouTube](https://www.youtube.com/watch?v=Dorf8i6lCuk&t=1008s) **(16:48-1:28:15)**
    - Please start from the section "Creating a React Project" (starts: 16:48) and watch through the section "Event Props" (ends: 1:28:15). The first 16:48 is useful information but not applicable to this camp, so it has been omitted.

Additional resources:

- We recommend using [Surge](https://surge.sh/help/getting-started-with-surge) to deploy React apps for projects.
- (optional) [React Developer Tools](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en) is an incredibly useful tool for debugging React in the Chrome and Firefox web browsers.
- (optional) [Install Tailwind CSS with Create React App [tailwindcss.com]](https://tailwindcss.com/docs/guides/create-react-app) - instructions on how to setup TailwindCSS in your React project
- (optional) For CS Majors, our instructor Houston has made [an introduction to React](https://github.com/ClemsonTRACE/tracecamp-summer-2021/blob/main/curriculum/week-1/Declarative-JavaScript.org) centered around teaching the ***declarative development paradigm*** as opposed to the imperative paradigm taught in most CS contexts.
- (optional) [Getting started with React [MDN Docs]](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_getting_started) - This is Mozilla's React tutorial.  It has a similar project to the one used in our lesson.  If you prefer a text based tutorial to a video one, this one is highly recommended.  We get through "Componentizing our React App".  Downsides of this tutorial include: a simpler visual design and no introduction to Prettier.
    - To supplement the lack of an introduction to Prettier in the Mozilla tutorial, [here is a text tutorial](https://www.digitalocean.com/community/tutorials/code-formatting-with-prettier-in-visual-studio-code) on using Prettier to format your code.
- (optional) For a more casual breakdown of introductory React material, a few of us on the team really appreciated [Dev Ed's React Tutorial For Beginners](https://www.youtube.com/playlist?list=PLDyQo7g0_nsVHmyZZpVJyFn5ojlboVEhE).  In particular, I found the first video did an excellent job of breaking down what all the files from create-react-app do as well as introducing many of the basic concepts we went over in this lesson.
- <b>NOTE</b>: in older React code, you will see the line `import React from 'react'` at the start of basically every file.  As of React 17, this is no longer necessary.
- <b>NOTE</b>: any time you use the syntax `function foo(bar) {}`, it is possible to use the syntax `const foo = (bar) => {}`.  I personally like this syntax, but it introduces compatibility issues with Internet Explorer.  As IE users aren't real and cannot hurt you, I am willing to sacrifice that use case.  That said, if you may get an industry job working with React, it is potentially worth it to get in the habit of using classic function syntax as opposed to arrow functions

## 📔 Project
Rewrite your personal page from the pre-work as a react app.

Core requirements:

- <b>Divide your code into components and put those components into their own files in a components folder</b> (hint: I used the main structural components: the header, the introduction, the about section, the pets section, and the trademark; and repeated code: cards and pets)
- <b>Make your code readable</b> (hint: the VSCode extension ***Prettier*** helps make your code readable)
- <b>Publish code publicly on Github</b>
- <b>Deploy your code online</b> (We strongly recommend using surge.sh for this)
- <b>Post a link to the Github repository page and your deployed website</b>

Stretch Goals:

- Use states and conditional rendering to mimic page navigation between the different sections of your website
- <i><b>Get creative!</b></i> Webdev is about making stuff. Feel free to experiment.
