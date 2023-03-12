# Automated Testing with Jest and JavaScript

This repository contains a simple example of how to use Jest to write and run automated tests in JavaScript

## 💻 Installation

To use Jest in your project, you need to install it as a development dependency. You can do this using npm, with the following command in the terminal:

```
npm install --save-dev jest
```

## ⚙ Usage

Tests are written in separate files from your code, in a directory called __tests__. By convention, test files are named with the suffix .test.js.

Let's use the sum function as an example, which takes two numbers as parameters and returns their sum. The test file would look like this:

```
// __tests__/sum.test.js

const sum = require('../sum');

test('adds two numbers', () => {
  expect(sum(1, 2)).toBe(3);
});
```

In this example, we are importing the sum function from the sum.js file and testing whether it returns the correct value for the parameters 1 and 2. The expect function is a Jest function that defines the expected value, and the toBe method checks whether the function result is equal to the expected value.

Now let's create the sum function in the sum.js file:

```
// sum.js

function sum(a, b) {
  return a + b;
}

module.exports = sum;
```

The function simply returns the sum of the two parameters.

With the code and tests created, we can run the tests using Jest. To do this, simply run the following command in the terminal:

```
npx jest

```

Jest will look for test files in the __tests__ directory and run them. If everything is working correctly, you should see a success message in the terminal.
## ✨ Technologies

This project was developed with the following technologies:

- [TypeScrip](https://www.typescriptlang.org/)
- [Jest](https://jestjs.io/pt-BR/)

## 🔗 Find me!
- Linkedin: https://www.linkedin.com/in/italo-santos-dev/
- Instagram: https://www.instagram.com/italosantsz/
