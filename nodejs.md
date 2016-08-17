# NodeJS

`node [options] [v8 options] [script.js | -e "script"] [arguments]`

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
