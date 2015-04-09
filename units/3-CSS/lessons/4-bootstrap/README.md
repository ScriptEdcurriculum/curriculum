#Lesson 4 - Twitter bootstrap

![image](http://i.imgur.com/RpE7nCs.jpg)

## Before class

### Objective

Students will be able to use the basics of Twitter bootstrap's CSS offerings.

### Key points

* Twitter bootstrap is a CSS and JavaScript library.
* Twitter bootstrap contains a collection of styles that we can apply to our own HTML elements.
* Twitter bootstrap makes it easier to create a simple and clean looking page.

### Assessment

1. Write do-now based off of [assessments from previous lesson](../3-div/assessments/).
2. Write exit-ticket based off [assessments from current lesson](assessments/).

Students will show progress toward reaching the objective based on their performance on the exit-ticket quiz.

### Vocabulary

* Library
* Twitter bootstrap

### References

* http://getbootstrap.com/css/
* http://www.bootply.com/new#
* http://www.sitepoint.com/understanding-twitter-bootstrap-3/

## During class

### Do-now

1. Attendance: Teacher takes student attendance at www.kinvolved.com
2. Return graded do-now and exit ticket from previous class
3. Do-now quiz

### Opening

Today we will learn about Twitter bootstrap. This is important because bootstrap lets us create simple and clean looking web pages without spending a lot of time. It connects to what we've previously learned because we will able to use CSS classes written by others to style our pages.

What's CSS? How is it different than HTML? What's a CSS class? How about ID? When do we use one versus the other?

### Introduction of new material ("I do")

####Getting started

**Twitter bootstrap** is a CSS and JavaScript library written by former Twitter employees. A **library** is a body of code that others have written to make our lives easier. Rather than writing our own CSS which takes time, we can use Bootstrap's styles in our HTML pages. 

For this unit, we will only look at the CSS aspects of Bootstrap.

#####Installation

We first need to bring Bootstrap into our project. We do this by using the ``<link>`` tag in the ``<head>...</head>`` section of our page. Starting from scratch, our HTML code should look something like this:

```html
<html>
  <head>
    <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css">
    <title>My first bootstrap page!</title>
  </head>
  <body>
    Hello world!
  </body>
</html>
```
Note the link where the Bootstrap CSS file is located. Another website is hosting this file for us. This is convenient because we don't have to download the file and store it in our own project.

####Deep dive

Let's take a look at a single element before the inclusion of Bootstrap and afterwards. Consider the following code:

```html
<html>
  <head>
    <title>Hello world!</title>
  </head>
  <body>
    <button type="button" class="btn btn-default">Click me</button>
  </body>
</html>
```

Click [here](http://jsbin.com/quxeg/1/) to see what this code looks like. Using the Chrome browser, right click on the button and click on "Inspect element". Look at the right side of the new screen. It should look something like:

![image](http://i.imgur.com/Aq8CQOp.jpg)

These are all the styles being applied to that button. But wait. We don't have a CSS file in our project. We haven't written any styles for our button so where are these styles coming from? These styles are coming from the browser. Every browser has its default styles. 

Let's now insert bootstrap into our code above. Consider the following code:

```html
<html>
  <head>
    <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css">
    <title>Hello world!</title>
  </head>
  <body>
    <button type="button" class="btn btn-default">Click me</button>
  </body>
</html>
```
Click [here](http://jsbin.com/vaguto/1/) to see what this code looks like. Notice that the button looks different. Again, right click on the button and click on "Inspect element." It should look something like:

![image](http://i.imgur.com/72KRqeD.jpg)

Notice the new styles being applied to the button. Also note that they are all coming from bootstrap.min.css which is the file we're bringing in using the ``<link>`` tag.

This is the power of Boostrap. By just including one file into our HTML file, we get hundreds of styles for free. Our button now looks better than the default version and we didn't even have to write any CSS to accomplish that.

####Text

Bootstrap has many styles for controlling the appearance of text. Go [here](http://getbootstrap.com/css/#type) for more details.

####Grid system

Bootstrap offers a grid system that lets you arrange you content in columns and rows. Using this structure will also make your webpage viewable in different sizes such as on a smartphone.

Consider the following code:

```html
<html>
  <head>
    <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css">
    <style type="text/css">
      .col-md-1
      {
        background-color: red;
        border: 1px solid;
      }
      .col-md-4
      {
        background-color: lightblue;
        border: 1px solid;
      }
      .col-md-6
      {
        background-color: lightgreen;
        border: 1px solid;
      }
      .col-md-8
      {
        background-color: pink;
        border: 1px solid;
      }      
    </style>
    <title>Hello world!</title>
  </head>
  <body>
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
        <div class="col-md-1">.col-md-1</div>
      </div>
      <br/><br/>
      <div class="row">
        <div class="col-md-8">.col-md-8</div>
        <div class="col-md-4">.col-md-4</div>
      </div>
      <br/><br/>
      <div class="row">
        <div class="col-md-4">.col-md-4</div>
        <div class="col-md-4">.col-md-4</div>
        <div class="col-md-4">.col-md-4</div>
      </div>
      <br/><br/>
      <div class="row">
        <div class="col-md-6">.col-md-6</div>
        <div class="col-md-6">.col-md-6</div>
      </div>
    </div>
  </body>
</html>
```
Click [here](http://jsbin.com/cureg/1/) to see the produced page. 

Let's break this down. There are four rows total in this grid. In the first row, there are 12 columns each sized with 1 unit. In the second row, there are two columns sized 8 units and 4 units respectively. In the third row, there are three columns equally sized 4 units. Finally, in the last row, there are two columns each sized 8 units.

These units specify the width of the column. Bootstrap allows for the total width of a row to add up to 12 units maxiumum. 

### Guided practice ("We do")

We're going to make a page about your school with Boostrap in it. Let's have the [reference](http://getbootstrap.com/css/) documentation open.

1. Let's start from scratch and create an empty page. Let's get our `head` and `body` tags correct.
2. Let's include Bootstrap into it.
3. Let's use the `h1` tag at the very top to include the name of your school.
4. Let's use the `h2` tag to write an "Address" heading. 
5. Let's use the `address` tag that Bootstrap offers to write down the address of your school.
6. Let's make another `h2` tag to write an "Alma mater" heading.
7. Let's use the `blockquote` tag that Bootstrap offers us to write down your school's alma mater.
8. Let's make another `h2` tag to write a "Roster" heading.
9. Let's create a grid with 3 equally sized columns using Bootstrap's grid system. Each cell of the grid should have the name of a student in our Code Park class.

### Independent practice ("You do")

Repeat the exercise above with the following changes:

1. Do it for the college you wish to attend in the future.
2. For (9), make the grid have 4 equally sized columns. Fill it with the name of alumni; you can get names from the "Notable alumni" section of the college's Wikipedia entry.
3. Add another sub-heading and call it "Campus". Include a picture of the campus shaped in a circle. Hint [here](http://getbootstrap.com/css/#images).

#### Exit ticket

Give exit-ticket quiz.

### Closing

Today you learned about Twitter bootstrap. This is important because Bootstrap allows us to create clean and elegant HTML without writing additional CSS>

#### Homework

There is no homework for this lesson. Point students to the project instead.

## After class

* Grade do-now & exit-ticket. Record in class spreadsheet.
* Prepare for next lesson / hand off to next volunteer in rotation.

