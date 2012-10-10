# NodePDF

Down and dirty PDF rendering in Node.js

## Installation

````
npm install nodepdf
````

## Dependencies

1. PhantomJS

## API

````
var NodePDF = require('nodepdf');

var pdf = new NodePDF('http://www.google.com', 'google.pdf');

pdf.on('error', function(msg){
	console.log(msg);
});

pdf.on('done', function(msg){
	console.log(msg);
});

````