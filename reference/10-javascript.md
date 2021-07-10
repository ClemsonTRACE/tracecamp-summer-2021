# JavaScript

In this curriculum, you will not need to memorize all the JavaScript patterns below. Use this document as a reference, and refer back to it when you need it.

For more information about these topics, check out:

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [javascript.info](https://javascript.info/)

Or, watch:

- https://www.youtube.com/watch?v=hdI2bqOjy3c
- https://www.youtube.com/watch?v=W6NZfCO5SIk

## Setup

### Locally

- Be sure you have NodeJS installed
- Run `npm init -y` to initialize your project
- Create an `index.js` file
- Run the file with `node index.js`.

### Online

- Run online with a [codesandbox](https://codesandbox.io/s) NodeJS template.

## Console

Using the console.log method, you can print content to the terminal. Don’t worry about understanding a method or the syntax yet.

```js
console.log("Hello World!");
```

## Variables

JavaScript has three types of variable declarations: `const`, `let`, and `var`. Use `const` for variables that do not change. Use `let` for variables that change. Try to avoid `var`, but be aware that you may find it in legacy code. You can assign variables with the `=` operator.

```js
const hello = "Hello World!";

let greeting = "hi";
greeting = "hi hi";

console.log(hello); // 'Hello World!'
console.log(greeting); // 'hi hi'
```

### Value types

JavaScript has several builtin value types. You’ve already worked with strings. There are also numbers, booleans, undefined, null, symbols, and BigInt. We won’t cover symbols and BigInt in this review.

```jsx
const myString = "A String of Characters";
const myTemplateLiteral = `
  A
  Multiline
  ${myString}
`;
console.log(myTemplateLiteral);
const myNumber = 3;
const myBoolean = true; // or false
let myUndefinedVariable; // = undefined;
let myNullVariable = null;
```

A template literal is just another way to write a multiline string.

Null and undefined are very similar. On one hand, undefined is a variable that has been not yet been defined. On the other hand, null is a variable that is explicitly nothing (no value).

### Reference types

JavaScript has many reference types: objects, arrays, maps, sets, weakmaps, weaksets, dates, and more. The most common are objects and arrays. Objects hold key and value pairs, while arrays are lists of values.

```js
const myObject = {
  key: "value",
};
const myArray = [1, 2, "fish"];
```

#### Objects

Here are examples on how to access and mutate (change) objects.

```js
// accessing objects
let myCar = {
  maker: "Buick",
  year: 2003,
  key: `
     8 8 8 8                     ,ooo.
     8a8 8a8                    oP   ?b
    d888a888zzzzzzzzzzzzzzzzzzzz8     8b
     '""^""'                    ?o___oP'
  `,
  "Legal Jargon": "tl;dr legal",
};

// accessing and mutating objects
console.log("Old Car:", myCar.year);
myCar.year = 2010;
console.log("New Car:", myCar.year);

// accessing irregular keys
console.log(myCar["Legal Jargon"]);

// accessing objects with variables
const myCarKey = "key";
console.log(myCar[myCarKey]);
```

#### Arrays

Here are examples on how to access and mutate (change) arrays.

```js
// accessing arrays
let groceryList = ["cheese", "more cheese", "CHEESE"];
// zero indexing
console.log(groceryList[3]); // undefined
console.log(groceryList[0]); // 'cheese'

// mutating arrays
console.log(groceryList[1]); // 'more cheese'
groceryList[1] = "tortillas";
console.log(groceryList[1]); // 'tortillas'

// adding and removing items from arrays

// add item to end
groceryList.push("SO MUCH CHEESE");
// remove item from end
groceryList.pop();
// add item to beginning
groceryList.unshift("plates");
// remove item from beginning
groceryList.shift();
```

#### Complex Data Structures

Objects and array can be nested to model complex data. We can chain together our access methods to access this nested data.

```js
const books = [
  {
    title: "Crime and Punishment",
    ratings: [2, 4, 5],
  },
  {
    title: "Programming is Hard",
    ratings: [5, 4, 3],
  },
];
console.log("Nested rating", books[0].ratings[0]); // 2
```

#### JSON

JSON stands for JavaScript Object Notation. It is a very common format for reading and writing data. JSON is similar to the objects and arrays we have already learned, but all keys and strings have to be in "double quotes".

```json
{
  "booksJson": [
    {
      "title": "Crime and Punishment",
      "ratings": [5, 4, 5]
    },
    {
      "title": "Programming is Hard",
      "ratings": [5, 4, 3]
    }
  ]
}
```

## Math

You can perform basic math with JavaScript and use the order of operations. When you change a variable, be sure to set its value.

```js
let myLuckyNumber = 7;
console.log("Plus 1", myLuckyNumber + 1); // 8
console.log("Variable", myLuckyNumber); // 7

// to update, must set the variable
myLuckyNumber = myLuckyNumber + 1; // 8
myLuckyNumber += 1; // 9
myLuckyNumber++; // 10

const myEquation = 1 + (((2 / 3) * 7) % 8);
```

## Conditionals

Conditions are if statements. If this, do that, else do the other thing. To understand conditionals, we must understand equality and truthiness.

### Equality and inequality

- `=` assigns variables
- `==` checks equality and converts types
- `===` strict equality without type conversion (preferred)

```js
// assign variable
const price = 20;

// true, type coersion, try to avoid
console.log(price == "20");

// false, string and number types are not equal
console.log(price === "20");

// true, types are equal
console.log(price === Number("20"));
console.log(price === 20);

// inequalities
console.log(price > 10); // true
console.log(price >= 30); // false
```

### If statements

If statements allow you to run different code depending on the condition. You can run multiple checks with `else if` and run `else` if the previous conditions are false.

```js
let time = 9;
if (time < 12) {
  console.log("Good morning");
} else if (time < 18) {
  console.log("Good afternoon");
} else if (time < 22) {
  console.log("Good evening");
} else {
  console.log("Good night");
}
```

### Truthiness

You do not have to use equalities in if statements, you can just check if a value is truthy or falsy.

```js
let dogName = "Roxie";
if (dogName) {
  console.log(`I love my dog ${dogName}`);
}
```

Be aware that truthy and falsy values are not always what you think they are.

```js
let debt = 0;
if (debt) {
  console.log("Try to save more money this month");
  // 0, false, empty strings, null, undefined, and NaN are all falsey
  // this code will run even if your debt is 0
}
```

### Logical operators

- `||` - Logical OR operator
- `&&` - Logical AND operator
- `!` - Logical NOT operator

```js
let isWeekend = true;
let isMorning = false;
let isWorkDone = true;

if (!isWeekend) {
  console.log("week day");
}
if (isWeekend && isMorning) {
  console.log("snooze");
}
if (isWorkDone || isWeekend) {
  console.log("fun");
}
```

### Ternary operator

The ternary operator is like an `if…else` statement, but it fits in a single expression.

```js
// condition ? exprIfTrue : exprIfFalse
const myLuckyDay =
  myLuckyNumber === 7
    ? "Something good will happen today!"
    : "Better luck tomorrow!";
```

### Immutability

JavaScript objects and arrays are reference types. When you set a variable equal to a reference type, it does not copy it. Rather, both variables now point to the exact same reference in memory.

```js
const myClassSchedule = ["literature", "math", "philosophy"];
const friendClassSchedule = myClassSchedule;

const myGrades = { literature: "B" };
const friendGrades = myGrades;

console.log(myClassSchedule === friendClassSchedule); // true
console.log(myGrades === friendGrades); // true

// Because arrays and objects are reference types,
// Changing one changes both

myClassSchedule[1] = "government";
console.log(myClassSchedule); // ["English", "AP Government", "Philosophy"]
console.log(friendClassSchedule); // ["English", "AP Government", "Philosophy"]

myGrades.literature = "A";
console.log(myGrades); // { literature: "A" }
console.log(friendGrades); // { literature: "A" }

// Make a copy immutably (without a reference)
const tuesdayClassSchedule = [...myClassSchedule];
const fallGrades = { ...friendGrades };

console.log(myClassSchedule === tuesdayClassSchedule); // false
console.log(myGrades === fallGrades); // false

// you can change tuesdayClassSchedule and fallGrades without affecting the origins
```

## Functions

Using functions, it is possible organize and reuse code. There are many ways to write them.

```js
// function keyword
function greeterOne() {
  return "Hello World 1";
}
greeterOne();

// arrow function
const greeterTwo = () => {
  return "Hello World 2";
};
greeterTwo();

// arrow function with implicit return
const greeterThree = () => "Hello World 3";
greeterThree();
```

### Methods

Methods are functions—the only difference is that methods are located on an object or class.

```js
const greeterObject = {
  // function keyword
  greeterFour: function () {
    return "Hello World 4";
  },
  // function shorthand without keyword
  greeterFive() {
    return "Hello World 5";
  },
  // arrow function
  greeterSix: () => {
    return "Hello World 6";
  },
  // arrow function with implicit return
  greeterSeven: () => "Hello World 7",
};

greeterObject.greeterFour();
greeterObject.greeterFive();
greeterObject.greeterSix();
greeterObject.greeterSeven();
```

### Parameters and arguments

When calling functions, you can pass variables. Arguments are the actual variables passed at runtime, while parameters are the variable names in the function definition.

```js
// name and greeting are parameters
let friendlyGreeter = (name, greeting) => `${greeting} ${name}!`;
// "Bob" and "Hi" are arguments
friendlyGreeter("Bob", "Hi"); // Hi Bob!
```

## Destructuring

Destructuring unpacks properties from an object or items from an array and assigns them to variables.

```js
const person = {
  name: "Billy",
  age: 7,
  favoriteColor: "green",
  country: "USA",
};
const { name, age, ...personalInfo } = person;
console.log(name); // "Billy"
console.log(personalInfo); // {"favoriteColor":"green","country":"USA"}

const rgb = ["red", "green", "blue"];
const [firstColor, ...otherColors] = rgb;
console.log(firstColor); // "red"
console.log(otherColors); // ["green", "blue"]
```

### Defaults

When destructuring properties that are optional or may not exist, default values can be set in case they are undefined.

```js
const person = {};
const { name = "Bob" } = person;
console.log(name); // Bob
```

### Renaming

Sometimes, a property can be renamed to provide clarity or prevent naming collisions with other preexisting variables.

```js
const person = { name: "Bob" };
const { name: firstName } = person;
console.log(firstName); // Bob
```

### Renaming with defaults

It is possible to destructure with both default values and renamed values at the same time.

```js
const person = {};
const { name: firstName = "Bob" } = person;
console.log(firstName); // Bob
```

### Destructuring inside a function

```js
function safeGreeter({ name: firstName = "there" } = {}) {
  return `Hello ${firstName}`;
}
safeGreeter();
```

The `= {}` gives an empty object as the default parameter for the function. Otherwise, an error will be thrown when you try to destructure properties from `undefined`.

## Imports

To help organize code, many files are used to hold functions, objects, and more. To access them, use ES6 Modules and the import/export syntax.

```js
// named exports
export const cyan = "cyan";
export const magenta = "magenta";
export const yellow = "yellow";
export const key = "black";

// default export
const cmyk = ["cyan", "magenta", "yellow", "key"];
export default cmyk;
```

```js
// named import
import { cyan, magenta } from "./cmyk";
console.log(cyan, magenta);

// default import with named import
import cmyk, { yellow } from "./cmyk";
console.log(cmyk);

// wildcard imports, imports everything
import * as colors from "./cmyk";
console.log(colors.magenta);
```

## Loops

Often, loops are used to process each item in an array.

```js
let wishList = [];

for (let i = 0; i < wishList.length; i++) {
  wishList[i] = wishList[i].toUpperCase();
}

wishList.forEach((item, index) => {
  wishList[index] = item.toLowerCase()
};

// map returns a new array, while forEach does not
wishList = wishList.map((item) => item.toUpperCase());

const addTwo = (num) => num + 2;
let ratings = [6, 7, 8];

// map takes a function, iterates over each item in the array, and returns a new array
ratings = ratings.map(addTwo);
console.log(ratings); // [8, 9, 10]

// filter takes a function, iterates over each item in the array, and returns a new array with items that are truthy
let ratings = ratings.filter(ratings => rating >= 9)
console.log(ratings); // [9, 10]

// reduce takes a function, and allows you to accumulate all your values together
const average = ratings.reduce((acc, val) => acc + val, 0) / ratings.length;
console.log(average); // 9.5

// Objects
const movie = {
  title: "It’s a Wonderful Life",
  rating: "PG",
  year: "1946",
};

// "title", "rating", "year"
console.log(Object.keys(movie));
// "It’s a Wonderful Life", "PG", "1946"
console.log(Object.values(movie));
// [["title", "It’s a Wonderful Life"], ["rating", "PG"], ["year", "1946"]]
console.log(Object.entries(movie));
```

## Asynchronous functions

Sometimes, operations may not complete immediately—for example, reading files, making requests, or simply waiting a certain period of time.

```js
const callback = () => console.log("callback done");
// callback will be called after 500 milliseconds
const takesTimeCallback = setTimeout(callback, 500);

// however, chaining callbacks are messy
fs.readFile("file-v1.txt", function (err, file1) {
  fs.readFile("file-2.txt", function (err, file2) {
    fs.readFile("file-3.txt", function (err, file3) {
      // all files loaded
    });
  });
});

// promises allow for easier chaining and better error handling
const takesTimePromise = new Promise((resolve, reject) =>
  setTimeout(() => resolve("promise done"), 500)
);
// promise will be resolved after 500 milliseconds
takesTimePromise
  .then((data) => console.log("then", data))
  .catch((error) => console.log(error));

// To write clean code, use the async / await syntax with promises
const start = async () => {
  const takesTimeAsync = await new Promise((resolve, reject) =>
    setTimeout(() => resolve("done"), 500)
  );
  console.log("waited for…", takesTimeAsync);
};
start();
```

### iffe

An iffe is an immediately invoked function expression, which prevents polluting the global object and allows the use of async and await.

```js
(async () => {
  // safe to write asynchronous code here
})();
```

### Asynchronous loops

```js
(async () => {
  const addThree = (num) =>
    new Promise((resolve, reject) => setTimeout(() => resolve(num + 3), 500));

  let grades = [97, 90, 85];
  // [[object Promise] { ... }, [object Promise] { ... }, [object Promise] { ... }]
  // You want the promised result, not the promises themselves
  console.log("grades", grades.map(addThree));

  // parallel
  let roundedGrades = await Promise.all(grades.map(addThree));
  console.log("roundedGrades", roundedGrades); // 100, 93, 88

  // synchronous
  let curvedGrades = [];
  for (const grade of grades) {
    const curvedGrade = await addThree(grade);
    curvedGrades.push(curvedGrade);
  }
  console.log("curved grades", curvedGrades); // 100, 93, 88
})();
```

## Libraries

There are thousands of third party libraries available on npm for JavaScript. Save time and use them in your projects.

meaningOfLife.txt

```txt
42
```

```js
import fs from "fs-extra";

(async () => {
  let meaningOfLife;
  try {
    meaningOfLife = await fs.readFile("./meaningOfLife.txt", "utf-8");
  } catch (error) {
    console.log(error);
  }
  console.log(meaningOfLife.trim());
})();
```

```js
import axios from "axios";

axios
  .get("https://swapi.dev/api/starships/9/")
  .then((response) => console.log(response.data));
```

## Practice

In Nodejs, using [SWAPI](https://swapi.dev/api/planets/) (the Star Wars API):

- Fetch all the pages of the planets (with [axios](https://www.npmjs.com/package/axios))
- Filter out any planets with an unknown population
- Log all planet names with their populations to the console
  - Log any planets with a population over 1 million in green (with [chalk](https://www.npmjs.com/package/chalk))

## Optional

- [Event loop](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
- VS Code plugins
  - [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2)
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  - [TabNine Autocomplete AI](https://marketplace.visualstudio.com/items?itemName=TabNine.tabnine-vscode)

## [Next lesson →](./11-surge.md)
