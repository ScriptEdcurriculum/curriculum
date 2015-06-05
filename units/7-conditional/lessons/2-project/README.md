# High low

![image](http://i.imgur.com/pQ1BCwf.jpg)

##Scope

This project involves implementing the core functionality for a simple high low game. The objective of this project is for students to practice conditional logic using `if/else` statements.
 
##Before Class

### Prerequisites
Students should only start this project after they have completed the other lessons in the unit.

### Starter code

See [here](starter_code/) for code and [here](https://rawgit.com/ScriptEdcurriculum/curriculum/master/units/7-conditional/lessons/2-project/starter_code/index.html) to view.

### Solution code

See [here](https://github.com/ScriptEdcurriculum/solutions/tree/master/units/7-conditional/lessons/2-project/solution_code) for code (private).

### Assessment

1. Write do-now based off of [assessments from previous lesson](../../../7-conditional/lessons/1-conditional/assessments/).

##During Class

###Do Now

1. Attendance: Teacher takes student attendance at www.kinvolved.com
2. Return graded do-now and exit ticket from previous class
3. Do-now quiz

###Opening

Let's play high low together as a class. I'm going to select a random number between 1 and 10 in my head. Your job is to guess the number. I can only say "too high", "too low", or "correct".

###Lecture
You are going to build the guts of a high low game. You will be given starter code. Your instructions are:

#### 1. `generateRandomNumber()`

Modify the following function in the `js/guts.js` file:

```
function generateRandomNumber() { }
```

This function must generate a random number between 1 and 10 and then return it.

#### 2. `checkGuess(guess, generatedRandomNumber) `

Modify the following function in the `js/guts.js` file:

```
function checkGuess(guess, generatedRandomNumber) {}
```
The function receives two parameters: `guess` which contains the number guessed by the user and `generatedRandomNumber` which contains the result from `generateRandomNumber()`. Use `console.log()` to check the parameter values.

This function contains two variables:

* statusCode: this variable must be set to 0 if the user guessed correctly, 1 if the user guessed too high, and 2 if the user guessed too low.
* statusMessage: this variable must be set to a message based upon which of the three scenarios the user falls in.

Be sure not to change any code that is already there.

###Brainstorming
Before you start coding, identify the list of steps you need to do to finish this project. Here's a start:

1. What kind of conditional logic will you need? Write pseudo-code on paper using `if` and `else` statements.
2. Bring the starter code into your own environment.
3. Solve for just the success scenario first. Get that working before moving on to the other two scenarios.

###Build Time
Students will work alone on this project. The teacher's role will be to walk around the room helping students with any questions they have. Students are encouraged to look at previous lessons for reference.

###Extension Activities
Students who complete the project at hand early may attempt to improve their project by including the following:  

* Added CSS for visual customization
* Create a counter that only allows the user 4 guesses before the program terminates.
* Create a system where the user is awarded a certain number of points based on the amount of guesses it took to find the random number. 
* Create a "Reset random number" button.
* Prompt the user to choose a difficulty (Easy, Medium, Hard). Difficulty can be increased by making the range of numbers to choose from larger.

##Closing
Select students to present their work to the class.

###Check for Understanding
Teachers should keep track of student success while they are presenting to the class.

###How to Submit
The teacher must ask students to share the link to their project on your school's [Project Submission Form.](https://docs.google.com/a/scripted.org/spreadsheets/d/1kaVH9hmkDCbBul19583UMPxl6IJ3-4pHgBQ2BU6TKDk/edit#gid=0)

Also remind students to add a link to their project on their About Me page.
