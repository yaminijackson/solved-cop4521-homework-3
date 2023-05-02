Download Link: https://assignmentchef.com/product/solved-cop4521-homework-3
<br>
The objective is to make sure

<ol>

 <li>You are familiar with the principles of Information Management.</li>

 <li>You can set up a simple Database and interact with it using SQL.</li>

 <li>You can set up a flask server in a Python application to work with the Database.</li>

</ol>

<h1>1           Specifications</h1>

For this homework you will be using the sqlite3 and flask libraries to create a database for a text-only ratings and reviews website, to be used by local restaurants. Samples for the different pages of the web application are shown on Section 3. Please make sure you conform to the following specifications:

<ol>

 <li>Create a sqlite3 database for your application. Call it db (1 points)</li>

 <li>Write a Python script called py that connects to the database and creates the tables specified in Steps 3 and 4. (1 points)</li>

 <li>Create a table called Reviews with the following fields ( 1 points):

  <ul>

   <li>Username – 40 character text field</li>

   <li>Restaurant – 50 character text field</li>

   <li>ReviewTime – SQL Datetime</li>

   <li>Rating – float</li>

   <li>Review – 500 character text field</li>

  </ul></li>

 <li>Create a table called Ratings with the following fields (1 points):

  <ul>

   <li>Restaurant – 50 character text field</li>

   <li>Food – float</li>

   <li>Service – float</li>

   <li>Ambience – float</li>

   <li>Price – float</li>

   <li>Overall – float</li>

  </ul></li>

 <li>Create an HTML page called html. This page will serve as the homepage for the website. It should include a Welcome Message and links to take users to the other pages in the website. (1 points)</li>

 <li>Create an HTML page called html. This page will display a form for a user to submit a review for a local restaurant. This will include a “Submit” button. Upon clicking the submit button, the application should insert a row in the Reviews and Ratings tables. (1 points)</li>

 <li>Create an HTML page called html. This page will display a form for a user to get all the reviews for a particular restaurant. This will include a “Submit” button that will fetch all the reviews for the given restaurant from the Reviews table and show them in the showReviews.html page. (1 points)</li>

 <li>Create an HTML page called html. This page will display the Username, Review and Overall ratings for a particular restaurant in a table format. This page will be rendered as a result of clicking on “Submit” in the getReviews.html page. (1 points)</li>

 <li>Create an HTML page called html. This page will fetch and display all the ratings of the top – 10 restaurants by overall rating. If different restaurants have the same overall rating, order them alphabetically. If there are fewer than 10 restaurants in the database, show all of them. (1 points)</li>

 <li>All pages except the homepage should have a “back to home” link. (1 points)</li>

 <li>Write a Python script called py that is going to essentially run the application. This script should contain functions to:

  <ul>

   <li>A function to render the homepage for the root directory of the application. ( 1 points)</li>

   <li>A function to add rows to the 2 tables triggered by submitting the form on html. The data from a single form should be separated into data pertinent to each table and then run</li>

  </ul></li>

</ol>

2 SQL insert queries. Make sure you handle exceptional situations by rolling back. (2 points)

<ul>

 <li>A function to fetch all reviews for a restaurant, triggered by submitting the form on html and rendering showReviews.html. (2 points)</li>

 <li>A function to run the query to get the top-10 restaurants and render the html page. (3 points)</li>

 <li>If this were the main module, run the application. (1 points) 12. Please make sure your submission is well documented (1 points)</li>

</ul>

<ol start="13">

 <li>Your submission tar should contain the following files:

  <ul>

   <li>py</li>

   <li>py</li>

   <li>html</li>

   <li>html</li>

   <li>html</li>

   <li>html</li>

   <li>html</li>

  </ul></li>

 <li>Please note that the SQL commands should handle ALL of the database interactions. You shouldnot be using Python functions to filter the results returned by a slecte all or similar SQL command.</li>

 <li>flask requires that the templated HTML files will be in a folder called “templates” in the same folderas the python file. We will use the same setup for tests, even if folder organization is not required for submission.</li>

</ol>

<h1>2           Sample</h1>

You do not have to worry about verifying if the data entered by the users would fit in the text fields. The user ratings will also definitely be a number between 1 and 5 (inclusive). This verification will usually be handled by client-side Javascript. This is not the objective of the assignment, nor is it one of the learning objectives of the course.

The samples below are strictly functional and are not very aesthetic, again because that would be handled by client-side CSS, which is not one of the objectives of the assignment.

<ol>

 <li>html</li>

 <li>html</li>

 <li>html</li>

 <li>html</li>

 <li>html</li>

</ol>

<h1>3           General Guidelines</h1>

<ul>

 <li>Add a comment with your name, FSUID, the due date and the line “The program in this file is the individual work of <em>&lt;</em>your name<em>&gt;</em>” on all files. Not having this in each of your files would result in a loss of 1 points.</li>

 <li>Create a tarball called tar with all your files. This is the only file you will be turning in.</li>

 <li>If we have listed a specification and allocated point for it, you will lose points if that particular item is missing from your code, even if it is trivial.</li>

 <li>Your outputs will be different from mine depending on the data in your database.</li>

 <li>Your program should load and run without issues. Every interpretation error or HTML/flask exception or SQL error will result in a loss of 1 points each.</li>

 <li>You are restricted to standard Python (built-ins), sqlite3 and flask Use of any other libraries would result in loss of 2 points per library.</li>

 <li>Testing your program thoroughly is a part of writing good code. We give you sample runs to make sure you match our output requirements and to get a general idea of how we would test your code. Only a file turned in through Canvas counts as a submission. A file on your computer, even if it has not been edited after the deadline, does not count.</li>

 <li>Please adhere to the Academic Honor Policy.</li>

 <li>The student is responsible for making sure they have turned in the right file(s). We will not accept any excuses about inadvertently modifying or deleting files, turning in incomplete tarballs, or turning in the wrong files.</li>

</ul>