# JS-Quiz
1. Create a CustomerOrder class with properties: orderId (string), items (array of objects with name, quantity, price), and status (string).
    Add a method calculateTotal() that returns the total order amount. Write an async method, processPayment(), that simulates payment with a
    Promise that resolves after 2 seconds. After calling the method, change the status to "paid" and print a success message.

   Pseudo-code
 1:  Create a class called CustomerOrder with properties
 a. orderId:(string)
 b. items: an array of objects where each object has a name (string), quantity (number), and price (number)
 c. Status:(string) Current status of the order
 2: Create two methods
 a. calculateTotal()
 Initialize a variable total to 0
 Loop through each item in the items array
For each item, multiply the quantity by the price
 Add the result to the total
Return the total amount
 b. processPayment() and async method
  Returns a promise that waits for 2 seconds and after two seconds resolves successfully and after the Promise resolves
  The status property changes to paid, and a success message is printed, including the  orderId and the new status of the order
2. Create a TeamMember class that takes a name, a role, and an array of tasks (each task is an object with a title and a completed boolean). Write a prototype method, completeTask(taskTitle,) that marks a task as completed. Write another method, checkProgress(,) that returns a Promise resolving to "All tasks completed!" or rejecting with "Pending tasks remaining" based on the state of the tasks array.
  pseudocode
// ## Question 2
// ### Input
// - Name as a string
// - Role as a string
// - Tasks as an array
// ### Process
// 1. Create a class called TeamMember
// 2. Create a constructor for the class and give it attributes of name,role, and tasks
// - Name:string
// - Role:string
// - Tasks:array of objects
// 3. Create prototype method that marks tasks as completed with a parameter of taskTitle using control flow and a loop to iterate through ech task of the task array.
// if completed in task = true then
// log to the console taskTitle was completed
// else log to the console taskTitle incomplete
// 4. Create another method that checks the team member's progress using an asynchronous function
// create a promise function and pass it the value of taskTitle then if it contains completed resolve with 'All tasks are completed' else resolve with 'Pending tasks remaining'
// ### Output
// - Task status as a string
// - Progress status as a string

  3. Create a Candidate class with properties: name, position, and interviews (array of objects with date, status).
  Add a method scheduleInterview(date) that pushes a new interview with status "pending". Then write an async function sendConfirmation() 
 that returns a Promise that resolves after 1 second with a message "Interview confirmed with [name]", and logs the message.
 
 Pseudocode
 1. Create a class Candidate with constructor properties  name, position, and interviews with an empty array.
2. Create a method scheduleInterview that takes in a date.
3. Within scheduled interview, create a new Interview object with date and status = "pending".
4. Push newInterview into this. Interviews array.
5. Create an async method sendConfirmation().
6. Inside sendConfirmation, return a Promise that waits 1 second using setTimeout.
7. After 1 second, resolve the Promise with the message "Interview confirmed with [name]".
8. When Promise resolves, log the message.
9. Create an array of interviews with two interview objects with dates and status.
10. Create a new Candidate instance with name and position.
11. Call scheduleInterview("2025-06-09") on candidate instance.
12. Call sendConfirmation() on candidate instance.
13. Log candidate interviews.

    //4. Design a Course class with properties: title, instructor, and students (an array of student objects with name and progress).
//  Add a method updateProgress(studentName, value) that modifies the student’s progress. Create an async method 
// generateCertificate(studentName) that returns a Promise resolving only if the progress is 100, otherwise rejects 
// with "Incomplete progress".

//Pseudocode
//1. Create a class with a function constructor taking in, title, an instructor, and an array of students
//2. Add a function updateProgress that takes in studentName and value that updates the student's progress
//3.Create an async method taking in a student's Name that returns a promise resolving only when the student's progress is 100, otherwise incomplete progress

 //5. Create a StockTracker class with a property watchlist (an array of objects with symbol, threshold, and currentPrice). 
//Add a method updatePrice(symbol, newPrice) that updates the stock’s current price. Write an async method, checkAlerts() 
//that loops through the watchlist and returns a Promise resolving with a list of stocks where currentPrice >= threshold,
 //or rejecting with "No alerts triggered".

// Pseudocode:
// 1.Create a class StockTracker
//2. Create a function constructor watchlist which is an array of symbols, a threshold, and the current Price.
//3. Create a function that takes in a symbol(String),newPrice(Int) to update the stock's current price.
// 4.Create an asynchronous method checkAlerts to loop through the watchlist and return alerts when currentPrice>=threshold 
//or  "No alerts triggered"
