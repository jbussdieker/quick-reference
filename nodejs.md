# NodeJS

[Node.js®](https://nodejs.org) is a JavaScript runtime built on Chrome's V8 JavaScript engine

`node [options] [v8 options] [script.js | -e "script"] [arguments]`

## Background

Node.js was started by Ryan Dahl. It was supported by Joyent which lead to conflicts and io.js was started but then merged back into Node.js with v4.

## Hello World

````javascript
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello World\n');
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});
````

````
$ node example.js
Server running at http://127.0.0.1:3000/
````

## Packaging

[npm](https://www.npmjs.com) is the package manager

## Task Running

[grunt](http://gruntjs.com) is a task runner
