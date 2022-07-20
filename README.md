# MWA Homework 03 - NodeJS 02
  
## Exercise 01
Given a file located at the same folder `data.json` which contains the following JSON structure:
```json
[{"id": 1, "name": "Asaad Saad"}, {"id": 2, "name": "Mike Saad"}]
```
* Create a class named `Names`, once instantiated, it reads the JSON file synchronously, and assigns its content to an instance property.
* Add a method `getNames()` to emits the details about all the names with an event `names_all`.  
* Add a method `getNameById(id)` to emits the details about the given `id` with an event `names_single`. 
* Add a method `removeNameById(id)` to remove the details about the given `id` and emit an event `names_deleted`.  
* Add a method `persist()` to write back the instance property of the names into the `data.json` file,  emit an event `names_saved` when the file is written successfully.  
  
Test you code: create an instance of `Names` class, call all the methods and listen to all emitted events, print appropriate messages.
  
## Exercise 02
Write an **asynchronous** Node program that has a function `checkSystem()` that returns a Promise object and checks if the system memory size is at least 8 GB and the processor has at least 4 cores (use `os` core module).  
* When you call the function, the console shows a message `Checking your system…`
* If the system doesn't have enough memory we should reject with a message: `This app needs at least 4 GB of RAM`
* If the system doesn't have at least 4 cores, reject with this message: `Processor is not supported`
* If the system has enough specs, resolve with the following message `System is checked successfully.`  
  
Note: use `async/await` when calling the function.
  
## Exercise 03
Create a web server that's going to send a response of big file (bigger than 500MB) to any client that sends a request to your specified server:port.  
Solve this question in three different ways and inspect the loading time in the browser, try to send many requests at the same time to observe performance differences, and write down your observations.
* Use `readFileSync`
* Use `readFile`
* Use streams API

