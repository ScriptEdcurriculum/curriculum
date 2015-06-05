# Movie search engine

![image](http://i.imgur.com/HuUsZQy.jpg)

##Scope

This project involves implementing the core functionality for a simple client side movie search engine. The objective of this project is for students to practice their skills with arrays, loops, and strings.
 
##Before Class

### Prerequisites
Students should only start this project after they have completed the other lessons in the unit.

### Starter code

See [here](starter_code/) for code and [here](https://rawgit.com/ScriptEdcurriculum/curriculum/master/units/8-array-loop/lessons/3-project/starter_code/index.html) to view.

### Solution code

See [here](https://github.com/ScriptEdcurriculum/solutions/tree/master/units/8-array-loop/lessons/3-project/solution_code) for code (private).

### Assessment

1. Write do-now based off of [assessments from previous lesson](../../../7-array-loop/lessons/2-loop/assessments/).

##During Class

###Do Now

1. Attendance: Teacher takes student attendance at www.kinvolved.com
2. Return graded do-now and exit ticket from previous class
3. Do-now quiz

###Opening

What is a search engine? Give me an example of one. Are there others? What is a query?

How does a search engine work?

Has anyone ever used IMDB? Let's search for some movies together on IMDB. 

###Lecture
You are going to build the guts of a basic movie search engine. At the end, the user should be able to search for movies and see the appropriate results. 

Here are your instructions. Follow them in order:

#### 1. `addMovies()`

Modify `js/guts.js` and add a function called `addMovies()` to it. This function does not take in any parameters. This function returns an array of strings where each string represents a movie.

#### 2. `searchMovies(movies, query)`

Modify `js/guts.js` and add a function called `searchMovies(movies, query)` to it. This function takes in two parameters: an array of movies (again, stored as strings) and a search query. This search query is a string and represents what the user is searching for. Use `console.log()` to verify these statements.

This function must search the `movies` array based on the query. It must return an *array of indices* of any matches. These indices are of any matches in the `movies` array.

For example, suppose the `movies` array contains "Captain America", "Transformers", "The Road", and "Road to Perdition". Suppose the query is "road". This function would return an array with two elements: 2, 3.

#### 3. `getNoMoviesFoundText()`

Modify `js/guts.js` and add a function called `getNoMoviesFoundText()` to it. This function does not take in any parameters. This function should return a string that contains the message you want displayed to the user when there are no movies matching their search query.

#### 4. `getMoviesFoundText(numberMatches)`

Modify `js/guts.js` and add a function called `getMoviesFoundText(numberMatches)` to it. This function takes in one parameter: `numberMatches` represents the number of movies that matched the user's search query. This function should return a string that contains the message you want displayed to the user when there are movies found that match their search query.

#### 5. `printFoundMovies(indices, movies)`

Modify `js/guts.js` and add a function called `printFoundMovies(indices, movies)` to it. This function takes in two parameters: `indices` represents an array of indices into the `movies` array of matched movies; `movies` is an array containing all movies. This function should return an array of strings. Each string should be a movie that matches the user's search query.

###Brainstorming
Before you start coding, identify the list of steps you need to do to finish this project. Here's a start:

1. Draft a small list of movies that will be in your movie database. Then come up with several test cases. What is in the input (search query) and output (search results) in each test case? Do this on paper.
2. Write pseudo-code for each of the functions above on paper.
3. Bring the starter code into your own environment.

###Build Time
Students will work alone on this project. The teacher's role will be to walk around the room helping students with any questions they have. Students are encouraged to look at previous lessons for reference.

##Closing
Select students to present their work to the class.

###Check for Understanding
Teachers should keep track of student success while they are presenting to the class.

###How to Submit
The teacher must ask students to share the link to their project on your school's [Project Submission Form.](https://docs.google.com/a/scripted.org/spreadsheets/d/1kaVH9hmkDCbBul19583UMPxl6IJ3-4pHgBQ2BU6TKDk/edit#gid=0)

Also remind students to add a link to their project on their About Me page.
