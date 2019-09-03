# MWA Homework 03 - NodeJS 02
## Exercise 01
Create a simple Node script that converts `www.mum.edu` domain name to the equivalent IP address.  
Use `dns` core module, `resolve4()`.  
Note: Use `async/await` after converting the callback function to a `Promise` object.
  
## Exercise 02
* Build a pseudo-class named `Gym` that emits a `boom` event every 1 second.  
* Add a method `rest()` to stop the interval.  
* Create an instance of `Gym` and bind to the `boom` event, printing `Athlete is working out` every time it gets one.
  
## Exercise 03
Write an asynchronous Node program that has a function `checkSystem()` that checks if the system memory size is at least 4 GB and the processor has more than 2 cores (use os core module).  
* When you call the function, you should receive an immediate message on the console `Checking your system…`
* If the system doesn't have enough memory we should print a message to the console: `This app needs at least 4 GB of RAM`
* If the system doesn't have at least 2 cores, print this message to the console: `Processor is not supported`
* If the system has enough specs, print the following message `System is checked successfully.`
  
## Exercise 04
Create a web server that's going to send a response of big file (bigger than 500MB) to any client that sends a request to your specified server:port.  
Solve this question in many different ways and inspect the loading time in the browser and send many requests at the same time to observe performance differences, and write down your observations.
* Use `readFileSync`
* Use `readFile`
* Use streams API

