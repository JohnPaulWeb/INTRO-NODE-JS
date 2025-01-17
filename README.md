# INTRO-NODE-JS

NodeJS


What is Node.js?
Node.js is an open source server environment
Node.js is free
Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
Node.js uses JavaScript on the server

Why Node.js?
Node.js uses asynchronous programming!
A common task for a web server can be to open a file on the server and return the content to the client.
Here is how PHP or ASP handles a file request:
Sends the task to the computer's file system.
Waits while the file system opens and reads the file.
Returns the content to the client.
Ready to handle the next request.
Here is how Node.js handles a file request:
Sends the task to the computer's file system.
Ready to handle the next request.
When the file system has opened and read the file, the server returns the content to the client.
Node.js eliminates the waiting, and simply continues with the next request.
Node.js runs single-threaded, non-blocking, asynchronous programming, which is very memory efficient.

What Can Node.js Do?
Node.js can generate dynamic page content
Node.js can create, open, read, write, delete, and close files on the server
Node.js can collect form data
Node.js can add, delete, modify data in your database




 Example of Modules


To include module 
var http = require('http');

Now we have to create a server he has access in HTTP
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.end('Hello World!');
}).listen(8080)


To Setup ur Project

Install the NodeJs - SetUp
Create a project - CMD - Command Prompt


var url = require('url');
var adr = 'http://localhost:8080/default.htm?year=2017&month=february';
 Example URL


var q = url.parse(adr, true);

console.log(q.host); //returns 'localhost:8080'
console.log(q.pathname); //returns '/default.htm'
console.log(q.search); //returns '?year=2017&month=february'

var qdata = q.query; //returns an object: { year: 2017, month: 'february' }
console.log(qdata.month); //returns 'february'



NPM INSTALL 

NPM is a package manager for Node.js packages, or modules if you like.
www.npmjs.com hosts thousands of free packages to download and use.
The NPM program is installed on your computer when you install Node.js

What is a Package?
A package in Node.js contains all the files you need for a module.
Modules are JavaScript libraries you can include in your project.

Download a Package
Downloading a package is very easy.
Open the command line interface and tell NPM to download the package you want.
I want to download a package called "upper-case":

