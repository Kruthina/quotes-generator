

## Getting started

[![NPM](https://nodei.co/npm/inspirational-quotes.png?compact=true)](https://nodei.co/npm/inspirational-quotes/)

```
$ npm install --save inspirational-quotes
```

## Installation


This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/).

Before installing, [download and install Node.js](https://nodejs.org/en/download/).

Installation is done using the
**[`npm install`](https://docs.npmjs.com/getting-started/installing-npm-packages-locally)** command:

```bash
$ npm install inspirational-quotes
```

## Usage

```js

const Quote = require('inspirational-quotes');

console.log(Quote.getQuote()); // returns quote (text and author)
console.log(Quote.getQuote({ author: false }); // return quote without author
console.log(Quote.getRandomQuote()); // return any random quote

```

- ***getQuote()*** method returns an object containing ***text*** and ***author***.

```json
 {  
    "text":"My number one piece of advice is: you should learn how to program.",
    "author":"Mark Zuckerberg, founder of Facebook"
 }
 ```

- ***getRandomQuote()*** method returns a random **inspirational** quote : *`You miss 100 percent of the shots you don’t take.`*

### Options

Additionally you can provide `options` to `getQuote` method. By default `{ author: true }` is used. 

```js

getQuote({ author: false });

```

-  `{ author: true }`: Returns a quote with author information
-  `{ author: false }`: Returns a quote without author information

> **Note**: Recommended to use `getQuote` with `{ author: false}` option instead of `getRandomQuote` as it will be deprecated in the further versions. It's available just to ensure the backward compatability.

## Examples

To view the examples, clone the **inspirational-quotes** repo and install the dependencies:

```bash
$ git clone https://github.com/vinitshahdeo/inspirational-quotes.git
$ cd inspirational-quotes
$ npm install
```

Then run the [`examples/index.js`](./examples/index.js):

```bash
$ node examples
```

## Tests

- `npm run test`: Runs unit tests
- `npm run test-lint`: Run lint tests

