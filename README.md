# NODE

## About Node

**Node.js** is a cross-platform runtime environment and library for running JavaScript applications outside the browser.

*Node.js is a platform built on Chrome's JavaScript runtime for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.*

<img src="https://www.javatpoint.com/js/nodejs/images/what-is-nodejs.png" alt="parts of node"/>


`Node.js = Runtime Environment + JavaScript Library`

### Features of Node.js

1. **Extremely fast**: Node.js is built on Google Chrome's V8 JavaScript Engine, so its library is very fast in code execution.
2. **I/O is Asynchronous and Event Driven**: All APIs of Node.js library are asynchronous i.e. non-blocking. So a Node.js based server never waits for an API to return data. The server moves to the next API after calling it and a notification mechanism of Events of Node.js helps the server to get a response from the previous API call. It is also a reason that it is very fast.
3. **Single threaded**: Node.js follows a single threaded model with event looping.
4. **Highly Scalable**: Node.js is highly scalable because event mechanism helps the server to respond in a non-blocking way.
5. **No buffering**: Node.js cuts down the overall processing time while uploading audio and video files. Node.js applications never buffer any data. These applications simply output the data in chunks.
6. **Open source**: Node.js has an open source community which has produced many excellent modules to add additional capabilities to Node.js applications.
7. **License**: Node.js is released under the MIT license.


## Installation and Best Practices

### Installation

`sudo apt-get install nodejs npm`

`brew install nodejs`

`npm install package_name`

### Best Coding Practices

1. Use `'` for string in node.


## Node | Basic Understanding


### Logging | Printing

```js
console.log('Hello World!');
> Hello World!
```

### Import modules

```js
var http = require('http');
```

### Data Types

Types of data used in node.

**Types of data**

1. **string**
2. **boolean**
3. **integer**
4. **float**
5. **number**

### Server | Creating and Using It

```js
var http = require("http");  
http.createServer(function (request, response) {  
    // Send the HTTP header   
    // HTTP Status: 200 : OK 
    // Content Type: text/plain  
    response.writeHead(200, {'Content-Type': 'text/plain'}); 
    // Send the response body as "Hello World"  
    response.end('Hello World\n');  
}).listen(8081);  
// Console will print the message  
console.log('Server running at http://127.0.0.1:8081/'); 
```
